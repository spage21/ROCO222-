#Basic Linux commands

**1- ls**
lists all files and folders in your current directory

**2- cd**
lets you change directory, got into other folders you can use "cd .." to go back a folder.

**3- mkdir** 
used to create a new folder or subfolder. "rmdir" will remove any empty directory

**4- sudo**
basically an override command. put sudo before something to force it.

**5-cp**
stands for copy and paste. first determine the file you want to copy and type the destination location to paste the file.

_$ cp (file name) (location you want to paste too)_

**6- rm**
remove. its a command used to delete your file or even your directory. you can use -f if the file needs root permission to be removed. 

_$ rm myfile.txt_

**7- apt-get**
this command is to install, remove and upgrade any package. apt advanced packaging tool. the 
apt-get command will help you install software. its a powerful command line which can perform installation, upgrade and even remove software.

_$ sudo apt-get update_

**8-grep**
if you need to find a file but cant remember its exact location or path grep will help you solve this problem.

_$ grep user /etc/password_

**9- cat**
it will show you text inside your file.

_$ cat Cmakelists.txt_

**10- poweroff**
sometimes you need to power off directly from the terminal this command will need a sudo before it to work.

_$ sudo poweroff_

**11- pwd** 
to know what directory youre in type pwd in the terminal

**12- df**
the df command is used to see the availble disk space in each of the partitions of your system in KB if you want to see it in mbs type "df -m"

**13- zip and unzip**
zip is a command used to compress files into a zip archive. unzip is used to extract files from a zip archive.


#What is Markdown ?

-Markdown is a way to style text on the web. you can control the display of the document. you can format the words as bold or italic, add images etc....Mostly markdown is just regular text with a few non-alphabetic characters like # and *. you can use markdown is most places around git hub, like gists comments in issues and pull requests and files with ".md" and ".markdown" extentions

using a single '#' all the words after it will become a heading

using two * before and after words makes them all bold

using one _ before and after words puts them in italics

using two ~ before and after words puts a line through them. (though I cant seem to get it to work)

#Notes on GitHub
saving markdown document using commits and github.
first open terminal and type  _git init_ then navigate into the directory using _Cd_ and _ls_ after making changes to a markdown document  write _git status_ and you can see the files that you have changed. to save these files type _git add_ then the file name. once youve added all the files you want to save type git commit and an appropriate message then _ctrl X_ and _Y_ after this is type _git log_ to check the commit has been made successfully.

#Lab 2, Creating a DC motor.












