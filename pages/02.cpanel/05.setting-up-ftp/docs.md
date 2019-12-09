---
title: 'Setting Up FTP'
taxonomy:
    category:
        - docs
visible: true
---

There may be times when you need to upload files to your website in the Rutgers SC&I web hosting environment. There are a number of scenarios when this might be necessary:
* You’re working with an application that allows you to install plugins/extensions, but the files need to be manually added to your file manager in order to install them. (Note: This is not required for WordPress which allows you to install themes/plugins through the WordPress dashboard.)
* You’ve developed a custom site/pages using a Web design program, and you need to upload the files you created to your file manager
* You’re installing an application that isn’t part of the applications list in Installatron.

One way to upload files is by using the File Manager that is part of cPanel. However, sometimes you’ll find it easier/necessary to use File Transfer Protocol (FTP) to move files to your site. This can be particularly useful if you’re working with a Web space where you’re not the owner (so you don’t have access to the File Manager in cPanel) or if you need to provide file access to someone else to your space on the Web server. File Manager also only allows you to upload files one by one, so if you’re working with large amounts of data then FTP will be preferable.

## What exactly is FTP?
File Transfer Protocol is a method that allows you to remotely move files to a Web server from another location – usually your local/personal computer. Using a pre-defined FTP account (with a username and password), you can configure an FTP client (a program you run on your computer that allows you to transfer files via FTP.

There are lots of FTP clients that you can use; some are free and some are not. A few free ones you might consider:
* [FileZilla (Mac & PC)](https://filezilla-project.org/)
* [CyberDuck (Mac & PC)](http://cyberduck.io/)

For the purpose of this tutorial, we’ll show you how to set up FTP in FileZilla, ([Cyberduck instructions](https://community.reclaimhosting.com/t/ftp-file-transfer-protocol/304) for your reference) but you should be able to generalize these instructions to use in any FTP client.

## Get Information about Your FTP Account
If you’re connecting via FTP to your own space on Rutgers SC&I, or if you’re setting up an FTP account for someone else to use, you’ll need to start by getting the proper FTP credentials from cPanel:
1. Login to rutgers-sci.domains with your RU Net ID and password.
2. In the **Search Box** at the top of the page, search for “FTP”, and click the **FTP Accounts** icon that appears.
3. Every cPanel has an FTP account by default, and you can find those credentials by scrolling down on the FTP Accounts page. You also have the option to create a new FTP account, which can be done by filling out the **Add FTP Account** form with a username and password. Unless you change it, the new FTP account will be limited to a directory with the same name as the account you’re creating. You can change this to a different directory, if you want to grant this account access to a different location.  **NOTE: Make sure you know/remember the password you enter.** When you’re done, click **Create FTP Account**.
4. Once you’ve created the new account, you’ll see it appear in the list at the bottom of the FTP Accounts page. In addition to any accounts you’ve created, in the Special FTP Accounts section, you’ll see the default FTP Account. You’ll know this account because the username corresponds to your cPanel username. This FTP account has full privileges to access all directories within your cPanel.
5. For whichever account you need credentials for, click the **Configure FTP Client** link. 
6. Write down the username, server, and port information that appears. You will need to use this (or you will need to provide this to the person you are giving FTP access) along with the password you created in Step 3 in order to configure your FTP client.

### Please Note
For cPanel’s default FTP account, use the following settings:
* Connect via **SFTP** (more secure than FTP)
* Port: **22**
For an FTP account that you manually created (shown in Step 3 above), use the following settings:
* Connect via **FTP** (cPanel doesn’t allow an SFTP connection for manual accounts)
* Port: **21**

Permissions Settings:
* 644 / all files
* 755 / all folders

## Configure FTP in Your FTP Client


Below are links to tutorials for setting up both FileZilla and CyberDuck to connect to your FTP account.
* [FileZilla Configuration Instructions](http://www.siteground.com/tutorials/filezilla/filezilla_management.htm)
* [CyberDuck Configuration Instructions](https://trac.cyberduck.io/wiki/help/en/howto/ftp)
