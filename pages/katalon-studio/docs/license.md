---
title: "Type of Licenses"
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/license.html
description:
---

> Starting from **version 7.0.0**, you need a license to activate and use one of the Katalon Studio products, including Katalon Studio Enterprise (KSE), Katalon Studio (KS), and Katalon Runtime Engine (KRE).

This section provides information on the licensing system of Katalon. You will find description of Katalon products and their available license types.

## Katalon Studio Enterprise

KSE license is named license, meaning:

* One license is exclusively assigned to one Katalon account/user.
* One account can be activated/used on one machine at a time.
* Licenses are transferable.
* License activation and validation require an internet connection.

## Katalon Runtime Engine

KRE license can be a node-locked or Floating license. When running from the command-line interface (CLI), one working session accounting for one license equals to a conducted process. Learn more about the use cases of [KRE](https://docs.katalon.com/katalon-studio/docs/intro-RE.html).

## License types

### Node-Locked License

This license type is applied to local desktops or workstations with fixed hardware specifications (machine-blocked license):

* Virtual machine with fixed machine ID
* Physical machine

The number of licenses to acquire should be based on the number of execution machines.

* A license is linked to a single machine ID and for one execution session.
* A machine can be mapped to multiple licenses (if needed).
* The license can be transferred to a new machine for an online environment. For the offline environment, once converted, the license cannot be transferred to another machine until it is expired.

> This license allows both online and offline activation for **annual subscriptions**. With monthly subscriptions, only online activation is allowed.

### Floating License

This license type is applied to all types of execution environments, including cloud or virtual machines with dynamic hardware specifications (to execute tests in Docker, Azure, AWS).

* One floating license can be shared across maximum of 3 machines.
* One floating license is assigned to one execution session at a time.

For instance, you have 1 floating Katalon Studio Enterprise license attached to the email example@katalon.com.
You can use example@katalon.com to log in to Katalon Studio and enjoy all of the Enterprise level features in 3 different machines at maximum. 
However, since you only have 1 floating Katalon Studio Enterprise license, you can only be active on 1 of that 3 machines at a time.

> Only online activation is allowed.