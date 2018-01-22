# google-proxy
Create a Free Proxy Server with Google App Engine

Go to appengine.google.com and sign-in using your Google Account.
Click the “Create an Application” button. Since this is your first time, Google will send a verification code via SMS to your mobile phone number. Type the code and you’re all set to create apps with Google App Engine.
Pick an Application Identifier and it becomes the sub-domain* of your proxy server. Give your app a title (say Proxy Server), set the Authentication Option as “Open to all users”, agree to the terms and create the application. (screenshot)
OK, now that we have reserved the APP ID, it’s time to create and upload the proxy server application to Google App Engine. Go to python.org, download the 2.7 Installer and install Python. If you are on Mac, Python 2.7 is already installed on your computer.
Download this zip file and extract it to your desktop. The zip file contains a couple of HTML, YAML and Python (.py) files that you can view inside WordPad.
Go to code.google.com, download the Google App Engine SDK for Python and follow the wizard to install the SDK on your computer. When the installation wizard has finished, click the “Run Launcher” button to open the App Engine Program.
Choose Edit -> Preferences inside the Google App Engine Launcher program from the desktop and set the correct values (see screenshot) for the Python Path, App Engine SDK and the Text Editor (set this is as WordPad or write.exe and not notepad.exe).
Click File – > Add Existing Application under the Google App Launcher program and browse to the folder that contain the index.yaml and other files that you extracted in Step 5. Once the project is added to App Engine, select the project and click Edit to replace “YOUR_APP_ID” with your App ID (screenshot). Save and close the file.
Click Deploy, enter you Google account credentials and, within a minute or two, your online proxy server will be deployed and become ready for use (screenshot). The public URL (or web address) of your new proxy server will be your_app_id.appspot.com (replace your_app_id with your App Engine Identifier).
[*] The sub-domain or the App ID will uniquely identify your App Engine application. For this example, we’ll use labnol-proxy-server as the Application Identifier though you are free to choose any other unique name.

Next Steps – Setting up a Free Proxy with Google
You can edit the main.html file to change the appearance of your proxy website. You can even add code for Google Analytics and Google AdSense code to monetize your proxy server.

The proxy server is public on the web (open to everyone) but you can add a layer of authentication so that only Google Account users who are logged-in can use your proxy server.

If you have made any changes to your HTML files, you can upload the latest version to Google App Engine either by clicking the “Deploy” button again or use the following command – appcfg.py update <app-directory>

This proxy works with Flash videos (like YouTube and ABC News) though not with Hulu.
As some of you have suggested, web domains with the word “proxy” or “proxies” are banned at workplaces so you may avoid using them in your appspot.com proxy address.
Though there exist proxy servers for accessing secure (https) sites, this is a basic proxy server that won’t work with sites that require logins (like Gmail).
The proxy server code is available on Github and is fork of the Mirrorr project.
