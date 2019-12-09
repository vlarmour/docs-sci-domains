---
title: 'File Structures and the File Manager'
taxonomy:
    category:
        - docs
visible: true
---

Web hosting is, at its basic core, files and folders on a computer that is connected to the internet and setup to distribute them. How that computer (typically a server) is set up to do that is covered more in [LAMP Environments]() but this article will explain the idea of the file structure and how it relates to what you view on your domain.

When you signed up for your domain, a web hosting account was created. Although you typically will interact mostly with the web interface to create subdomains, install applications, and other common tasks, you might occasionally also need to work directly with the files in your account. The **File Manager** in your cPanel is one way to see these files. You can also create an FTP account in cPanel and use an FTP program to interact with these files (FTP stands for File Transfer Protocol, and it’s a way of using a desktop client to transfer files to and from your Web server space).

Let’s take a look at the **File Manager** built into your cPanel to get a better understanding of the file structure that makes up your website(s).
1. Login to cPanel at rutgers-sci.domains with your RU Net ID and password.
2. On the homepage of your control panel, you’ll have all the various tools listed. You can easily find the File Manager by using the search tool in the upper righthand corner and typing File Manager. You can also find its icon under **Files**.
3. You are now sent to the File Manager and can navigate the folder structure there.

You’ll notice when the File Manager opens up that this looks very much like a folder on your computer. There are a few folders in it as well as files, and you can navigate down into those folders and see what’s inside of them. At the top level of the File Manager, you also have the option of interacting with files and folders you select by moving them around or removing them. There is a larger article all about how to use the file manager at [Accessing Your Files through the File Manager]() so we won’t talk much about how the interface works here. Instead, we’ll cover what those folders and files actually mean and how they relate to what someone sees when they visit your website.

By default, you have a variety of folders at the root of your web space (the first screen you see when you open up the file manager). Some of them are created automatically to store information about the panel and setup of certain sites. These folders are things like access-logs, etc, ssl, and tmp. You can safely ignore most of those folders because they don’t correspond to actual websites. Let’s look at which folders do and how it all works.

Your main domain will correspond with a folder called **public_html**. Whatever files and folders are inside of this folder are available on that main domain. If you installed WordPress here you’ll likely see a lot of WordPress-related files within it (which were probably helpfully put there by the automated installer). Let’s say we uploaded an image called mypicture.jpg directly into the public_html folder. That image would now be available at yourdomain.com/mypicture.jpg. The slash after your domain implies “this file is inside this folder”. But what if we had a folder inside the public_html folder? How does that appear? This is typically called a subfolder so let’s put a folder in public_html called “images” and put our image, mypicture.jpg, inside of that folder. What would you type in a browser to get to that file now? The location would be mydomain.com/images/mypicture.jpg. So subfolders are also indicated by a forward slash after a domain.

**What about subdomains?** You can have completely separate sites called subdomains that appear as nameofsubdomain.yourdomain.com. But where are they in the file structure? When you create a subdomain, cPanel will ask you to give the subdomain directory a name. If I had a subdomain called photos.mydomain.com for example, I might want to name the folder “photos” (by default your control panel will call the folder by the name of the subdomain). Folders for subdomains are located inside the public_html folder. So when you go to the File Manager and navigate to public_html, you’ll see folders listed for all of your subdomains and once you navigate inside one of those folders, you’ll see files and folders specifically for that subdomain that appear on the web at that subdomain’s address.

File Manager in cPanel is great to view these files and folders, but it can be limiting if you want to upload an entire folder of information to your website. If you find yourself wanting to do more with the files and folders on your web space you may want to consider using File Transfer Protocol (FTP). FTP will allow you to upload and download files to and from your File Manager (i.e. your website) in bulk. 