######################### Naukri Profile Update Automation #############################

This script automates the process of updating your Naukri.com profile to keep it active.

## Setup Instructions
=== Install Python requirements:
   ```
   pip install -r requirements.txt
   ```
=== Install Chrome WebDriver:
   - Download ChromeDriver that matches your Chrome browser version
   - Add it to your system PATH
=== Update credentials:
   - Edit `credentials.json` with your Naukri.com login details
=== Run the following command to install the required Python libraries:
"pip install selenium webdriver-manager pyautogui"


##Install Chrome WebDriver:
=== The script uses webdriver-manager to automatically manage the ChromeDriver version matching your Chrome browser.
=== Ensure you have Google Chrome installed on your system.

##Update Credentials:
=== Edit the credentials.json file with your Naukri.com login details in the following format:
{ 
"email": "your-email@example.com",
 "password": "your-password"
}

##Usage
=== Run the script using the following command:
```
python naukri_automation.py
```


##Features
=== Automated Login: Automatically logs into your Naukri.com account.
=== Resume Upload: Uploads a new resume file to keep your profile updated.
=== Download Updated Resume: Downloads the updated resume for backup.
=== Screenshots: Captures screenshots during critical steps, such as file upload, for debugging.
=== Error Handling: Handles login errors, resume upload errors, and unexpected issues gracefully.
=== Cleanup: Ensures the browser closes after execution.



##Notes
=== The file paths (e.g., for the resume and screenshots) can be configured directly in the script.
=== Ensure the XPath selectors in the script are updated if Naukri.com changes its layout or structure.

##Security Note
=== Keep your credentials.json file secure and never share it publicly.
=== Avoid hardcoding sensitive information directly into the script.

##Troubleshooting
ChromeDriver Version Errors:
--------------------------- Update your Chrome browser or run:
----------------------------pip install --upgrade webdriver-manager
##Element Not Found:
-------------------------- If elements cannot be found, check if the XPath selectors are correct.
-------------------------- Adjust waiting times in the script if the page takes longer to load.
##File Upload Issues:
-------------------------- Ensure the file path to your resume is correct and accessible.

##Future Improvements
===will Add support for other browsers (e.g., Firefox, Edge).
===Implement CLI arguments for flexibility (e.g., specifying the resume file path).


##License
===This project is free to use under the MIT License.
