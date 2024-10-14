How to Run:
Open PowerShell as Administrator.
Copy and paste the script into the PowerShell window.
Press Enter to run it.
This script will:

Check for the cache directories for Chrome and Firefox.
If found, it will delete the cache files for both.
If the directories don’t exist, it will notify you.
Make sure to run this script with administrator privileges to avoid permission issues.

Description of the PowerShell Script:

This PowerShell script is designed to clear the browser cache for **Google Chrome** and **Mozilla Firefox** on a Windows PC. It does the following:

1. **Clear Chrome Cache:**
   - It identifies the cache folder for Google Chrome located at:
     - `C:\Users\<YourUserName>\AppData\Local\Google\Chrome\User Data\Default\Cache`
   - If the cache folder exists, the script will delete all files and subfolders inside the `Cache` directory.
   - If the cache folder does not exist, the script will inform you that the cache path was not found.

2. **Clear Firefox Cache:**
   - It looks for the cache directory for Mozilla Firefox, which is located within Firefox profiles at:
     - `C:\Users\<YourUserName>\AppData\Roaming\Mozilla\Firefox\Profiles`
   - The script loops through all user profiles and deletes the cache files from the `cache2` folder for each profile it finds.
   - If the cache directory for a profile does not exist, it will notify you that no cache was found for that profile.
   - If no Firefox profiles exist, it will inform you that the Firefox cache path was not found.

Key Points:
- The script targets **Chrome** and **Firefox** but can be adapted to other browsers or paths by modifying the folder paths.
- It does not clear browser history or cookies, only cached files (temporary internet files).
- **Administrator privileges** are recommended when running the script to avoid any permission issues when deleting files.
  
This is a quick way to free up space and potentially resolve issues caused by old cache files for these browsers.
