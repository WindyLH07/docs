---
title: "Installing WebDriverAgent for iOS devices"
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/installing-webdriveragent-for-ios-devices.html
redirect_from:
    - "/display/KD/Installing+WebDriverAgent+for+iOS+devices/"
    - "/display/KD/Installing%20WebDriverAgent%20for%20iOS%20devices/"
    - "/x/TwbR/"
    - "/katalon-studio/docs/installing-webdriveragent-for-ios-devices/"
description:
---

> If you use **Android** devices, this setup process is **NOT** neccesary. To learn more about setting up Android devices, you can refer to this document: [[Mobile] Android Setup](https://docs.katalon.com/katalon-studio/tutorials/mobile-android-setup.html#set-up-android-tests-on-windows-and-macos)

WebDriverAgent is a WebDriver server used to control iOS devices remotely. You need to install and set up WebDriverAgent for Katalon Studio to automate iOS devices.

1\. Open **Xcode > Preferences > Accounts** > add your developer's Apple ID.

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/installing-webdriveragent-for-ios-devices/add-apple-id.png" width=85%>

2\. Open **Terminal** > enter the following commands to initialize the **WebDriverAgent** project:

  - Appium 2.32.0
    ```groovy
    cd /usr/local/lib/node_modules/appium/node_modules/appium-webdriveragent
    mkdir -p Resources/WebDriverAgent.bundle
    ```
  - Appium 1.15.0+
    ```groovy
    cd /usr/local/lib/node_modules/appium/node_modules/appium-webdriveragent
    mkdir -p Resources/WebDriverAgent.bundle
    sh ./Scripts/bootstrap.sh -d
    ```

  - Appium 1.14.2 or older versions
    ```groovy
    cd /usr/local/lib/node_modules/appium/node_modules/appium-xcuitest-driver/webdriveragent
    mkdir -p Resources/WebDriverAgent.bundle
    sh ./Scripts/bootstrap.sh -d
    ```

    > **Common issues**
    >
    > * Error code 13: re-run command with sudo: **sudo ./Scripts/bootstrap.sh -d**
    >
    > * Error _Error StackTrace: Cannot find module 'eslint-config-appium': _missing paramter -d when running **./Scripts/bootstrap.sh**

3\. Log in to you Apple developer account and [register your device](https://www.wikihow.com/Add-a-New-Device-to-Your-Apple-Developer-Portal).

4\. Go to **File** > **Open** > type "appium-webdriveragent" in the search bar > Select **WebDriverAgent.xcodeproj**.

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/installing-webdriveragent-for-ios-devices/xcodeproj.png" width=85%>

5\. Select **WebDriverAgentLib** > in the **Signing & Capabilities** section, check **Automatically manage signing** > select a team.

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/installing-webdriveragent-for-ios-devices/lib.png" width=85%>

   On the menu bar, select **Product > Build**.

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/installing-webdriveragent-for-ios-devices/build-lib.png" width=85%>

6\. Select **WebDriverAgentRunner** > in the **Signing & Capabilities** section, check **Automatically manage signing** > select a team. 

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/installing-webdriveragent-for-ios-devices/runner.png" width=85%>

   On the menu bar, select **Product > Build**.

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/installing-webdriveragent-for-ios-devices/build-runner.png" width=85%>
