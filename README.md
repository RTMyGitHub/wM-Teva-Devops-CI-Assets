# wm-Teva-Devops-CI-Assets
This is the repo/module that supports the continuous integration activity for Teva.


## Description
wm-Teva-Devops-CI-Assets is a library that easily enables CI for your webMethods projects. You can setup your infrastructure in minutes and then deploy flowlessly on your test service while also checking the quality by running all tests uploaded your version control.


## Set-up

### webMethods Installation
Prepare your webMethods installation - your build server can contain only a plain IntegrationServer with Deployer. Keep the server plain - there is no need for designer or database connection. Your test server can be more complex as CI will execute unit and integration tests against it. The build and the test server must reach each other over http so that the deployment and the testing can be performed.

### CI Library
Download this repo on your build server.

Edit the System.properties - Update the deployer installation location.
Edit the DeployEnv.xml - This file contains the Deployer setup of your env in SAG landscape. 
Edit the TestEnv.xml - This file contains the setup of your webMethods Test server of wherever your test scripts will be executed