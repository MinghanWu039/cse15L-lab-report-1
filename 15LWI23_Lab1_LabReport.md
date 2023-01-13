Remote Access Tutorial - Minghan Wu
====================
Part I - Installing Visual Studio Code
----------
I have installed VS Code already on my macbook.

To install VS Code, go to the VS code website: [link](https://code.visualstudio.com/)

![Image](https://github.com/MinghanWu039/cse15l-lab-reports/blob/0e39e588b1c2d4504c37e916c74dc309a26eb76b/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8B%E5%8D%883.01.23.png)

Press "Download Mac Universal" and proceed by following instructions (if you are using a Windows then use the scroll button).

After you install successfully, you should see this when you run VS code (for Windows it's something similar):

![Image](https://github.com/MinghanWu039/cse15l-lab-reports/blob/6b8b2913bc08cb8226aa8a92bbbbc477200ff274/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8B%E5%8D%882.17.34.png)

----
Part II - Remotely Connecting
-----------
In order to remotely connect to a remote server, you need to have a CSE15L account first and have changed the password.

To do so, follow the instructions on this [link](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit)

Then, if you're a Windows user, please refer to the part 4 of this [link](https://ucsd-cse15l-w23.github.io/week/week1/) to install gitbash.

The next steps will be done in VS Code. Open VS Code. To open the terminal, either click "Terminal" -> "New Terminal" or control+shift+` (for mac)

The terminal should look like this:
![Image](https://github.com/MinghanWu039/cse15l-lab-reports/blob/c2136a4fa71ec100e896a4163f2863fc60cca136/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8B%E5%8D%883.37.22.png)

Then, to use ssh, put in this command: *ssh cs15lwi23zz@ieng6.ucsd.edu*  where zz should be replaced by your 3-letter course username.
Mine is "aur".
![Image]()

Since it's the first time you access this server, you will likely get this message:
![Image}()

Select "yes" and enter your password. If you have just changed your account password, you should wait about 10 min for the system to update.

Note that the password you enter will not appear on the screen.

After that, you should find this:
![Image]()

----
Part III - Trying Commands
-----------------

You can try the following commands:

*ls* -- list files

*cd + (directory)* -- change directory

*ls -lat*

*ls -a*

*ls\<directory\>* -- where \<directory\> is /home/linux/ieng6/cs15lwi23/cs15lwi23abc where abc is someone else's username

*cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/*

*cat /home/linux/ieng6/cs15lwi23/public/hello.txt*

Here is an example of me inputting *ls -lat* before opening the file hello.txt:
![Image]()
