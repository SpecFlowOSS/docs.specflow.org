# License to Account Migration

We have introduced a new license model for SpecFlow+ and SpecMap. This new licensing model is account-based instead of requiring a license key. You need to sign up for a free personal SpecFlow account in order to use SpecFlow+ and SpecMap. Learn more about the SpecFlow account [here](../specflowaccount.md).

## What are the benefits?

Signing up for a free SpecFlow account allows you to use the previously paid SpecFlow+ (Runner and LivingDoc) and SpecMap products for free. You no longer need to wait for us to process your request for a license manually and can expand your use of the software to more users as required. We also plan to offer exclusive additional benefits to help you boost your productivity and get the most out of SpecFlow and SpecMap.

## Migrate to the SpecFlow Account

In order to migrate from an existing active SpecFlow+ or SpecMap license key to the new SpecFlow Account follow the step-by-step instructions below.

### SpecFlow+ Runner

Migrate from an active license key for the SpecFlow+ Runner to the SpecFlow account:

**1-** Update to the latest [SpecFlow+Runner NuGet Runner package](https://www.nuget.org/packages/SpecRun.SpecFlow/)

**2-** Unregister your license key – Follow the instructions [here](../managinglicenses.md)

**3-** Return to your IDE and run your scenarios

**4-** Open the URL from the console message in your browser

You are displayed with a “Welcome Page”. Click on **Sign in with Microsoft** to continue

Test- Output window in Visual Studio:
![Runner sign up](./_static/images/runnerimage.png)

**5-** Sign in with your Microsoft account. It can be a personal or corporate/enterprise account. If you are already signed in to your Microsoft account, this should happen automatically – *you might need additional permissions from your Active Directory admin. Learn more about admin consents [here](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-admin-consent-workflow)*

**6-** You will be taken to a setup page where you can set up your SpecFlow account. Enter your details to sign up for a free SpecFlow account

**7-** After you finished the sign-up, return to your IDE and run your scenarios again

**Important Note for Active Directory Approvals:** It might be possible, that your Active Directory admin needs to grant you and your team permission to use the SpecFlow+ Runner due to your organizations’ Active Directory configuration. Learn more about admin consents [here](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-admin-consent-workflow).

### SpecFlow+ LivingDoc

Migrate from an active license key for SpecFlow+ LivingDoc to the new SpecFlow account:

**1-** Update to the latest version of SpecFlow+ LivingDoc – *usually happens automatically for Azure DevOps*

**2-** Start SpecFlow+ LivingDoc under **(Overview| SpecFlow+ LivingDoc)** in Azure DevOps

**3-** Click on *Issued to*

**4-** Clear the *Issued to* field

**5-** Update

**6-** Click on *Sign in with Microsoft*

**7-** Sign in with your Microsoft account. It can be a personal or corporate/enterprise account. If you are already signed in, this should happen automatically – *you might need additional permissions from your Active Directory admin. Learn more about admin consents [here](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-admin-consent-workflow)*

**8-** You will be taken to a setup page where you can set up your SpecFlow account. Enter your details to sign up for a free SpecFlow account.

**9-** Return to SpecFlow+ LivingDoc and refresh your browser

**Important Note for Active Directory Approvals:** It might be possible, that your Active Directory admin needs to grant you and your team permission to use the SpecFlow+ LivingDoc due to your organizations’ Active Directory configuration. Learn more about admin consents [here](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-admin-consent-workflow).

### SpecMap

Migrate from an active license key for SpecMap to the new SpecFlow account:

**1-** Update to the latest version of SpecMap – usually happens automatically for Azure DevOps

**2-** Start SpecMap under **(Boards| SpecMap)** in Azure DevOps

**3-** Click on the *Help – ? –* icon in the toolbar

**4-** Click on *Issued to*

**5-** Clear the *Issued to* field

**6-** Save

**7-** Click on *Sign in with Microsoft*

**8-** Sign in with your Microsoft account. It can be a personal or corporate/enterprise account. If you are already signed in, this should happen automatically – *you might need additional permissions from your Active Directory admin. Learn more about admin consents [here](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-admin-consent-workflow)*

**9-** You will be taken to a setup page where you can set up your SpecFlow account. Enter your details to sign up for a free SpecFlow account

**10-** Return to SpecMap and refresh your browser

**Important Note for Active Directory Approvals:** It might be possible, that your Active Directory admin needs to grant you and your team permission to use the SpecMap due to your organizations’ Active Directory configuration. Learn more about admin consents [here](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-admin-consent-workflow).

### Do you have any further questions?

We want to make the transition as easy as possible. If you have any questions or concerns, please take a look at our [FAQs](https://specflow.org/plus/documentation/FAQ/).
