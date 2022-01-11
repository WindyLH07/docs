---
title: "Test Suite and Test Suite Collection Reports"
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/test-suite-report.html
redirect_from:
    - "/display/KD/Test+Suite+Report/"
    - "/display/KD/Test%20Suite%20Report/"
    - "/x/v4IY/"
    - "/katalon-studio/docs/test-suite-report/"
    - "/display/KD/Test+Report/"
    - "/katalon-studio/tutorials/viewing_test_suite_reports.html"
    - "/katalon-studio/docs/basic-report.html"
    - "/display/KD/Test+Suite+Collection+Report/"
    - "/display/KD/Test%20Suite%20Collection%20Report/"
    - "/x/7gAM/"
    - "/katalon-studio/docs/test-suite-collection-report/"
    - "/katalon-studio/docs/test-suite-collection-report.html"
    - "/katalon-studio/docs/get-generated-reports-location-at-runtime.html"
    - "/display/KD/Get+generated+Reports+location+at+runtime/"
    - "/display/KD/Get%20generated%20Reports%20location%20at%20runtime/"
    - "/x/ewXR/"
    - "/katalon-studio/docs/get-generated-reports-location-at-runtime/"
    - "/display/KD/Video+Capturing/"
    - "/display/KD/Video%20Capturing/"
    - "/x/qRJO/"
    - "/katalon-studio/docs/video-capturing/"
    - "/katalon-studio/docs/video-capturing.html"
description:
---

## Test suite report

> Starting from version 6.3.0, reports can be viewed directly inside each Test Suite page.

After executing a test suite, to see the test suite report, go to the **Result** tab.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/KS-REPORTS-Test-suite-results-tab.png" width="100%" alt="Results tab"> 

<table><thead><tr><th>Component</th><th>Description</th></tr></thead><tbody><tr><td>Test cases table</td><td>List of executed test cases.</td></tr><tr><td>Summary</td><td>Summary information of executed environment.</td></tr><tr><td>Execution settings</td><td><p>Settings of executed browsers/devices. For example:</p><p style="text-align: center;"><a class="pop"><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/KS-REPORTS-Execution-settings.png"></a><br><em>Click the image to enlarge it.</em></p></td></tr><tr><td>Execution environment</td><td><p>Other information about the executed system. For example:</p><p style="text-align: center;"><a class="pop"><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/KS-REPORTS-Execution-environment.png"></a><br><em>Click the image to enlarge it.</em></p></td></tr></tbody></table>

### Test cases List

The summary information of all executed iterations done in the test suite is displayed here. Each time when a test case is executed with a test data row is considered an iteration.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/image2017-2-24-193A153A33.png" width="80%" alt="Test cases list"> 

Users can easily determine which type of information to be displayed by using the provided filters:

| Filter | Description |
| --- | --- |
| Passed | Show only iterations which are passed. |
| Failed | Show only iterations which are failed. |
| Error | Show only iterations having errors. |
| Incomplete | Show only incomplete iterations |

If qTest and JIRA are configured in project settings, you can submit data to those systems. To learn more about qTest and Jira integration, you can refer to the following documents:
- [qTest Integration](https://docs.katalon.com/katalon-studio/docs/qtest-integration.html)
- [JIRA Integration](https://docs.katalon.com/katalon-studio/docs/jira-integration.html)

### Test suite summary

This section gives the summary information of the test suite:

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/KS-REPORTS-Summary.png" width="100%" alt="Test suite summary"> 


| Field | Description |
| --- | --- |
| Test Suite ID | The ID of the executed test suite in Katalon Studio. |
| Hostname / OS / Platform | The environment where the test suite was executed |
| Start / End / Elapse | Execution start/end date time and duration |
| Total TC | Total number of test cases, along with their executed status. |

### Test case log details

To view details of the executed logs, in the **Test Case Table**, select an iteration and click **Show Test Case Details**.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/KS-REPORT-Show-test-case-details.png" width="80%" alt="Show Test Cases Details"> 

1. Test log tab

    Details regarding all the executed steps and their status are displayed in this tab. 

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/image2017-2-24-203A293A56.png" width="80%" alt="Test log tab"> 

    <table><thead><tr><th>Component</th><th>Description</th></tr></thead><tbody><tr><td>Log Information</td><td>Information of the test step selected in the <strong>Test Case's Log</strong> section:<ul><li>The <strong>Name</strong> of the test step (the name of the keyword used in the test step)</li><li>Execution <strong>Start/End</strong> date time and duration</li><li>The <strong>Description</strong> of the test step</li><li>Any system <strong>Message</strong> raised when the test step was executed</li></ul></td></tr><tr><td>Log Image</td><td><p>The screenshot taken from the application under test, it is captured in either of following situations:</p><ul><li>An error occurs during test execution</li><li>The <code>take screenshot</code> keyword is used. To learn more about the <code>take screenshot</code> keyword, you can refer to the following document: <a href="https://docs.katalon.com/katalon-studio/docs/webui-take-screenshot.html" target="_blank" rel="noopener noreferrer">[WebUI] Take Screenshot</a></li></ul></td></tr></tbody></table>

    Users can easily determine which type of information to be displayed by using the provided filters:

    | Filter | Description |
    | --- | --- |
    | Info | Show the messages logged for information/reference. |
    | Passed | Show the steps which are successfully executed. |
    | Failed | Show the steps which are failed to execute. |
    | Error | Show the steps having errors. |
    | Incomplete | Show incomplete steps due to other factors such as wrong syntax, power shortage, disconnected network, etc... |
    | Warning | Show the steps which have warning status. |
    | Not Run | Show the skipped steps. |

    If you have configured Jira integration, you can submit a ticket to this system. For further details, you can refer to this document: [Submit an issue to Jira](https://docs.katalon.com/katalon-studio/docs/jira-integration.html#submit-an-issue-to-jira).
    Screenshots are taken for the failed steps and you can hover the mouse cursor over the attachment icon to review.

2. Information Tab

    Users can find the summary information of the test case in this tab.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/image2017-2-24-203A43A11.png" width="80%" alt="Information tab"> 

    | Field | Description |
    | --- | --- |
    | Test Case ID | The ID of the executed test case in Katalon Studio. |
    | Start / End / Elapse | Execution start/end date time and duration. |
    | Description | The description of the test case. |
    | Message | Any system message raised when this iteration was executed. |

3. Integration Tab

    The information regarding qTest Integration of this iteration is displayed in this tab.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/image2017-2-24-203A153A4.png" width="80%" alt="Integration tab"> 

    | Field | Description |
    | --- | --- |
    | Test Log ID | The ID of the integrated qTest Test Run. |
    | Test Run Alias | The alias of the integrated qTest Test Run. |
    | Attachment | Indicate whether all the execution log and report are placed in a zipped file which is sent to qTest as an attachment. |

## Test Suite Collection Report

> Starting in version 6.3.0, reports can be viewed directly inside each Test Suite Collection page.
>
> Test Suite Collection Report are only available for Katalon Studio Enterprise users.

After executing a test suite collection, to see the test suite collection report, go to the **Result** tab.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/KS-REPORTS-Results-of-the-TSC.png" width="100%" alt="Test suite collection report">


| Field | Description |
| --- | --- |
| ID | The ID of the executed test suite in Katalon Studio. |
| Environment | The environment which the test suite is executed on. |
| Status | Information about whether the execution is completed or not. |
| Failed Tests / Total | Total test cases in the test suite and the number of failed test cases if any. |
| Test Suite Details | Shows test suite reports, see above: [Test suite reports](https://docs.katalon.com/katalon-studio/docs/test-suite-report.html#test-suite-report). |

## Report History

> Report History is only available for Katalon Studio Enterprise users.

Once a test suite/test suite collection finishes its execution, a historical report will be automatically generated and stored in Reports.

For example:

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/image2017-2-24-193A13A55.png" width="" alt="Test suite history reports">
<br>
<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-collection-report/image2017-2-24-203A483A52.png" width="" alt="Test suite collection history reports">

The report will be named with the following naming convention: _YYYYMMDD_HHmmss_, which is the datetime when the test suite/ test suite collection starts its execution.

## Export reports to other formats

For the purpose of sharing, users can export reports of test suites into other formats such as **HTML**, **CSV**, **PDF** and **JUnit**.

> For Katalon Studio version 6.1.5- 6.3.3, please install [Basic Report](https://store.katalon.com/product/59/Basic-Report) plugin to use this feature.

> Starting in version 7.0, Katalon Studio automatically generates junit report for both Test Suite and Test Suite Collection.

### Automatically generate reports

In **Project > Settings > Plugins > Report**, select the formats of reports that will be automatically generated after each Test Suite execution.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/KS-REPORTS-Reports-settings.png" width="70%" alt="Reports settings">

Execute a Test Suite and observe the *Log Viewer* after the test execution completes. The generated reports will be the same as the settings you've configured above.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/Basic%20Report/log-viewer.png" width="391" alt="Report generator in the log viewer">

You can view the generated reports in `<project_folder>\\Reports\\<execution_folder>` after the test execution finishes.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/Basic%20Report/report-folder.png" width="" alt="report folder">

### Manually export reports

Open the **Result** view of a Test Suite or a Test Suite Collection > on the top right corner, select **Export report** > choose a format to export.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/KS-REPORTS-Export-reports-manually.png" width="100%" alt="Manually export reports">

> For Test Suite Collection, you can export to **HTML** format only.

## Get generated reports location at runtime

To retrieve current generated reports location, you can use the sample code below:

```groovy
import com.kms.katalon.core.configuration.RunConfiguration
RunConfiguration.getReportFolder()
```

You can also retrieve other information through the RunConfiguartion package, please refer to this documentation: [RunConfiguration](https://api-docs.katalon.com/com/kms/katalon/core/configuration/RunConfiguration.html).

## Video Capturing

> * K-Lite Codec is recommended to play the Katalon Studio test execution video. You can download K-Lite Codec in the Codec Guide website: [K-Lite Codec](https://www.codecguide.com/download_kl.htm). 
> * Support execution at the test suite level.
> * Support all browsers except for Remote, Headless, Kobiton, Custom. For remote or headless browsers, it's recommended to use [Katalium Server](https://docs.katalon.com/katalium-server/docs/katalium-server-katalon-studio-remote-machine.html) to view captured sessions.
> * Recording parallel execution is NOT supported yet.

Debugging can be time-consuming and challenging for many automation testers. Katalon Studio helps solve this problem by supporting users with the ability to capture test execution via video format. Users can enable video capturing feature in Project Settings.

Follow the steps below to see how to work with Katalon Studio video capturing feature

1. After creating a test suite in Katalon Studio, select **Project > Settings > Execution**. Check the **Enable Video Recorder during execution** option. 

    By default, Katalon Studio only captures **Failed** test cases. However, users can select options to capture only the **Passed**/**Failed** test cases or both. 

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/KS-REPORTS-Enable-video-recording.png" width="100%" alt="Enable video capturing">

    Video settings can be specified based on the preferences of users. Katalon Studio recommends AVI (`.avi`) format and low quality to save disk space. The higher the video quality is, the bigger the file size is.

    * **Video format**: AVI (`.avi`) or MOV (`.mov`)

    * **Video quality**: Low; Medium or High

3. After executing a test suite, navigate to the **Result** tab, you can view the list of test cases in the test cases table with its video attached accordingly. 
    To play the video, click on the play icon in the **Video** column . Test steps descriptions are embedded as a subtitle.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-suite-report/KS-REPORTS-Watch-the-video.png" width="100%" alt="View video capturing">

By watching how the automated test was executed, the testing team can identify exactly where the test failed. Thus, time and resources are managed more efficiently and effectively.
