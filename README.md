### BARKING ---> BARK

![bark](https://github.com/Sulaimannabdul/Barking/assets/151133481/ee400007-4db2-4826-8fd4-78bc8989d572)

BARK stands for BloodHound Attack Research Kit. It is a PowerShell script built to assist the BloodHound Enterprise team with researching and continuously validating abuse primitives. BARK currently focuses on Microsoft's Azure suite of products and services.

BARK requires no third party dependencies. BARK's functions are designed to be as simple and maintainable as possible. Most functions are very simple wrappers for making requests to various REST API endpoints. BARK's basic functions do not even require each other - you can pull almost any BARK function out of BARK and it will work perfectly as a standalone function in your own scripts.

***Barking***  barking is a versatile tool for Bloodhounds, aiding in their effectiveness as trackers and enhancing their ability to communicate with both humans and other dogs.

Meta Functions
--------------
* ``Test-AzureRMAddSelfToAzureRMRole`` used in abuse validation testing to determine whether a service principal with certain rights can grant itself the User Access Admin role over a subscription.
* ``Test-AzureRMCreateFunction`` used in abuse validation testing to test if a service principal can add a new function to an existing function app.
* ``Invoke-AllAzureRMAbuseTests`` performs all AzureRM abuse validation tests and outputs a resulting object that describes which AzureRM roles granted the ability to perform each abuse.
* ``Remove-AbuseTestAzureRMRoles`` is a clean-up function for removing AzureRM admin roles created during testing.
* ``Remove-AbuseTestServicePrincipals`` cleans up abuse tests by removing the serivce principals that were created during testing.
* ``New-TestAppReg`` creates an application registration object for the explicit purpose of abuse validation testing.
* ``New-TestSP`` creates a new service principal and associates it with the app created by the above function.
* ``Test-MGAddSelfAsOwnerOfApp`` is used in abuse validation testing to determine whether a service principal with a particular privilege can grant itself ownership of an existing AzureAD app.
* ``Test-MGAddSelfAsOwnerOfSP`` is used in abuse validation testing to determine whether a service principal with a particular privilege can grant itself ownership of an existing AzureAD service principal.
* ``Test-MGAddSelfToAADRole`` is used in abuse validation testing to determine whether a service principal with a particular privilege can add itself to an AzureAD admin role - Global Admin, for example.
* ``Test-MGAddSelfToMGAppRole``is used in abuse validation testing to determine whether a service principal with a particular privilege can grant itself a particular MS Graph app role without admin consent.
* ``Test-MGAddOwnerToRoleEligibleGroup`` is used to test whether a service principal can grant itself explicit ownership of a role assignable group.
* ``Test-MGAddMemberToRoleEligibleGroup`` is used to test whether the service principal can add itself to a role assignable group.
* ``Test-MGAddSecretToSP`` is used to test whether the service principal can add a new secret to an existing service principal.
* ``Test-MGAddSecretToApp`` is used to test whether the service principal can add a new secret to an existing app.
* ``Invoke-AllAzureMGAbuseTests`` performs all abuse validation tests that can be executed by holding an MS Graph app role. Returns an object describing which privileges were successful at performing each abuse test.
* ``Invoke-AllAzureADAbuseTests`` performs all abuse validation tests that can be executed by principals granted AzureAD admin roles. Returns an object describing which privileges were successful at performing each abuse test.
* ``ConvertTo-Markdown`` is used for massaging output from the Invoke-<type>Tests functions for usage in another platform.

![Apache_Bloodhound-Logo wine](https://github.com/Sulaimannabdul/Barking/assets/151133481/4a71bcaa-f5e8-4e81-bb1b-944d189cfc9d)

#### **Credit to bloodhound and bark repo.**
