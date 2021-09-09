---
title: "Activate Katalon Licenses"
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/license_activation.html
description:
---
In this guide, you will learn to activate the Katalon Studio Enterprise (KSE) and Katalon Runtime Engine (KRE) licenses.

## Activate the KSE/KRE online license

> Requirements:
>
> You have been added to the **Licensed Users** list. Contact your Owner/Admin if you haven't been granted a license.

After the Owner/Admins grant you a license, you can automatically use KSE. See: [Activate KSE](https://docs.katalon.com/katalon-studio/docs/activate-KSE.html).

You also activate the KRE licenses by simply using KRE online.

> Notes:
>
> From **version 7.7 onwards**, if you belong to more than one Organization purchasing KRE licenses, you can choose which organization to validate your license usage. Katalon retrieves and displays the organizations bound to your Katalon account. Once you have selected an Organization, you pass the Organization ID to the generated command (`-orgID=<Katalon_OrgID>`).

> Notes:
>
> See [Command Syntax](https://docs.katalon.com/katalon-studio/docs/console-mode-execution.html#katalon-studio-plugins-in-console-mode) for further instructions on working with KRE.

For an Enterprise user with a private network, you might encounter a situation where you fail to execute test scripts or integrate Katalon Studio due to the network security error. In such case, contact your IT team to whitelist the following domains:

* store.katalon.com
* update.katalon.com
* analytics.katalon.com
* testops.katalon.io
* admin.katalon.com
* katalon-test.s3-accelerate.amazonaws.com (used for uploading reports to Katalon TestOps).

> Notes:
>
> See also [Install Runtime Engine](https://docs.katalon.com/katalon-studio/docs/install-RE.html) for installing and executing KRE.

## Activate the KSE/KRE offline license

> Notes:
>
> You must provide the Owner/Admins with your machine ID. The Owner/Admins then grant you an offline license file.
> 
> To find your machine ID and send it to the Owner/Admins, follow these steps:
> 1. Download and open Katalon Studio.
> 2. In the **Katalon Studio Enterprise Activation** log, click **Offline Activation** to view and copy the machine ID.
> <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/create-offline-kse-licenses/view-machineid.png" width="494" height="" alt="kse activation log">
>
> 3. Send the machine ID to the Owner/Admins.

### For KSE

To activate and use the KSE license offline, follow these steps:

1. Download the KSE offline license file (named `KSE_<machineID>.lic`).
2. Open Katalon Studio.
4. Go to **Katalon Studio Enterprise Activation** log, then click **Offline Activation**.
5. Browse the license file with the corresponding machine ID.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/create-offline-kse-licenses/activate.png" width="498" height="" alt="kse activation log">
6. Click **Activate**.

You have activated the offline license.
You can now use KSE in an offline environment.

### For KRE

To activate the KRE license offline, download the KRE offline license file (named `KRE_<machineID>.lic`).

Depending on your operating system, you can find the **license** folder as follows:

* For Windows: **C:\Users\<user_name>\.katalon\license**.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/activate-RE/license.png" width="" height="" alt="license folder location">

* For Linux: **/home/<user_name>/.katalon/license**

* For MacOS: **/Users/<user_name>/.katalon/license**

    > Notes:
    >
    > **.katalon** is a hidden folder.
  
Now you can use the KRE offline license to execute KSE from the command-line interface and in the offline environment:

* To execute a single session, put an offline license file  in the **license** folder.
* To execute multiple sessions in parallel, put multiple offline license files in the **license** folder.
