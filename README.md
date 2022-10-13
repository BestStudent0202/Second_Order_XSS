# Second_Order_XSS
## Not patched web application
0. put the file in the C:\\xamp\\htdocs
1. open xampp control panel
2. click start on apache and my sql
3. click admin on my sql 
4. type in forum in the create database textbox and click create database
5. click on forum on left hand side bar
6. on the top bar press import
7. click on forum.sql
8. after import has done go to firefox/chrome type localhost/index.php

##  Second_Order_XSS_Patched HTML encoding
same step as above except step 8 if user have setup the not patch web application step above could just ignored the setup for this patch.
1. if you have injected the stored xss payload , you can click admin on mysql on xampp control panel. Click on  forum and press empty
2. go to firefox/chrome type localhost/Second_Order_XSS_Patched HTML encoding

## Second_Order_XSS_Patched Regex
same step as above except step 8 if user have setup the not patch web application step above could just ignored the setup for this patch.
1. if you have injected the stored xss payload , you can click admin on mysql on xampp control panel. Click on forum and press empty
2. go to firefox/chrome type localhost/Second_Order_XSS_Patched HTML encoding

## Explanation of each file

```Second_Order_XSS_Patched HTML encoding``` This folder shows the patching using HTML Encoding. The code is in ```main.js``` line 5 to line 12 under the function called escapeHtml, and it is used in line 59 and 60

```Second_Order_XSS_Patched Regex``` This folder shows the patching using Regex. The patch code is in ```main.js``` line 51

```conn.php``` The connection file to the database

```forum.sql``` This is the sql file for this application

```index.php``` This is the front page of the application

```main.js``` The main javascript file, used to handle all the HTTP requests between the frontend and the backend

```save.php``` This file is responsible for saving the comment into the database

```view.php``` This file is responsible for retrieving the data from the databaase and sending it to the frontend for rendering
