# File-Integrity-Monitor

This is a script developed to be used in CTF. 
This code is a Python script for a basic file integrity monitor, which is a tool used to monitor changes to files in a given directory. The script takes two arguments: a directory to scan, and an output file for alerts. The script will recursively scan the given directory and its subdirectories, and will create alerts for any added, removed, or changed files. The script uses the os, sys, and pickle libraries to perform file system operations, as well as the datetime, hashlib, logging, and time libraries for other operations.
 

## Utility 
The script recursively scan the given directory tree . Then, it will log any file changes (every 4 seconds by default ) including;

- Modified files
- Removed files
- Added files

![image](https://user-images.githubusercontent.com/117517618/202917616-d6bb3e36-b20f-4125-b851-627316a37a2e.png)

> This script will generate two log files : **handler.log** and **alert.log** 
## Use Cases

+ You may monitor the integrity of the files that may have PII. In this case, you can place the script where your files live, and create a crontab or use task scheduler to run the script.
+ You can use the script to monitor the files stored in the web app.
+ If you are in the Blue Team at a CCDC competition, you can use this script to monitor your server and easily see which files modified.
#### Libraries Used
> To proceed without any problems you need to install all required libraries 
- os
- pickle 
- datetime
- hashlib	
- logging
- time 
- signal
- dictdiffer 
- progress
