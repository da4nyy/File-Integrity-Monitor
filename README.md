# File-Integrity-Monitor

This is a script developed to be used in CTF. 
 

## Utility 
The script recursively scan the given directory tree . Then, it will log any file changes (every 4 seconds by default ) including;

- Modified files
- Removed files
- Added files

![image](https://user-images.githubusercontent.com/117517618/202917616-d6bb3e36-b20f-4125-b851-627316a37a2e.png)

## Use Cases

+ You may monitor the integrity of the files that may have PII. In this case, you can place the script where your files live, and create a crontab or use task scheduler to run the script.
+ You can use the script to monitor the files stored in the web app.
+ If you are in the Blue Team at a CCDC competition, you can use this script to monitor your server and easily see which files modified.
#### Libraries Used

- os
- pickle 
- datetime
- hashlib	
- logging
- time 
- signal
- dictdiffer 
- progress
