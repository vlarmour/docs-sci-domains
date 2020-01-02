---
title: 'FTP Connection Issues'
taxonomy:
    category:
        - docs
visible: true
---

## Symptoms
* Lost connection to see your files online.
* Error: Critical error: Could not connect to server
* 500 Internal Server Error

## Resolution
Email the SC&I IDTS team at sci-idts@comminfo.rutgers.edu to fix the permissions.  

Please note that our business hours are Monday-Friday 8am-4:30pm Eastern Time. If you're submitting this request within business hours, a SC&I Instructional Designer will be in touch shortly. If you're submitting this request outside of business hours, there will likely be a delay in reply to your ticket.

## Prevention Tips
Permissions Settings:
* 644 / all files
* 755 / all folders

Our Rutgers SC&I hosting environment runs the LINUX operating system and an APACHE Web server.  Apache requires specific permissions to serve content (644 on files, 755 on directories), so anything without the correct permissions is going to break and not be accessible (like uploading files with 755 perms to public_html).

Anything uploaded via FTP to a website root, like public_html, must follow these conventions of 644 for files and 755 for folders. Outside of them, unless it’s required by a specific program, it’s much more flexible. Using 755 is wrong for files since files in places like public_html should be 644, because they do need to be read by other users/programs outside of the user’s group. 