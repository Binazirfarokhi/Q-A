# Q-A
what is library and framework?
a "library" is a collection of pre-written code that provides specific functions for developers to use in their applications, while a "framework" is a structured set of code that defines the overall architecture of an application, dictating how the code should be organized and providing a foundation for building upon, essentially controlling the flow of the program rather than just offering individual tools; library is a pre build code that you just use , but in framework there are some part that you have to optimzie to make that code work on your project. 
=========================================================
What is value proposition: why are you different from other works or other person around you? 
what is metric in lean canvas? metrics are numbers, for instance hoe many customers are getting back to you.

=====================================================
Fire base authentication error: 
🚨 "Access to script at 'Log-in.html' has been blocked by CORS policy: Cross-origin requests are only supported for protocol schemes: chrome, chrome-extension, chrome-untrusted, data, http, https, isolated-app."

this is becasue: 
Why is this happening?
Your HTML file is being opened from file:// protocol instead of a local server (e.g., http://localhost).
Browsers block cross-origin requests from file:// for security reasons.
Firebase Authentication requires requests to come from a proper web server.
Solution: Run a Local Server
Instead of opening the HTML file directly, start a local development server:
cross-origin requests are not acceptable for Fire-base Authenctication.

**Using VS Code Live Server Extension (Easiest)
Open the project in VS Code.
Install the Live Server extension (if not already installed).
Right-click on index.html or login.html and select "Open with Live Server."
This will start a local server (e.g., http://127.0.0.1:5500 or http://localhost:5500).
Try logging in again.**
** 
===================================
.env File Still Pushed to GitHub Despite .gitignore
Why is this happening?
If the .env file was added to Git before adding it to .gitignore, it will still be tracked.
Solution: Remove the .env File from Git History
Remove the file from tracking (but keep it locally):
git rm --cached .env

===================================

Commit the change:
git commit -m "Removed .env from tracking"
Push the changes to GitHub:
git push origin yourNameBranch
Now, the .env file should no longer be pushed to GitHub.
====================================
What is .gitignore ?
.gitignore is a special file used in Git to tell Git which files/folders should not be tracked or uploaded to GitHub.
Why do we need .gitignore?
Some files should not be shared in a repository, like:
Secret keys (.env files)
Node modules (node_modules/ folder)
Log files (.log files)
===========================
3️⃣ What is .env ?
.env (environment file) is used to store secret keys and configuration settings.
Instead of hardcoding API keys in your code, you store them in a .env file.
Why use .env?
Security: Keeps secrets out of your public code.
Flexibility: Allows different settings for development and production.========
===========================
📌 Summary
Term	Meaning
Cross-Origin Request (CORS)	Browser security rule that blocks requests between different origins (e.g., file:// to http://).
.gitignore	A Git file that tells Git not to track certain files (e.g., .env, node_modules).
.env	A file that stores secret keys and settings outside of the public code.
==============
+========================================
how to add a bulk email to our campaing: 
https://support.microsoft.com/en-us/office/use-mail-merge-in-word-to-send-bulk-email-messages-0f123521-20ce-4aa8-8b62-ac211dedefa4#BulkMail=macOS


=====
what is webappmanifest " ? there are five essentials that we need to add to this file. shortname , start_URL , icons : which is array of object , display. 

========
event.keycode : which key was pressed  on the keyboard
event.x
event.y y loc axis of your cursor 

========================
toFixed() ; will just show how many digit after the decimal you want to go.

=======
to see how many recursively item are in a file or folders: 
right click on folder : 
servoces --> open terminal on that folder = run this command : ls -al -R
will show how many elements are inside it?
===================
different between Session storage and local storage?
Both Session Storage and Local Storage are part of the Web Storage API, allowing web applications to store data in a user's browser. 
 data will be cleared when the page ends. 
but for local sotrage which will be your browser Data persists even after closing the browser or restarting the computer.
When to Use Which?
Use Session Storage for temporary data that should disappear after a user leaves the page (e.g., a shopping cart that resets on closing the tab).
Use Local Storage for long-term storage needs, such as saving user preferences, themes, or cached data.
==========
WOrdpress : 
Can I delete the "Create Block Theme" plugin after creating a theme, while keeping others like MetaSlider, ACF, CPT UI, Kadence Blocks, and UpdraftPlus, since their functionality depends on the plugin?

Answer:
Yes, you can safely delete the Create Block Theme plugin after generating a theme, as the theme becomes independent. However, the other plugins (MetaSlider, ACF, CPT UI, Kadence Blocks, UpdraftPlus) must remain active for their features to work properly.
=====
plesk issue: 

If your Plesk account goes over quota, let me know and I'll unsuspend it.

However, if it stays over quota, the system will automatically suspend it again by the next morning. Before that happens, you'd need to login into Plesk and figure out what's causing the site to go over quota.

Possible reasons could include:

Making Duplicator backups of the site. After downloading a Duplicator backup, delete the package. If you go over while making the Duplicator package, the account isn't suspended immediately, so you can just make it, download it, then delete it.
Setting your cloud backup to backup to the server. Make sure that it's set to Dropbox, Google Drive, etc
Having too many plugins or themes. Delete ones that aren't being used.
Having too-large images. Images from Unsplash can be 5 or 6 MB when downloaded. Make sure to size them down. 
Having old sites (like the Deployed Site exercise). Delete old ones from the Plesk control panel. 


