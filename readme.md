Jelli Project Config
====================

##What is Jelli Project Config?
This little script will save you the hassle of all the repetitives tasks each time you start a new wordpress project.

##So what it does?
The script will
- Prompt you for a project name
- Create a new folder
- Fetch and Install the latest wordpress build
- Remove readme.html and license.txt
- Fetch your favorite starter theme and rename it with your project name
- Remove twentyten, twentyeleven and twentytwelve themes
- Remove Hello Dolly plugin
- Fetch H5BP server-configs .htaccess
- Create a database with your project name
- Prompt you for a table prefix and configure wp-config.php
- Create a Sublime text 2 project config file (projectName.sublime-project)
- Configure .sublime-project file with 3 folders : 
	- your theme
	- plugins
	- everything (it will be helpfull for the 1st migration on a remote server)
- Create a Sublime text 2 sFTP config file sftp-config.json in each previous folder.
- Create a new project to watch in codeKit 
- Launch your project in Sublime text 2
- Open your newly created wordpress website in your favourite browser

##Requirements
- I created this script for MAC, I don't know if it works on other platforms.
- MAMP
- git
- codeKit
- sublime text 2
- and sFTP plugin if you want

##Installation
JPC is a shell script with a .command extension to make it double clickable.
Copy the newproject.command file in your all projects folder
Double click
That's all

##Configuration
You can edit the script with your favourite code editor and change some variables.
- DIRECTORY you can type your projects folder path or left it blank, in this case, it will take the current folder
- WORDPRESS_URL must be a zip to download, I use zip download rather than a git repository cause I personally fetch a locale (french) version of wordpress 
- THEME_URL must be a git repository
- DB_USER, DB_PASSWORD, DB_HOST these are the defaults for MAMP
- LOCAL_URL default is localhost:8888/ for MAMP but you could have changed it

and for sure, you can modify or delete some part not useful for you







