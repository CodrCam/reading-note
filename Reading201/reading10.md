# Reading 10

## What Went Wrong? Troubleshooting JavaScript.

- Name some key differences between a Syntax Error and a Logic Error.

1. Nature of the error: Syntax errors occur when the code violates the rules of the programming language, such as missing a semicolon, using an undefined variable, or having mismatched parentheses. Logic errors, on the other hand, occur when the code produces unintended results due to flawed reasoning or incorrect assumptions in the algorithm.
2. Detection: Syntax errors are usually detected by the compiler or interpreter, which checks the code for compliance with the language syntax and reports any violations. Logic errors, however, may not be detected by the compiler or interpreter, as the code may still run without throwing any errors, but produce incorrect or unexpected results.
3. Impact on the program: Syntax errors prevent the program from being executed or compiled, whereas logic errors can cause the program to run but produce incorrect results. In some cases, logic errors can also lead to crashes, infinite loops, or other unexpected behavior.
4. Debugging: Syntax errors are relatively easy to debug, as the compiler or interpreter can point to the exact location of the error in the code. Logic errors are more challenging to debug, as they may require careful examination of the program's logic, inputs, and outputs to identify the source of the problem.

### Personal Experience

- List a few types of errors that you have encountered in past lab assignments and explain how you were able to correct them.

I was able to find both logic and syntax errors. Usually, the linter points me towards grammatical errors, while I use the console and print out variables to detect syntax errors.

- How will this topic continue to influence your long term goals?

I'm excited about the future of debugging and the streamlined way to find errors, as linters have improved significantly over time.

How would you describe the JavaScript Debugger tool and how it works to someone just starting out in software development?

1. Setting breakpoints: The first step in using the debugger tool is to set a breakpoint in your code. A breakpoint is a line in your code where you want the program execution to pause. You can set a breakpoint by clicking on the line number in the source code editor, or by using the debugger keyword in your code.
2. Examining the code: When the program execution pauses at the breakpoint, you can examine the state of your code. You can see the values of your variables, inspect the call stack, and look at the current line of code that's about to be executed.
3. Stepping through the code: You can use the debugger controls to step through your code one line at a time, or to jump to the next breakpoint. This helps you see how the program behaves and identify any errors or unexpected behavior.
4. Debugging errors: If you find an error in your code, you can use the debugger to isolate the problem and fix it. You can use the console to log messages and view the output of your code, or use the debugger's watch feature to monitor the value of a particular variable.

### Order of Operations

- What is the call stack?

The call stack is a data structure that is used by programming languages to keep track of the order in which functions are called and to remember where to return to when a function has finished executing.

When a function is called, the current state of the program, including the function's arguments and local variables, is pushed onto the top of the call stack. This creates a new stack frame, which represents the current function's execution context. The function's code is then executed, and if it calls another function, a new stack frame is created for that function and pushed onto the top of the call stack.

Each function that is called in turn creates a new stack frame, which is pushed onto the top of the call stack. When a function finishes executing, its stack frame is popped off the top of the call stack, and the program returns to the point where the function was called. The previous stack frame is then reinstated, and the program continues executing from that point.

The call stack is important for maintaining the correct order of execution of functions and for ensuring that the program returns to the correct point after a function has finished executing. It is also used to handle errors and exceptions, as the call stack can be examined to see where an error occurred and which functions were called before the error was thrown.
