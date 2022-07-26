# User Role Can Be Modified in User Profile

> Category : Access Control

> LAB : https://portswigger.net/web-security/access-control/lab-user-role-can-be-modified-in-user-profile

## Description

This lab has an admin panel at /admin. It's only accessible to logged-in users with a roleid of 2.

Solve the lab by accessing the admin panel and using it to delete the user carlos.

You can log in to your own account using the following credentials: wiener:peter.

## WriteUp

1. Access the lab and go to **My Account**. Use wiener:peter to login.
   
   ![image1](1.png)

2. Start your BurpSuite enable Proxy Intercept. Back to the browser use default email of wiener and click **Update Email**. 
   
   ![image2](2.png)

3. The Intercept will get the HTTP request and it will look like this:
   
   ![image3](3.png)

4. Click on the Action and Send to Repeater. In the bottom of HTTP Request, you will see the email in JSON format. Add ```"roleid":2``` after the email.
   
   ![image4](4.png)

5. Click **Send** and the roleid will change to 2.
   
   ![image5](5.png)

6. Back to the Browser, you will see the Admin Panel. Click on the Admin Panel.
   
   ![image6](6.png)

7. Delete user with name Carlos and the Lab will Solved.
   
   ![image7](7.png)