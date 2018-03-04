# Task Runners 103:

As a continuation from the 2nd task runner tutorial, in this session we are going to be using live reload to see the changes to our code as soon as we make the changes without refreshing the browser.

# TR-103 dev directory structure as follows:
Project Folder(TR-103)

tr-103/

   |- dev/

       |- index.html
   
       |- js/
   
           |- main.js
      
           |- jquery-3.3.1.min.js
      
gulpfile.js

README.md

package.json

package-lock.json

server.js

*** ">>" means run this from the command terminal without the ">>" ***

# Some introduction
Install NODE.JS:
-- Install Node:
http://nodejs.org

--Open a command prompt and navigate to your project directory.

--NPM and gulp should already be installed from the previous session but if you started a new project do not worry. The commands with install and load all you need.

--We are adding 1 new plug-ins for this one.

--The gulp-livereload is the plugin to refresh the browser when code changes are made.

# Install
Here are all of the commands to run(once Node is installed):

(Open a command prompt and navigate to the project directory)

********************** Command to install npm **********************
>>npm install

********************** Single line command to install all plugins ***************
>>npm install gulp gulp-htmlclean gulp-clean-css gulp-concat gulp-uglify run-sequence gulp-bump del gulp-remove-empty-lines gulp-clean gulp-js-obfuscator gulp-livereload gulp-strip-code static-server --save-dev


# Run
**********************Run the following command in the terminal***************
>>gulp watch


--Launch index.html in a browser

-- Open a file from the dev, dev/css & dev/js directories in an editor make a change and save it, the browser will reflect and render changes.

>>ctrl + c   

& y for yes to stop livereload server and run any other gulp command. (gulp stagetest or gulp stageprod)

>> gulp stagetest

-- Open index.html in the test directory in an editor you will see the live reload script at the bottom is now gone along with the comments and blanklines.
-- Open the test/js/main.js in an editor to verify that the contents are obfuscated.
************************************************
####Extra npm commands:
-Remove unused packages from the directory to keep things lean.

>>npm prune

************************************************
Part I: (HTML File clean-up)

https://github.com/mstatt/tr-101

Part II: (Javascript Obfuscation)

https://github.com/mstatt/tr-102

************************************************
Helpful Link:
https://gist.github.com/renarsvilnis/ab8581049a3efe4d03d8
