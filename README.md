# Salesforce.com Mobile SDK Shared Repository for JavaScript Artifacts
This repository contains JavaScript artifacts that are shared between the different Salesforce Mobile SDK repositories. 
For more information, please check out the [Salesforce Mobile SDK for Android](https://github.com/forcedotcom/SalesforceMobileSDK-Android/), or the [Salesforce Mobile SDK for iOS](https://github.com/forcedotcom/SalesforceMobileSDK-iOS).

# /libs
==

Contains all the SalesforceMobileSDK JavaScript libraries.

**cordova.force.js**

Contains all the Cordova plugins for the SalesforceMobileSDK (oauth / smartstore / sdkinfo).
Includes this library after cordova.js in your HTML application.

**forcetk.js**

Library to do REST API calls from JavaScript.

**force.entity.js**

Contains the new SDK 2.0 Entity Framework. 
This library depends on forcetk.js and cordova.force.js. It also requires jquery, underscore and backbone.


# /external
==

Contains all the external libraries used in sample apps or required by some of the libraries above:

** backbone **

Contains backbone and underscore.

** jquery **

Contains jquery and jquery mobile.
Required by entiy framework and used in some of the sample apps.

** qunit ** 

Contains qunit. A unit test library for JavaScript.


# /SampleApps
==

Contains all the SalesforceMobileSDK JavaScript sample applications.

**entity**

Contains sample applications demonstrating the use of the new SDK 2.0 Entity Framework:
* UserAndGroupSearch.html: simplest sample app with a single search/list screen that allows searching for users or collaboration groups
* UserSearch.html: another sample app that allows searching for users and has a basic user detail screen to the search/list screen
* AccountEditor.html: most advanced sample app that allows searching for accounts, editing their details, creating new accounts or deleting existing accounts. It also works offline and detects conflicts when records have changed on the server.

**contactexplorer**

HTML/CSS/JavaScript used by ContactExplorer application.

**sfdcaccounts**

HTML/CSS/JavaScript used by SFDCAccounts application.

**smartstoreexplorer**

HTML/CSS/JavaScript used by SmartStore Explorer application.

**vfconnector**

Contains bootconfig.json for VF Connector application.

# /test
==

Contains all the tests for the SalesforceMobileSDK JavaScript libraries.

**test.html**

HTML page to run the tests outside the container.

**MockCordova.js, MockSDKInfo.js, MockSmartStore.js**

Libraries used to mock the container when running tests directly in a browser.

**SFTestSuite.js, SFAbstractSmartStoreTestSuite.js**

Super class of test suites.

**SFSmartStoreTestSuite.js, SFLSmartStoreLoadTestSuite.js**

Test suites for SmartStore.

**ForceEntityTestSuite.js**

Test suite for the new SDK 2.0 Entity Framework.
