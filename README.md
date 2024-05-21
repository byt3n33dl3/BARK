### Barking through Bark

![bark](https://github.com/Sulaimannabdul/Barking/assets/151133481/ee400007-4db2-4826-8fd4-78bc8989d572)

BARK stands for BloodHound Attack Research Kit. It is a PowerShell script built to assist the BloodHound Enterprise team with researching and continuously validating abuse primitives. BARK currently focuses on Microsoft's Azure suite of products and services.

BARK requires no third party dependencies. BARK's functions are designed to be as simple and maintainable as possible. Most functions are very simple wrappers for making requests to various REST API endpoints. BARK's basic functions do not even require each other - you can pull almost any BARK function out of BARK and it will work perfectly as a standalone function in your own scripts.

***Barking***  barking is a versatile tool for Bloodhounds, aiding in their effectiveness as trackers and enhancing their ability to communicate with both humans and other dogs.

Meta Functions
--------------
* ``Invoke-ExternalAbuseTest`` performs all abuse validation tests that can be executed by holding an MS Graph app role.
* ``Invoke-AllAzureADAbuseTests`` performs all abuse validation tests that can be executed by principals granted AzureAD admin roles.
* ``ConvertTo-Targets`` is used for massaging output from the Invoke-<type>Tests functions for usage in another platform.

![Apache_Bloodhound-Logo wine](https://github.com/Sulaimannabdul/Barking/assets/151133481/4a71bcaa-f5e8-4e81-bb1b-944d189cfc9d)

#### **Credit to bloodhound and bark repo.**
