# CS5744_project3

To start xampp  

   sudo /opt/lampp/xampp start

To open mysql     
  
  /opt/lampp/bin/mysql  

To go to the location :   
  
  cd /opt/lampp   

To open up the contrl panel(or faqs):     
  
  open localhost in chrome

-------------------------------


.htaccess :: Super Important.


-------------------------------

To change the DocumentRoot     
Open Control panel.      
cd /opt/lampp     
sudo ./manager-linux-x64.run       
Open "configure"        
Change (both lines together :        
DocumentRoot from: "/opt/lampp/htdocs"       
To place where you are storing your files (No trailing /)         
Example: "/home/apache"          
 

--------------------------------


To place php in a file, include the code. Rename the file as a  .php       
So that apache can process it.
In browser , write page.php      


Another example :       
Place header in a templace.

Use the template, using           
   \<?php include_once 'template.php' ?\>



---------------------------------

.htaccess      
each folder can have its own .htaccess file


   Read tutorial on this!

use htaccess file to redirect like home.php no one likes. 

In configuration file we have mode_rewrite.  
Turn it on in htaccess here. Then we write rules.:

   RewriteEngine on  
   RewriteRule ^home$ home.php 
   RewriteRule ^$ home.php

   #Take care of trailing / like home/       
   RewriteRule^home$/?$

Now we can redirect users to a controller, rather than a template. Controller can have business logic.   
There can be multiple controllers, such as a controller per item.
See the class video!!      

Idea is to tell controller to load which view to load. Its MVC.         

This is going to be done http request methods.


