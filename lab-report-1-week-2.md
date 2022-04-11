## **Tutorial: course-specific account on ieng 6** 

# Installing VScode 
Hello! 
Before showing how to log into a course-specific account on **ieng6**, first we need to download VScode. This is a source-code editor, basically is where you are going to be coding!

- Go to this website [VScode Link](https://code.visualstudio.com/Download). In this link, you will find all the versions for all the major operating systems, like for Macs and Windows. When is installed correctly, it should look something like this: 
![VSCode Installed](Screenshot%20(556).png)

# Remotely Connecting
We will be using course-specific accounts, to help connect your machine to a remote computer over the Internet. 

- First, if you are on Windows you need to [Install OpenSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse).
- Second, you will need to look up your course-specific account for your class [here](https://sdacs.ucsd.edu/~icc/index.php). For example, for UCSD the class CSE15L, should look like this **cs15lsp22zz@ieng6.ucsd.edu** 
- Then, we are going to use VSCode to connect to a remote computer.
- Open a terminal in VSCode and put **ssh** in front of your course-specific account, like this **ssh cs15lsp22zz@ieng6.ucsd.edu**, it should look something like this in your terminal.
Say yes to questions if it asks, and then it's going to ask for your password so make sure you remember.
![ssh connection](Screenshot%20(390).png) It might look a little bit different in your termial but at least make sure at the end there is like a table like the picture. 
# Trying Some Commands
Once you are log in with you course-specific account you can try some commands in the terminal. Some commands you can try: 
- cd
- ls -lat
- ls -a

It should look something like this...










