# Remote Access Tutorial - Minghan Wu

## Part I - Installing Visual Studio Code

To install VS Code, go to the [VS code website](https://code.visualstudio.com/)

![image](https://github.com/MinghanWu039/cse15l-lab-reports/blob/0e39e588b1c2d4504c37e916c74dc309a26eb76b/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8B%E5%8D%883.01.23.png?raw=true)

Click "Download Mac Universal" (if you are using a Windows then use the scroll button) and proceed by following the instructions.

I have installed VS code on my computer so no screenshots available for the installation process.

After you install successfully, you should see this when you run VS code (for Windows it's something similar):

![image](https://github.com/MinghanWu039/cse15l-lab-reports/blob/6b8b2913bc08cb8226aa8a92bbbbc477200ff274/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8B%E5%8D%882.17.34.png?raw=true)

-----------------------------------
## Part II - Remotely Connecting

In order to remotely connect to a remote server, you need to have a CSE15L account first and have changed the password.

To do so, follow the instructions on this [link](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit)

Then, if you're a Windows user, please refer to the part 4 of this [link](https://ucsd-cse15l-w23.github.io/week/week1/) to install gitbash.

The next steps will be done in VS Code. Open VS Code. To open the terminal, either click "Terminal" -> "New Terminal" or control+shift+` (for mac)

The terminal should look like this:

![image](https://github.com/MinghanWu039/cse15l-lab-reports/blob/c2136a4fa71ec100e896a4163f2863fc60cca136/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8B%E5%8D%883.37.22.png?raw=true)

Then, to use ssh, put in this command: ```ssh cs15lwi23zz@ieng6.ucsd.edu```  where zz should be replaced by your 3-letter course username. Mine is ```aur```.

![image](https://github.com/MinghanWu039/cse15l-lab-reports/blob/0a154c0fa893d8f061dd8499ea86283acbf97ec9/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8B%E5%8D%883.44.26.png?raw=true)

If it's the first time you access this server, you will likely get this message:
 ```
The authenticity of host 'ieng6-202.ucsd.edu (128.54.70.227)' can't be established.
 
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.

Are you sure you want to continue connecting (yes/no/[fingerprint])? 
```

Select "yes" and enter your password. If you have just changed your account password, you should wait about 10 min for the system to update.

Note that the password you enter will not appear on the screen.

After that, you should find this:

![image](https://github.com/MinghanWu039/cse15l-lab-reports/blob/7b0dd92d4966fef47b6c4b33cb74845c7987341a/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8B%E5%8D%883.48.12.png?raw=true)

------------------------------
## Part III - Trying Commands

You can try the following commands:

 ```ls``` -- list files

```cd + (directory)``` -- change directory

```ls -lat```

```ls -a```

```ls\<directory\>``` -- where ```\<directory\>``` is ```/home/linux/ieng6/cs15lwi23/cs15lwi23abc``` where ```abc``` is someone else's username

```cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/```

```cat /home/linux/ieng6/cs15lwi23/public/hello.txt```

Here is an example of me inputting ```ls -lat``` before opening the file hello.txt:

![image](https://github.com/MinghanWu039/cse15l-lab-reports/blob/86670f23a252caed6a68895599e62c39e813e7bc/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8B%E5%8D%885.00.05.png?raw=true)

In comparison, here is what happens when I input ```ls -a``` and ```ls -la```:

![image](https://github.com/MinghanWu039/cse15l-lab-reports/blob/a5ab65ae88a25dc50e20ac8bcb2546b6d5c1c374/%E6%88%AA%E5%B1%8F2023-01-25%20%E4%B8%8A%E5%8D%8811.11.02.png?raw=true)

![image](https://github.com/MinghanWu039/cse15l-lab-reports/blob/a5ab65ae88a25dc50e20ac8bcb2546b6d5c1c374/%E6%88%AA%E5%B1%8F2023-01-25%20%E4%B8%8A%E5%8D%8811.11.19.png?raw=true)

Observe that ```ls -a``` just shows every file name; ```ls -la``` lists the long format of them; On top of that, ```ls -lat``` sorts the files by time and date.

Finally, to log out, type the command ```exit```.
