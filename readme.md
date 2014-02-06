Wordpress New Project Config
====================

##What is Wordpress New Project Config?
This little script will save you the hassle of all the repetitives tasks each time you start a new wordpress project.

##So what it does?
The script will
- Prompt you for a project name
- Create a new folder with the project name
- Fetch and Install the latest wordpress build
- Remove readme.html and license.txt
- Fetch your favorite starter theme and rename it with your project name
- Remove twentyten, twentyeleven and twentytwelve themes
- Fetch a list of plugins you want on every projects
- Remove Hello Dolly plugin
- Fetch H5BP server-configs .htaccess
- Create a database with your project name
- Prompt you for a table prefix
- Configure wp-config.php and change update salt strings
- Create a wp-config-local.php file for local database parameters 
- Exclude wp-config-local.php in .gitignore and Sublime ftp config file 
- Create a Sublime text 2 project config file (projectName.sublime-project)
- Configure .sublime-project file with 3 folders : 
	- My theme
	- plugins
	- All website (it will be helpfull for the 1st migration on a remote server)
- Prompt you if you want to configure ftp for Sublime text 2
- Create a Sublime text 2 sFTP config file sftp-config.json in each folder.
- Create a new project in codeKit 
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
Just duplicate config-sample.cfg to config.cfg

##Configuration
You can edit the script with your favourite code editor and change some variables.
- DIRECTORY you can type your projects folder path
- WORDPRESS_URL must be a zip to download, I use zip download rather than a git repository cause I personally fetch a locale (french) version of wordpress 
- THEME_URL must be a git repository
- PLUGINS_URL is a list of plugins from the wordpress.org plugin directory
- DB_USER, DB_PASSWORD, DB_HOST these are the defaults for MAMP
- LOCAL_URL default is localhost:8888/ for MAMP but you could have changed it

and for sure, you can modify or delete some part not useful for you

##Why a .command extension?
The script is a common shell script with normally a .sh extension  
The .command extension allow to make the script double clickable  
Tip : If you are using Alfred or an other launcher application, you can execute the script from everywhere! 

##Changelog

###v1.3.2
- fixe a mySQL issue
- Remove twentythirteen and twentyfourteen theme
- Update fetching of the new H5BP .htaccess

###v1.3.1
- Add mysql path in the config file 
- Add sublime text path in the config file

###v1.3
- Now you can fetch a list a plugins from the wordpress.org plugin directory

###v1.2.2
- Fixed the path for browser launching (thanks to <a href="https://github.com/aarow" >Aarow</a>)

###v1.2.1
- Fixed sftp config process (thanks to <a href="https://github.com/carlesjove" >Carles Jove</a>)

###v1.2
- Do not allow empty strings on FTP config, and allow to abort process (thanks to <a href="https://github.com/carlesjove" >Carles Jove</a>)

###v1.1.2
- Empty values are now not allowed for project name (thanks to <a href="https://github.com/carlesjove" >Carles Jove</a>)

###v1.1.1
- Fixed table_prefix issue

###v1.1
- Split the configuration part in an another file config.cfg
- gitignore config.cfg