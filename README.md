mobilegame
==========


Installing ionic etc so that you can run the simulation
=======================================================

1. Install node.js
2. install ionic and cordova - $ npm install -g cordova ionic
3. Install Bower - $ npm install -g bower
4. install ngCordova - $ bower install ngCordova
5. Install virtualbox
6. Install genymotion - you will need a geny motion account (free) so you can pull down a virtual device (i choose a galaxy s5)
7. Install the android SDK 
8. Set your path to include the andorid tools and platform tools (mine ws export PATH=${PATH}:/Developer/SDKs/android-sdk-macosx/platform-tools:/Developer/SDKs/android-sdk-macosx/tools)
9. If you dont have platform tools in your sdk run android from the comand line and download the tools plus android 4.4.2 (api 19) - then of course add them to your path
10. After that you will probably need to install apache ant.... i did this using brew (mac only) not yet done this on mint, but i expect there will be a package for it. 


Getting the repo
================

1. first you will need to create your ssh keys this article explains everything: https://help.github.com/articles/generating-ssh-keys/
2. create a new directory /var/www/mobilegame
2. CD into the directory and run $ git init
3. The add the remote git account $ git remote add origin git@github.com:robcollyer/mobilegame.git
4. Finally get the repo running $ git pull origin master

Running the sim 
===============
1. CD into the mobilegame directory
2. On mint you will need to run $ inonic platform add android
3. Start geny motion and run the virtual device
4. When this has loaded iin the terminal run $ ionic run android

ALl should be good and the app should appear in the virtual device








