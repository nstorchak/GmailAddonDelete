# A Delete Email Add-on For Gmail
A Gmail Add-on that deletes the currently open email at the press of a button

### Prerequisites
a Gmail account

### Getting Started
- Download the contained files.
  All the .txt files are actually .gs files, but only Google Scripts understands this format. 
  You can see the code in the TXT version.
- Deploy the add-on on your gmail account as written in the article, but using my files:
  https://developers.google.com/gmail/add-ons/guides/quickstart  
  Note that you will need to create 2 script files (to match the 2 in this project)

### Additional Instructions
- After creating the script files and updating the manifest, deploy the addon to your gmail as listed in google's documentation above
- You should see a fish icon on the right of your screen, click that icon and a card will open
- Click on an email you'd like to delete and a button will appear inside the addon
- Press the "Move To Trash" button on the add-on and press the back button on the email you had open
- The email you just viewed will be moved to Trash

### Authors
Nicole Storchak

### Acknowledgments
Martin Berube for making the fish icon
