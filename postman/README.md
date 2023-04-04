Initial Date: August 3, 2020
Initial Author: Tom Baker

Revision Date: March 31, 2023
Revision Author: Tom Baker

================================

MANDATORY ENVIRONMENT SETTINGS

================================

The Core Capture Services - SmokeTest.postman_collection uses the following mandatory environment settings:

host = This should be the base URL for Core Capture Services. For example: https://capture.ot2.opentext.com

clientid = This should be your clientid for your API credentials obtained from Admin Center.

secret = This should be your API credentials secret obtained from Admin Center.

tenantid = This should be used if you are going to go against one of the Developer data centers such as api.opentext.com.

Use Postman's environment settings UI to define these three environment variables.

================================

TEST DEPENDENCIES

================================

The tests should be run from top to bottom. After some requests additional values are stored that are used in subsequent tests. For example, executing the Home request will capture the token URL in which to GetServiceToken will use to perform a credential grant. Another example is the uploading of files after which the file IDs are stored and used in the service calls.

In addition, the tests are also dependent upon the files found in this directory. You can either copy these images to your Postman's working directory or assign your Postman's working directory to where these files are.

