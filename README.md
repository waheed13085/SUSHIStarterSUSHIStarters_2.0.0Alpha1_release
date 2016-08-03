# SUSHIStarterSUSHIStarters_2.0.0Alpha1_release
CONTENTS OF THIS FILE ---------------------
* Requirements and notes 
* Installation 
* SUSHIStarters Extensions  
* More information 

REQUIREMENTS AND NOTES ----------------------
 
SUSHIStarters requires:
* Apache Web Server (version 2.0 or greater) is recommended e.g. WAMP Server version 2.5 or above (http://www.wampserver.com/en/). 
* PHP 5.1.6 (or greater) (http://www.php.net/). 
* Access to the internet to harvest information

Security issues
* SUSHIStarters stores and exposes sensitive/confidential information, including: Requestor IDs, Customer IDs, usernames, passwords, usage statistics. 
* It is VERY IMPORTANT that you secure the application from prying eyes!
    * Best option: install SUSHIStarters on a server in your internal network and give it internet access via a firewall
    * Or, if you have to: install SUSHIStarters on a public access server and secure it using HTTP Basic Authentication, SSL, Shibboleth etc. (Consult your IT security experts!)
 
INSTALLATION ------------
 
1. Download and extract the SUSHIStarters distribution file
 
You can obtain the latest SUSHIStarters release from http://?????????? -- the files are available in .zip format and can be extracted using most compression tools.
 
Extracting the distribution file will create a new directory SUSHIStarters-x.y.z/ containing five main directories and five other files:

    * SSIncludes     --- Directory
    * SushiStarters  --- Directory
    * schedule       --- Directory
    * get            --- Directory
    * config         --- Directory 

    * home.html.php     --- HTML file
    * Index.php         --- HTML file 
    * ReadMe.txt        --- Text file for instructions
    * License.txt       --- License file
    * sushistarters.css --- CSS file    

2. Put the five SUSHIStarters directories and the five file contents into required locations

    * Copy or move the SSIncludes directory and contents into your Apache Web root folder (e.g. \wamp\www\ or C:\wamp\www\)
    * Copy or move the SushiStarters directory and contents into your Apache Web root folder (e.g. \wamp\www\ or C:\wamp\www\)
    * Copy or move the schedule directory and contents into your Apache Web root folder (e.g. \wamp\www\ or C:\wamp\www\)
    * Copy or move the get directory and contents into your Apache Web root folder (e.g. \wamp\www\ or C:\wamp\www\)
    * Copy or move the config directory and contents into your Apache Web root folder (e.g. \wamp\www\ or C:\wamp\www\)
    * Copy or move the home.html.php file into your Apache Web root folder (e.g. \wamp\www\ or C:\wamp\www\)
    * Copy or move the Index.php file into your Apache Web root folder (e.g. \wamp\www\ or C:\wamp\www\)
    * Copy or move the ReadMe.txt file into your Apache Web root folder (e.g. \wamp\www\ or C:\wamp\www\)
    * Copy or move the License.txt file into your Apache Web root folder (e.g. \wamp\www\ or C:\wamp\www\)
    * Copy or move the sushistarters.css file into your Apache Web root folder (e.g. \wamp\www\ or C:\wamp\www\)


3. Set directory ownership and permissions

The web server needs (read + write) permissions on two directories and their contents, namely:

    * SushiStarters/params/  
    * SushiStarters/filestore/
 
4. Configure SUSHIStarters 

You just need to set two variables to configure SUSHIStarters!

Using your preferred text editor, open up helpers.inc.php which is in the SSIncludes directory, and set:

    * $SSRoot  : the URL of the webclient
    * $SSPath  : Path to SUSHIStarters directory containing the filestore, params and CLI scripts

5. Verify that the Apache Web server is running.

Open your favourite web browser and access your web server using http://localhost

Usage ------------  

1. Once the application is loaded; one can see that there are four tabs.

    * Home               - This is the main lainding page of the web application 
    * Configure Services - Here the settings for the SUSHI can be amended as per the requirement. 
    * Get Report         - For here the user can download the required SUSHI reports. While downloading the report either user can save to the directory \SUSHIStarters\filestore or their own desired location.  
    * Schedule Report    - Here reports can be scheduled as per need. Further detail mentioned on the page.

 
