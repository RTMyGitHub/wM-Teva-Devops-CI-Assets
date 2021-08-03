# sagdevops-ci-assets
Software AG DevOps library to support assets CI (continuous integration) with webMethods 9.x and 10.0. Works together with [webMethods sample project layout](https://github.com/SoftwareAG/webmethods-sample-project-layout)


## Description
sagdevops-ci-assets is a library that easily enables CI for your webMethods projects. You can setup your infrastructure in minutes and then deploy flowlessly on your test service while also checking the quality
by running all tests uploaded your version control.


## Set-up

### webMethods Installation
Prepare your webMethods installation - your build server can contain only a plain IntegrationServer with Deployer. Keep the server plain - there is no need for designer or database connection.
Your test server can be more complex as CI will execute unit and integration tests against it. The build and the test server must reach each other over http so that the deployment and the testing can be performed.

### CI Library
Download the library on your build server by

```
git clone https://github.com/SoftwareAG/sagdevops-ci-assets.git
```

Edit the _System.properties_ to correspond to your inftrastucture - deployerHost is the machine where your Deployer is running(normally the build server) where targetHost is your test server - where the packages will be deployed and tested. 

*Notice* change the path the Deployer if you're not using the _default_ Integration Server instance.