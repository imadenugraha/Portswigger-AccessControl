# Unprotected Admin Functionality

> Category : Access Control

> LAB : https://portswigger.net/web-security/access-control/lab-unprotected-admin-functionality

## Description

This lab has an unprotected admin panel.
Solve the lab by deleting the user carlos.

## Write Up

1. Click on "Access Lab" to enter the lab.
   
2. The page will look like this:
   
   ![image1](1.png)

3. Add **/robots.txt** after the url and dissalow page will show up:
   
   ![image2](2.png)

4. Replace **/robots.txt** with **/administrator-panel** after the url.
   
   ![image3](3.png)

5. After you enter the administrator panel, you will see there are 2 users in the screen. According to the Description, delete user with name **carlos.**
   
   ![image4](4.png)

6. Task complete.
   
   ![image5](5.png)