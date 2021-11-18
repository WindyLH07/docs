---
title: "Katalon Studio Preferences" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/katalon-studio-preferences.html 
redirect_from:
    - "/display/KD/Katalon+Studio+Preferences/"
    - "/display/KD/Katalon%20Studio%20Preferences/"
    - "/x/NQRO/"
    - "/katalon-studio/docs/katalon-studio-preferences/"
    - "/katalon-studio/docs/test-case-preferences.html"
    - "/display/KD/Test+Case+Preferences/"
    - "/display/KD/Test%20Case%20Preferences/"
    - "/x/ZIUw/"
    - "/katalon-studio/docs/test-case-preferences/"
    - "/display/KD/Proxy+Preferences/"
    - "/display/KD/Proxy%20Preferences/"
    - "/x/hw1O/"
    - "/katalon-studio/docs/proxy-preferences/"
    - "/katalon-studio/docs/proxy-preferences.html"
    - "/display/KD/Object+Spy+Preferences/"
    - "/display/KD/Object%20Spy%20Preferences/"
    - "/x/iw1O/"
    - "/katalon-studio/docs/object-spy-preferences/"
    - "/katalon-studio/docs/object-spy-preferences.html"
    - "/katalon-studio/docs/dark-theme.html"
    - "/x/YYUw/"
    - "/katalon-studio/docs/execution-preferences-version-50-and-below/"
    - "/katalon-studio/docs/execution-preferences-version-50-and-below.html"
description: 
---

Katalon Studio Preferences define default behaviors of Katalon Studio across projects. You can configure the below preferences:
- Katalon Preferences
- Import Preferences
- Test Case Preferences
- Proxy Preferences
- Object Spy Preferences
- Katalon Studio themes
## Katalon Preferences

To configure Katalon general behaviors at startup, go to **Katalon Studio > Preferences > Katalon** from the menu. You can see the following options:

<table>
<thead>
  <tr>
    <th>Options</th>
    <th>Capabilities</th>
    <th>Notes</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Show Help at startup</td>
    <td>This option allows you to turn on/off the <strong>Help</strong> page at startup.</td>
    <td></td>
  </tr>
  <tr>
    <td>Automatically check for new version</td>
    <td>This option allows Katalon to check for the latest Katalon version automatically.</td>
    <td></td>
  </tr>
  <tr>
    <td>Allow usage tracking</td>
    <td>This option allows you to configure the usage tracked by Katalon Studio. <br>By default, Katalon Studio is allowed to collect errors, execution logs, and other information about your application use. <br>You can refer to this document: <a href="https://www.katalon.com/terms/katalon/privacy-policy/">Privacy Policy</a> for further details of our tracking.</td>
    <td rowspan="3">To disable these functions, you need an active Katalon Studio Enterprise license. <br>You can refer to this document to learn more about activating licenses: <a href="https://docs.katalon.com/katalon-studio/docs/activate-license.html#activate-trial-license">Activate Katalon License.</a></td>
  </tr>
  <tr>
    <td>Received dynamic content notifications</td>
    <td>From Katalon version 8.2.0 onwards, you can stop receiving notifications from the Katalon Studio team by unchecking this option.</td>
  </tr>
  <tr>
    <td>Show Start Page contents</td>
    <td>From Katalon version 8.2.0 onwards, you can hide Start Page contents by unchecking this option.</td>
  </tr>
</tbody>
</table>

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/katalon-studio-preferences/KS-PREF-Katalon-preferences.png" width=70% alt="Katalon preferences">

## Import Preferences

Katalon supports an in-app upgrade function for a smooth transition to the latest version (In **Help** menu > select **Check for updates...** > in the displayed dialog, download the latest version). The latest version upgraded via this channel will reuse the current version's Preferences configurations.

In case you have to download the latest version from the Katalon website and want to reuse the Preferences configurations of another Katalon Studio instance already installed in your machine, or you want to reuse the Preferences configurations of your project team, do as follows:

1. Rename the current Katalon Studio instance with its version number. For example, Katalon Studio 7.8.
2. Download the latest version from the [Katalon website](https://www.katalon.com/download/).
3. Open Katalon Studio, select **File** > **Import Settings**.
   
   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/katalon-studio-preferences/import-settings.png" width=50% alt="import settings">
   
4. Browse to the **config** folder of your preferred version. For instance:

* macOS:

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/katalon-studio-preferences/macos.png" width=100% alt="Browse to the Config folder in macOS">

* Windows:

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/katalon-studio-preferences/import_3.PNG" width=100% alt="Browse to the Config folder in Windows">

5. Click **Open**.

## Test Case Preferences

All the preferences under the **Test Case** group are for controlling the default behaviors that Katalon Studio should perform when test cases are designed.

You can configure the Test Case preferences via **Katalon Studio > Preferences > Katalon > Test Case**.

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-case-preferences/Window.png" width=70% alt="Test Case Preferences">

### Test Case Calling

This is to specify how Katalon Studio should behave when you are calling another test case in your current one.

* **Generate variable with default value**: Called test case uses the default values for its variables.
* **Generate variable with the same name as the exposed variable of the called test case**: Called test case uses the default values, which are the same as its variables name.
  * **Expose variables automatically after choosing the called test case**: Called test case uses the default values, which are the same as its variables name. The variables are also added to the current test case at the 'Variables' tab.

You might need to refer back to the [Variable Types](https://docs.katalon.com/katalon-studio/docs/variable-types.html#test-case-variables) section for which types of variables are supported in Katalon Studio.

### Initially open Test Case

This is to indicate in which view Katalon Studio should display a test case when it is first opened.

* **In Manual View**: The opened test case will be first in the manual view.
* **In Script View**: The opened test case will be first in the script view.

### Default Keyword Type

* **Default Keyword**: These default keywords will be available when a new step is added to your test case.

### Line-wrapping Settings

This is to enable Katalon Studio to wrap up the code lines in a script with a customized maximum line width. You can also wrap the code lines when switching from the manual mode to the script mode by pressing a keyboard combination of **Command+Shift+F** (Mac Users) or **Ctrl+Shift+F** (Windows and Linux Users).

Before the line-wrapping enabled:

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-case-preferences/wrap.png" width=100% alt="Before the line-wrapping enabled">


After the line-wrapping enabled:

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-case-preferences/wrapped.png" width=100% alt="After the line-wrapping enabled">


> All the above preferences are saved into the  `com.kms.katalon.composer.testcase.prefs` file under the "**config\\.metadata\\.plugins\\org.eclipse.core.runtime\\.settings**" location in your Katalon Studio build folder. You can manually modify the values in this file to change these preference settings.

## Proxy Preferences

From Katalon Studio version 7.5.0 onwards, the proxy is divided into two categories: Authentication and System proxies. You can apply different proxy configurations for connecting to the Katalon server and your servers during testing.

Please go to **Katalon Studio> Preferences > Katalon > Proxy** and select **Authentication** or **System** section for corresponding proxy configuration of each type.

### Authentication Proxy

The proxy configurations in this section are used for all network connections to authenticate with Katalon Servers including Katalon account authentication, Katalon Auto-updater, Katalon TestOps, and  Katalon Store integration, sample projects provider, AMI Authentication, and etc.)

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/proxy-preferences/auth-proxy.png" width="70%" alt="Authentication proxy">

### System Proxy

System proxy configurations are applied to all network connections generated when using Katalon Studio, including but not limited to recording, spying, executing tests, integrating with other tools, and downloading Web Drivers or Android SDK.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/proxy-preferences/proxy-system.png" width="70%" alt="System proxy">

### Proxy Settings

In the Proxy Settings areas of both Authentication and System proxies, you can select one of three options below.

* **No proxy**: there's no proxy.
* **Use system proxy configuration**: Katalon Studio guesses which proxy server your system is behind by checking Java, browser and operating system settings, and environment variables.
* **Manual proxy configuration**: you can manually set up your proxy
  * Address: an HTTP Proxy host
  * Port: an HTTP Proxy port
  * Excludes: A list of addresses separated by comma to exclude
  > The ability to exclude proxy is available from version 7.2.0 onwards. Katalon Studio only supports proxy exceptions in web recorder and spying with **Chrome** and **Firefox**.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/proxy-preferences/proxy-options.png" width="70%" alt="proxy settings">

### System proxy for test execution's desired capabilities

Katalon Studio applies the System proxy to test execution's desired capabilities on the instance automatically. If you wish to configure different proxy's desired capabilities for a project, you need to do as follows:

1. Open your project and go to **Katalon Studio/Preferences/Katalon/Proxy/System**
2. At the bottom of the displayed view, uncheck the **Auto-apply to test execution desired capabilities** option and click **OK** to save
   
  <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/proxy-preferences/uncheck.png" width="70%" alt="uncheck proxy for desired capabilities">

3. Go to **Project/Settings/Desired Capabilities** and select a testing environment

4. Specify proxy details and click **OK** to save

   For example:

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/proxy-preferences/desired-capabilities.png" width="70%" alt="use proxy for desired capabilities">

### Override proxy details in the test script

From version 7.0.0 onwards, Katalon Studio supports an option to pass proxy details via a request object in Web Service testing. Below is an example:

```groovy
RequestObject requestObject = findTestObject("google")
ProxyInformation proxyInfo = new ProxyInformation();
proxyInfo.setProxyServerAddress("localhost")
proxyInfo.setProxyServerPort(8001)
proxyInfo.setProxyOption(ProxyOption.MANUAL_CONFIG.toString())
proxyInfo.setProxyServerType(ProxyServerType.HTTP.toString())
requestObject.setProxy(proxyInfo)
```

> The proxy information passed in the request object takes precedence over the proxy information set in **Preferences**.

### Troubleshoot proxy issues

1. If you're behind a Proxy Server, you need to configure the Authentication proxy settings before activating Katalon Studio. Click **Configure Authentication Proxy** at the bottom of the Activation dialog box.

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/proxy-preferences/config-proxy-activation.png" width="70%" alt="troubleshoot proxy issue">

2. "*New and old proxy mechanisms are not allowed in one command. Please use either the new or the old one.*"

   If you encounter the above error when executing your test with Runtime Engine, please check if you are mixing options of the new mechanism with options for proxy configuration prior to 7.5.0 and correct the commands in use. [Learn more about proxy options](https://docs.katalon.com/katalon-studio/docs/console-mode-execution.html#proxy-options).

## Object Spy Preferences

You can access these preferences at **Window > Katalon Studio Preferences > Katalon > Object Spy.**

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/object-spy-preferences/image2017-11-27-113A43A34.png" width="70%" alt="Object spy preferences">

### Pin Object Spy Window while spying

Users can check/uncheck this option to pin Object Spy Window on top while spying for more convenience.

### Hotkeys

Katalon Studio supports customizable hotkeys for Object Spy function so that users can choose the preferred combination or avoid conflict with UAT hotkeys.

> This ability to change hotkeys for Object Spy only affects the Chrome browser. Other browsers will be considered for future releases.

## Apply Dark theme

By default, Katalon Studio has the Light theme applied. Starting from version 6.3.0, Dark Theme is available. You can enable it at **Window > Themes >Dark**. You need to restart Katalon Studio after changing the theme.
