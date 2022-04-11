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
![Trying some commands](Screenshot%20(560).png)

# Moving Files with scp
There is many ways to copy a file from your computer to a remote computer. We will be using the command **scp**, which will always be used when not logged into **ieng6.** 
- First, you will create a file in your computer called **WhereAmI.java** and copy the following code onto that file: 
```
class WhereAmI {
public static void main(String[] args) {
System.out.println(System.getProperty("os.name"));
System.out.println(System.getProperty("user.name"));
System.out.println(System.getProperty("user.home"));
System.out.println(System.getProperty("user.dir"));
}
}
```
- Second, in the same terminal and directory where you made the file, run the following command: 

```
scp WhereAmI.java cs15lsp22zz@ieng6.ucsd.edu:~/
```
- Then, log into ieng6 with **ssh** and use **ls**, you should see the file that you just created! And you should be able to run it with **javac** and **java!**

After you are done it should look something like this...
![Running the command javac and java when logged in (ieng6)](Screenshot%20(561).png)

And that's how you copy a file from your computer to a remote computer!

# Setting an SSH Key
In order to avoid repeating the task of logging in and putting the password over and over again the **ssh keys** will be very useful. In order to set up ssh keys: 
- First, on your computer run this command `ssh-keygen` (DO NOT add a **paraphrase**), You should end up with something like this...
![ssh-keygen](Screenshot%20(562).png)
- Second, log in to the server with ssh and your course-specific account `ssh cs15lsp22zz@ieng6.ucsd.edu` then, put `mkdir .ssh` and log out after that. 
- Lastly, write `scp /Users/<user-name>/.ssh/id_rsa.pub
cs15lsp22zz@ieng6.ucsd.edu:~/.ssh/authorized_keys` replacing user-name with the one in tha path. 

# Optimizing Remote Running
There are ways to make the use of time more efficient. For example, you can use a command and combine it with ssh to make things go faster. 
`ssh cs15lsp22are@ieng6.ucsd.edu "ls" `
![1st command](Screenshot%20(564).png)

or 

you can also run multiple commands on the same line of the termina like this...
`cp WhereAmI.java; javac OtherMain.java; java WhereAmI`
In your terminal it should look like this...
![2nd command](Screenshot%20(565).png)
















