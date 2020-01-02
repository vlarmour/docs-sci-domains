---
title: 'Error Logs'
taxonomy:
    category:
        - docs
visible: true
---

## Symptoms
* Blank page
* Page Not Found / HTTP Error 500
* Internal Server Error

## Resolution
Check the error logs via the cPanel and the File Manager to locate where the error is occurring.  

**cPanel Error Log**
1. Start with the cPanel error log since it requires minimal digging. Go into your cPanel account > in the Metrics section > Errors. This log will bring up an error that lists the most recent webserver error logs. A common error is (relevant content in bold):

[06-Dec-2019 17:04:08 UTC] PHP Warning: require_once **(login_fernando.php)** : failed to open stream: **No such file or directory in** /home/va226/public_html/**6_insertProcess.php on line 3**

Basically the error log is saying that it cannot find the file “login_fernando” so it cannot execute the script in the file 6_insertProcess.php on line 3.

**File Manager**
1. Check the File Manager error logs. 
2. You will first go to cPanel > File Manager > public_html > there will usually be an error log here. 
3. Then, use the search feature in File Manager to look at all of the error logs. This looks like cPanel > File Manager > search 'error_log' in the search bar and look through each error log for the most recent errors. For example, a common error found through the File Manager are errors in syntax (relevant content highlighted below):

[04-Dec-2019 04:47:53 UTC] PHP Parse error: **syntax error, unexpected ‘<’ in** /home/va226/public_html/550/exercise5/**Exercise5showResults.php on line 188**

The above error indicates a syntax error on line 188 of the file Exercise5showResults.php.

Your error reports will be similar but will provide specific information on the files that you have uploaded. 