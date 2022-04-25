## Lab 2
# There is going to be three code changes

# First Code Change
- The screenshot below is a screenshot of the code change diff from Github.

![Screenshot](Screenshot%20(573).png)


- This is the link to the failure-inducing input.
[Link: Failure-Inducing Input](https://github.com/aaamarque/markdown-parser/commit/026b3f3372b861540caa14c8c2f1d24f4e59de9b)


- This screenshot shows without the fix there would be an infinite loop. The terminal shows how it's in an infinite never ending.

![Screenshot 2](Screenshot%20(575).png)

- There is a bug, which was that it couldn't handle open brackets. So when I tested a file with one missing brackets it was given the symtom of an infinite loop when testing with the test file. The reason why the test case would give an infinite loop it's because the variables for the braces and paranthesis were always looking for the other parenthesis or bracket when it wasn't there so it would crash. 

# Second Code Change

- The screenshot below is a screenshot of the code change diff from Github.

![Screenshot](Screenshot%20(573).png)





