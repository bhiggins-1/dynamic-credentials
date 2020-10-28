# dynamic-credential-injection
  This Mule app showcases the ability to use the Salesforce Connector, Netsuite Connector or make an HTTP Request and pass in the Application credentials with the initial request.

 Typically, when building a Mule application and configuring the connectivity to an application, you will store the credentials to connect to that application inside the Mule Application. What if you want to inject the credentials at runtime?  Read on to find out how and why you may want to take this approach.

 There are a few benefits to this approach. 1) This approach could be used to build a multitenant application that connects to N number of accounts as the credentials are passed in the API request. 2) Passing in the credentials at runtime keeps the credentials from being stored in the app in case the credentials frequently change.

 However, one drawback of this approach, is that the Mule Application is not able to read the metadata of the external system because the credentials are not saved to the Mule application.  Keep this in mind if you are thinking of going down this route.
