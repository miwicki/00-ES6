# 1-ES6-practice

## Feature Tasks

Follow these instructions carefully and in order.

1. Open the HTML file in the browser to ensure that it works.
2. Turn all `var` variable declarations into `let`.
3. After you do, there will be one error. Find that line in the code, delete that line and respond to the adjacent TODO item.
4. Return to the browser to ensure that the code works again.
5. **Save the code, and do a Git "add" and "commit".**
6. Now, in the code, convert all `let` variable declarations into `const`.
7. Bugs will erupt everywhere. Debug by using the error messages in the browser console, turning `const` declarations back into `let` where necessary. Expect there to be some back-and-forth between your code editor and your browser.
8. When you think you have things working, clear local storage and reload the page to ensure that the code still works when starting from a totally clean state.
9. **Save the code, and do a Git "add" and "commit".**
10. Now find all concatenations in the code and convert them into template literal notation.
11. Reload the browser to ensure that the code works as expected.
12. **Save the code, and do a Git "add" and "commit".**
13. Answer the following questions:

---

##### Investigate how `let` and `const` are now used in the code. Where did you need to convert `const` into `let` to make the code work? Can you identify any patterns/similarities?

For repeated uses of i, 'let' had to be used each time in order to redefine the variable for a new loop, as 'const' variables cannot be redefined.  
For counters, like the variable totalClicks, the counter is always being redefined as a new number (theoretically being added to or detracted from) so it is by definition not constant.  
For constructor functions, where new instances of the constructor are being added throughout the code, the array of instances cannot stay constant, as new instances are being added.  

It seems like for small blocks of simple code 'let' and 'const' would have the same effect, but for larger and more complicated pages, they have very different uses.  As 'const' cannot be redefined, I can't see it being used very often in pages involved user input and saving that user data.

---

##### How did it go with making the adaptation from concatenations to template literal notation? Do you think you'll mostly use template literal notation from now on?

YESSSS ITS SO MUCH BETTER!!!! Once you've done it once it's not very difficult at all, and not having to worry about the spacing between words and plus signs is so much more intuitive and easy to read/check.  
