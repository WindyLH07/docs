---
title: "Jira Integration"
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/jira-integration.html
redirect_from:
    - "/katalon-studio/docs/configure-jira-integration/"
    - "/katalon-studio/docs/BDD-field-jira-cloud/"
    - "/katalon-studio/docs/install-and-use-katalons-jira-add-on/"
    - "/display/KD/Install+and+Use+Katalon%27s+JIRA+add-on/"
    - "/display/KD/Install%20and%20Use%20Katalon%27s%20JIRA%20add-on/"
    - "/x/TBBO/"
    - "/katalon-studio/docs/working-with-jira/"
    - "/display/KD/Configure+JIRA+Integration/"
    - "/display/KD/Configure%20JIRA%20Integration/"
    - "/x/7oEw/"
    - "/display/KD/JIRA%20Integration/"
    - "/display/KD/Working+with+JIRA/"
    - "/display/KD/Working%20with%20JIRA/"
    - "/x/MhBO/"
    - "/katalon-studio/docs/jira-plugin-integration.html"
    - "/katalon-studio/tutorials/katalon_studio_integration_with_jira_overview.html"
description:
---

Katalon Studio can natively integrate with both Jira Cloud and Jira Server. This integration helps you:

* Link a Katalon Studio project with a Jira project.
* Import Test Cases from Jira to Studio for creating test cases, and BDD tests.
* Automatically submit test results and their attachments to the linked Jira issue.
* Submit Bugs to Jira.

**Prerequisites**

* Install [Jira Integration plugin](https://store.katalon.com/product/3/Jira-Integration) for Katalon Studio from Katalon Store.
* Install [Katalon app](https://marketplace.atlassian.com/apps/1217501/katalon-bdd-test-automation-for-jira) for Jira from Atlassian Marketplace.

> Notes
> 
> If you need to enable Jira integration with [Katalon TestOps](https://analytics.katalon.com) to have an insightful look at your testing data and better test management. Refer to [TestOps - Jira Integration](https://docs.katalon.com/katalon-analytics/docs/kt-jira-config.html) to learn how to configure the integration.

## Configure Jira integration 

You need to enable JIRA Integration in order to submit issues to JIRA. Go to **Project > Settings > Plugins > JIRA**.

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/jira-plugin-integration/config.png)

1. Select **Enable integration** option. The settings will be available for configuration.

  * Jira Cloud
    * *Server URL* must be in the form *https://<site_name>.atlassian.net*.
    * Use a Atlassian Cloud's API token for *Password*. See instructions [here](https://confluence.atlassian.com/cloud/api-tokens-938839638.html).

  * Jira Server
    * *Server URL* must be in the form *http(s)://domain* without any trailing parts e.g. */secure*.
    * Use username instead of email for *Username*.

2.  Specify information regarding your JIRA Server and login credentials then click the **Connect** button.

3.  After successfully authenticating with JIRA, all relevant **JIRA Projects** and **Issue Types** will be retrieved and displayed under **Submit Options**. You can specify the default project and issue type for submission here.

The fields for setting include:

| Field | Description |
| --- | --- |
| Default JIRA Project | The default JIRA project to submit tickets. |
| Default JIRA Issue Type | The default JIRA Issue type to create when submitting tickets. |
| Use Test Case name as Summary for JIRA ticket | The Katalon Test Case Name will be used as a summary for submitted tickets. |
| Attach Screenshot to JIRA ticket | Any taken screenshot during execution will be included in submitted tickets. |
| Attach Log to JIRA ticket | The execution log will be included in submitted tickets. |

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/jira-plugin-integration/image2016-11-3-133A533A20.png)


4.  Click **OK** button to complete the JIRA Integration setup.

## Import Test Cases from Jira

1. Prepare [Jira JQL Script](https://confluence.atlassian.com/jirasoftwarecloud/advanced-searching-764478330.html)

   ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/jira-plugin-integration/image2017-8-2-113A393A33.png)

2. Select the **Jira Integration** icon > select **Import Test Case from JIRA JQL**
![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/jira-plugin-integration/image2017-8-2-113A233A49.png)

3. Enter the Jira JQL and click **OK**.
![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/jira-plugin-integration/image2017-8-2-113A413A34.png)

4. In the displayed **Test Case Folder Selection** window, select the destination to store the issues. Click **OK**.
![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/jira-plugin-integration/save_test_cases.png)

5. In the **Linked Jira Issues** window, click **OK**.
![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/jira-plugin-integration/image2016-11-3-143A413A132.png)

If your test cases have already been linked to a JIRA ticket, Katalon Studio will not sync them again.

## Import BDD Feature Files

### Jira Server Integration

Once you have enabled the integration with Jira Server, you can import Jira BDD Feature Files to Katalon Studio. When importing test cases from Jira, please check **Link to BDD Feature File** &gt; **OK** &gt; Choose the destination to store the issues.

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/jira-plugin-integration/sample.png)

A new Feature File (with the same name as the test case) will be created with the content from Jira BDD. Moreover, a RunFeature step will be created in the linked test case to Jira.

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/jira-plugin-integration/bdd2.png)

### Jira Cloud Integration

> Introduced in version 7.8

When importing Jira tickets with BDD feature file from Jira Cloud, you can import the BDD field to Katalon Studio as well by turning on this setting in Project Settings.

1. Go to **Project/Settings/Plugins/Jira**.
2. In the **Fetch Options** section, select **Enable retrieving content of the specified custom field**.
   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/configure-jira-integration/jira-bdd-78.png" width=100%>
3. Select a custom field from the list. Click **Fetch Custom Fields** to fetch the list from the connected Jira Cloud Server.

> Note: Only existing custom field ID is valid for this configuration.

4. Click **OK** to apply your settings. 

Once this setting is configured successfully in Project Settings, the custom field’s content will be retrieved like in Jira Server integration. 

## View Test Results in Jira

After a test suite execution finishes, Katalon Studio automatically uploads a test result to the integrated Jira issue. You can view the test result and its attachments (if you have predefined in Project Settings) in Jira.

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/jira-plugin-integration/image2017-8-2-173A563A40.png)

## Submit an Issue to Jira

Bug submission options will be available in Test Reports after JIRA Integration setup is successfully configured.

1. Open a test execution in **Reports** that you want to review for issues. In **Test Cases Table**, a dedicated column for JIRA Integration will be enabled.
![Test-Cases-Table](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/tutorials/katalon_studio_integration_with_jira_overview/Test-Cases-Table.png)

2. Click on the bug icon to display the list of related JIRA issues associated with the selected Test Case. The issues are shown in the following screen.
![JIRA issues associated](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/tutorials/katalon_studio_integration_with_jira_overview/JIRA-issues.png)

3. Select submit option under the **Add** command.
![Create new Jira ticket](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/tutorials/katalon_studio_integration_with_jira_overview/Add-command.png)
The bug submission options include:

<table>
    <thead>
        <tr>
            <th>Option</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Create as New</td>
            <td>A new Issue will be submitted to JIRA.</td>
        </tr>
        <tr>
            <td>Create as Sub Issue</td>
            <td>
                A sub-task for an existing JIRA issue will be created. You will be asked to provide the <b>ID</b> of the existing JIRA issue to create a sub-task within.
                <p></p>
                <p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/working-with-jira/image2017-8-2-163A123A21.png"></p>
            </td>
        </tr>
        <tr>
            <td>Link to existing Issue</td>
            <td>
                This option will append execution details to an existing JIRA issue. You will be asked to provide the ID of the existing JIRA issue for this.
                <p></p>
                <p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/tutorials/katalon_studio_integration_with_jira_overview/Link-to-existing-Issue.png"></p>
            </td>
        </tr>
    </tbody>
</table>

4. In case of creating a new JIRA issue (or Sub-task), a **JIRA native submission form** will be displayed. The following is an example form for creating a new JIRA issue:
![JIRA native submission form](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/tutorials/katalon_studio_integration_with_jira_overview/JIRA-native-submission-form.png)

5. Based on your preferences in [JIRA Integration settings](/display/KD/JIRA+Integration#JIRAIntegration-Configuration), the **Summary**, **Screenshots**, **Logs, Reporter, and Description** of test cases will be populated and attached accordingly. Once done, click on the **Create** button at bottom of the form.

6. A created **JIRA issue** will have its **ID** recorded in the **Linked JIRA issues** list so that you can quickly navigate there from Katalon Studio. You can also edit linked JIRA issue or remove the linking of the created JIRA issue.![Linked JIRA issues](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/tutorials/katalon_studio_integration_with_jira_overview/Linked-JIRA-issues1.png)

7. Once clicked on **ID**, you will be taken to **JIRA issues** page accordingly as shown below

![JIRA issues page](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/tutorials/katalon_studio_integration_with_jira_overview/JIRA-issues-page.png)

## JQL Syntax

Katalon Studio test execution status can be queried via [JQL](https://confluence.atlassian.com/jirasoftwarecloud/advanced-searching-764478330.html). The syntax is as following:

```groovy
"Katalon Status"=<status>
```

Where Status value can be one of the following:

| Status | Description |
| --- | --- |
| PASSED | The automation tests that executed successfully. |
| FAILED | The automation tests that failed to execute at certain steps. |
| INCOMPLETE | The automation tests that did not finish running all the steps due to other factors such as wrong syntax, power shortage, disconnected network, etc. |
| ERROR | The automation tests that have some errors occurred. |

For example, to search for all issues that have failed in Katalon Studio test execution_:_

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/install-and-use-katalons-jira-add-on/katalon-jira-plugin-2.png)


## Use JQL Syntax to query all issues with a particular execution status

Katalon Studio's test execution status can be queried via [JQL](https://confluence.atlassian.com/jirasoftwarecloud/advanced-searching-764478330.html). The syntax is as follows:

`"Katalon Status"="STATUS"`

For example, to search for the issues with *PASSED* status:

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/BDD-field-Jira-Cloud/passed.png)

