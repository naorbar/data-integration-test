# data-integration-test

## Overview
Webpals is looking for an industrial/software/system engineer to be responsible on migrating their exiting CRM solution to Salesforce, and later take ownership on maintaining and implementing new use cases according to the business needs.
This test checks how the candidate can:
 - Understand and follow business requirements
 - Learn quickly new material and tools, such as Data Integration, Database installation and REST interface
 - Work under preasure with a tight schedule
 - Communicate with co-workers
 
## Follow the next steps carefully:
The purpose of the test is to implement a utility which imports data from a remote server, i.e. XXX, transforms the data and export it to a local database (e.g. MySQL).
The utility will be implemented with [PDI](https://www.hitachivantara.com/en-us/products/big-data-integration-analytics/pentaho-data-integration.html) (aka Pentaho Data Integration tool)

1. Use this [link](https://sourceforge.net/projects/pentaho/files/latest/download?aliId=137249511) to download and install [PDI tool](https://community.hitachivantara.com/docs/DOC-1009855-data-integration-kettle) (community edition)
2. Use this [link](https://dev.mysql.com/downloads/windows/installer/8.0.html) to download and install MySQL database (community edition)
3. Open the PDI designer and create a new Transformation (ktr file) 
4. Implement a flow based on the following use case:
    1. the user gets a list of accounts from...
    2. the user transforms the data and export it to a local database (e.g. MySQL)

## Additional Requirements:
Follow the next steps to allow PDI to connect with your MySQL database:
 - Get MySQL JDBC driver from [here](https://dev.mysql.com/downloads/connector/j/) 
 - Take the following jar file: mysql-connector-java-8.0.16.jar from the package you just downloaded and put it in PDI lib folder (e.g. pdi-ce-8.2.0.0-342\data-integration\lib)
 - Restart PDI to have it load the jdbc driver (jar file)
 - Set the db connection step (i.e. Table Input or Table Output) with a Generic Connection as shown here:
 <img src="./images/PDI_HowToConfigureDatabaseConnection.PNG" alt="PDI_HowToConfigureDatabaseConnection.PNG" width="50%" height="50%"/>

1. The test should take ~3 hours to complete; though the completeness of the task should take precedence over the time limitation.
2. Please submit the solution (ktr script) via email to: naor.b@webpals.com 

**Goodluck** :+1:
