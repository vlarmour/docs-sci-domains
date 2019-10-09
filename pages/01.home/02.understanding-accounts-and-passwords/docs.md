---
title: 'Understanding Accounts & Passwords'
taxonomy:
    category:
        - docs
visible: true
---

One aspect of rutgers-sci.domains that users may find a bit complicated at first is understanding the different accounts (and associated passwords) that you can manage as part of your participation in the project. This article outlines the types of accounts that you are likely to have, what they are for, and how you go about resetting passwords on each of them.

##Your cPanel Account
When you first sign-up for your domain and hosting, a cPanel account will be generated that provides you with access to your slice of the rutgers-sci.domains web server. Your cPanel account is automatically associated with your Rutgers NetID. Therefore, **your Rutgers NetID will grant you access to your cPanel account.**

##Your Application Administrator Accounts
Every time you install a new application in cPanel, an Administrator Account for that application will be created. You will likely use these accounts very often – every time you need to login to your application to manage the associated website, you will use this account.

For example, if you install WordPress to manage your Web site, every time you need to add content to WordPress, change your theme, approve comments, etc. you will use this account to login.

Usually, you will be given the opportunity to choose the username and password for that account. We recommend choosing something that you are likely to remember but that is [strong and secure](https://lifehacker.com/geek-to-live-choose-and-remember-great-passwords-184773).

Upon installation, you will likely receive an email confirming the user-id/password combination you chose. It will also have information about how to access the login page for that application. You may wish to make sure you don’t delete this message.

Depending on the application you’re working with, managing and resetting the password for this account will vary. If you’ve used Installatron (in cPanel) to install the application, however, you can always review the account credentials:
* Login to cPanel through [https://rutgers-sci.domains/dashboard/](https://rutgers-sci.domains/dashboard/)
*  Click the Installatron icon in the Software/Services section.
*  Find the applications you installed under **My Applications**.
*  Click the **Edit** button (this looks like a blue wrench.)
*  Scroll down to find the Administrator Username and Password.

In addition, most applications should have some kind of password reset link on the login page.  Additional information on [resetting your application password through Installatron](https://community.reclaimhosting.com/t/finding-your-wordpress-password/201) is provided by Reclaim Hosting.

##Other Types of Accounts
In addition to the account types outlined above, there are a few other kinds of accounts you may have as part of rutgers-sci.domains:
* When you sign up for netid.rutgers-sci.domains, cPanel will automatically create an **FTP** account for you by default.  You will also have the option of manually creating your own FTP account.  You can learn about the differences in FTP accounts in the section on Setting Up FTP.
* Application User Accounts: In addition to the Administrator Account that you set up when installing an application, most applications will also let you set up user profile accounts within each application.