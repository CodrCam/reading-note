# Reading 13

## Local Storage and How To Use It On Websites

- Why would a developer use local storage for a web application?

1. Persistence: Local storage provides a way to store data on the client side that persists even after the user closes the browser or navigates away from the page. This makes it useful for storing user preferences, session information, and other data that needs to be available across multiple visits to the web application.
2. Performance: By storing data locally, the web application can reduce the number of server requests needed to retrieve data, which can improve performance and reduce network traffic.
3. Offline access: Local storage can be used to enable offline access to a web application by storing data locally and syncing it with the server when the user goes online.
4. Security: Local storage is considered more secure than cookies, as it provides a way to store data on the client side without sending it to the server with every request.
5. User experience: By using local storage, a web application can provide a smoother and more seamless user experience by reducing the need for users to re-enter data or settings every time they visit the site.

- What information should not be stored in local storage?

 Here are some types of information that should generally not be stored in local storage:

1. Sensitive personal information: Local storage is not an appropriate place to store sensitive personal information such as passwords, credit card numbers, or other sensitive data that could be used to compromise a user's identity or financial security.
2. Session tokens: Session tokens are used to authenticate users and grant them access to protected resources. If a session token is stored in local storage, it could be vulnerable to theft by malicious actors who could use it to gain unauthorized access to the user's account.
3. Large amounts of data: Local storage is limited in terms of the amount of data it can store. If a web application attempts to store large amounts of data in local storage, it could slow down the performance of the application and cause it to become unresponsive.
4. Information that needs to be kept in sync with the server: If data needs to be shared between the client and server, local storage may not be the best choice for storing that data. In this case, it may be better to use server-side storage or a different client-side storage mechanism, such as IndexedDB.

- Local storage can store what type of data? How would you convert it to that type before storing?

Here are some common types of data that can be stored in local storage and how to convert them to strings:

1. Strings: Since strings are already in text format, they can be stored directly in local storage without any additional conversion.
2. Numbers: To store a number in local storage, it must first be converted to a string using the toString() method. For example, var num = 42; localStorage.setItem("myNum", num.toString());
3. Boolean values: To store a Boolean value in local storage, it must first be converted to a string using the toString() method. For example, var isTrue = true; localStorage.setItem("myBool", isTrue.toString());
4. Objects: Objects cannot be stored directly in local storage since it only supports string values. However, objects can be converted to strings using the JSON.stringify() method. For example, var myObj = {name: "John", age: 30}; localStorage.setItem("myObj", JSON.stringify(myObj));
5. Arrays: Arrays can be converted to strings using the JSON.stringify() method in the same way as objects. For example, var myArray = [1, 2, 3]; localStorage.setItem("myArray", JSON.stringify(myArray));

*It is important to note that when retrieving data from local storage, it will be returned as a string, even if it was originally stored as a different data type. Therefore, it is necessary to convert the string back to its original data type using the appropriate method (e.g. parseInt() or JSON.parse()) before using it in the code.*
