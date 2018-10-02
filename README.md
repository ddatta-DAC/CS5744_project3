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







