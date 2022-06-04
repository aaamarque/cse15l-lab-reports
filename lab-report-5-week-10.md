# Lab Report 5 week 10
## Vimdiff
- To find the test with different results I used vimdiff

![Screenshot 4](Screenshot%20(626).png)

## Links to the test-file with different-results

[Link 1 Test](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/194.html.test)



[Link 2 Test](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/195.html.test)

## Test #1
- For the first test both implementations are wrong, it gives the wrong output. Because it's supposed to pick up foo*bar

![Screenshot 4](Screenshot%20(628).png)

Expected output

![Screenshot 4](Screenshot%20(631).png)

- My implementation picks up url becuase of the paranthesis around it. Because  **openparen** and **closeParen**. Since it finds a pair my program it's going to pick it up and add it to the links.

![Screenshot 4](Screenshot%20(632).png)

## Test #2
- For the second test both implementations are wrong, it gives the wrong output.

![Screenshot 4](Screenshot%20(628).png)

Expected output

![Screenshot 4](Screenshot%20(633).png)

- My implementation picks up nothing because becuase there is nothing surrounding it, there is no pair. 













