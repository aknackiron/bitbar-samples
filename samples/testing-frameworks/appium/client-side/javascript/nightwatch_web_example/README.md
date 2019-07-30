# Nightwatch Example

## Client Side Test Execution
### Setup
* Install Gulp

	```
	$ npm install -g gulp
	```

* Install NPM Dependencies

	```
	$ npm install
	```
    
* Add your apiKey to ./.credentials.json

   Create a file called ".credentials.json" in the project's root and add your Bitbar apiKey to it as described below:
	
	    {
	        "apiKey": "YOUR_BITBAR_CLOUD_APIKEY"
	    }


* Modify the nightwatch.json-file according to your project

### Run the test 

* To run the test on iOS

	```
	$ gulp ios
	```

* To run the test on Android
	
	```
	$ gulp android
	```

## Server Side Test Execution
### Setup
* Create a zip file to be uploaded to Bitbar

	* If you have Gulp installed, run the following command at the project's root folder:
		
		```
		$ gulp zip
		```
		This creates a zip-file of the project to the "dist"-folder.
	* Zip the project manually

### Run the test
On Bitbar cloud

* Create an Appium server side project
* Create a new testrun in new server side project
* Upload tested application (apk/ipa) through the “Application” step
	* When doing web-testing as in this example, you can upload any application as it will not be used. You can, for example, download an application from here :
	https://github.com/bitbar/bitbar-samples/tree/master/apps/builds
* Upload the zip with scripts through the “Upload test file” step
* Choose device group to use or create a new group for this run
* Start testrun



