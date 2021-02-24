# Call Stack

## A call stack :
is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

1. When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
2. Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
3. When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
4. If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

![image](https://miro.medium.com/max/638/1*CCHexfHNCNo-f8aw3rbRew.jpeg)

When the code is run if we get an error, A stack is printed showing how the functions are stack on top each other.
*Take a look at the diagram*

![image](https://cdn-media-1.freecodecamp.org/images/zOINLHPC8E56ac8yyINYOFWeImsjM2Wk2rdU)

## What causes a stack overflow?

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

for ex: **function callMyself(){  callMyself();}callMyself();**

## Types of error messages

1. Reference errors
2. Syntax errors
3. Range errors
4. Type errors

## Debugging

To debug your JS code, the easiest and maybe the most common way its to simply console.log() the variables you want to check or, by using chrome developer tools.

