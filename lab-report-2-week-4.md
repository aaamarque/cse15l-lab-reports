## Lab 2
# There is going to be three code changes

# First Code Change
- The screenshot below is a screenshot of the code change diff from Github.

![Screenshot](Screenshot%20(573).png)


- This is the link to the failure-inducing input.
[Link: Failure-Inducing Input](https://github.com/aaamarque/markdown-parser/commit/026b3f3372b861540caa14c8c2f1d24f4e59de9b)



- This screenshot shows without the fix there would be an infinite loop. The terminal shows how it's in an infinite never ending.

![Screenshot 2](Screenshot%20(575).png)

- There is a bug, which was that it couldn't handle open brackets. So when I tested a file with one missing brackets it was given the symptom of an infinite loop when testing with the test file. The reason why the test case would give an infinite loop it's because the variables for the braces and paranthesis were always looking for the other parenthesis or bracket when it wasn't there so it would crash. 

# Second Code Change

- The screenshot below is a screenshot of the code change diff from Github.

![Screenshot](Screenshot%20(579).png)

- This is the link to the failure-inducing input. (When you click the link the test is on the bottom of the page)
[Link: Failure Inducing Input](https://github.com/aaamarque/markdown-parser/commit/baadd0ca92fbcf639f8c637fce072570c4ba4948)


- This screenshot shows without the fix it would be producing the wrong answer. The terminal shows how it picked up the image putted in the list, when it's not supposed to do that. 

![Test failed 4](Screenshot%20(578).png)


- There was a bug that gave the symptom of the wrong answer. When testing with the test with the image link it would put it in the list giving the wrong answer. This was happening because the image, the format of inserting an image, had the brackets and braces and so it would ignore the "!".


# Third Code Change

-  The screenshot below is a screenshot of the code change diff from Github.

![Image](Screenshot%20(581).png)

- This is the link to the failure-inducing input.(it's on the bottom of the page)

[Link to the failure-inducing input](https://github.com/aaamarque/markdown-parser/commit/2d5f66b46bcaea1203ed3d228f26734b2eeb475f)

- This screenshot shows without the fix it would cause the wrong output. The terminal shows how it picked up the two strings that weren't even links, and added them to the list. 

![Image](Screenshot%20(582).png)



- There was a bug that gave the symptom of the wrong answer. What was happening is that since the two strings had the brackets and paranthesis it would add them to the list. The test case had the format of the link so that's why it would cause the wrong output. 



