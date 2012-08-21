My first backlift app
==================

The fastest way to get up-and-running with backbone.js


steps I did to create this app


## No 1 Set-up the Backlift Command Line Utility

Open up your terminal and download the Backlift Command Line Interface (CLI) by typing:
```
sudo easy_install backlift
```
Alternatively, you can use pip to install the Backlift CLI into a virtual environment.

Once you have backlift installed, setup backlift using your account's API key:

```
backlift setup 8vaW98N5RNKXtaFX 
```
Now you can use the Backlift CLI to communicate with the main backlift website.

From time to time you should make sure that you have the most recent version of the Backlift CLI. You can check that by typing 
```
backlift --version
```
The version string outputted should match the 'Backlift CLI current version' listed in the account details section to the right. If not you can update your Backlift CLI by entering the command 
```
sudo easy_install --upgrade backlift.
```
Now you're ready to create new apps and upload them to backlift.


## No 2 Create and Upload a new app

Create a new app with the command:
```
backlift create:demo backliftapp
```
This will create a new folder in the current directory called 'backliftapp' and begin downloading the backlift demo project. Once the project template has finished downloading, check it out by opening the 'newapp' folder with a text editor.

To see this app running on a public web server, first change directories into the 'backliftapp' folder and type 'backlift push'.
```
cd newapp
backlift push
```
This will upload the content of the 'backliftapp' folder to Backlift. Alternatively you can use the command backlift watch.

The watch command will first upload the 'backlifapp' folder and then wait for changes to the project. Any time you edit and save a file in the 'backliftapp' folder while the watch command is running, your changes will automatically by synced to Backlift.

## No 3 View and manage your app

You can launch a browser to view your app by typing:
```
backlift open
```
You can alternatively view the website's admin page by typing backlift admin.

That's all there is to it! The demo app contains a tutorial that will show you how to build a backbone.js app with Backlift. See you there!

