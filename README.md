# getting started with node.js and express to create a static (local) server on a mac using terminal


## prerequisites
1. Download and install [Node.js](http://nodejs.org/ "Download Node.js")
2. Decide on a folder to have your static server in
2. Make sure that there is a file in that folder called _"package.json"_ if it is not there create it and include the following lines in the body:

		{
  		"name" : "ServeStaticContent",
  		"version" : "0.0.1",
  		"dependencies" : {
    			"express" : "3.x"
  		}
		}

3. In that same folder have a file called _server.js_ that includes the following:
		var express = require('express');
		var app = express();

		//public is the actual folder of the website or app
		app.use(express.static(__dirname + '/public'));
		
		//you can change the port to anything above '3000'
		app.listen(process.env.PORT || 3000); 


## Steps first install
1. Open terminal
2. Go to the right directory (cd "name directory") 
3. Create a folder called "public" by typing _"mkdir public"_
4. In terminal you need to install **Express** in order to use it by typing _"npm install -g express"_ ( NB make sure you are not in node!!)
	a. if this does not work due to admin issues, use _"sudo npm install -g express"_ this will ask for credentials (password)
5. Install dash _"npm install dash"_
6. Execute the _server.js_ file by typing _"node server.js"_
7. In your browser type: "localhost:3000" // or whatever you used as a number


## Returning to the local server
1. Open terminal
2. Go to the right directory (cd "name directory") 
3. Execute the _server.js_ file by typing _"node server.js"_
4. In your browser type: "localhost:3000" // or whatever you used as a number


### Glossary

**mkdir** stands for make directory

**-g** stands for global so the item is available anywhere 

**Install** command to install packages in terminal

**NPM** (Node Package Manager, is two things: it is an online repository for the publishing of open-source Node.js projects; second, it is a command-line utility for interacting with said repository that aids in package installation, version management, and dependency management.) 

**Terminal** 
