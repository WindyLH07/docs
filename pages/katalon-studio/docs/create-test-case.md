---
title: "Create Test Case"
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/create-test-case.html
redirect_from:
    - "/display/KD/Script+View/"
    - "/display/KD/Script%20View/"
    - "/x/Y4Iw/"
    - "/katalon-studio/docs/script-view/"
    - "/katalon-studio/docs/script-view.html"
    - "/display/KD/Manual+View/"
    - "/display/KD/Manual%20View/"
    - "/x/9YEw/"
    - "/katalon-studio/docs/manual-view/"
    - "/katalon-studio/docs/manual-view.html"
    - "/display/KD/Test+Case+Manual+View/"
    - "/katalon-studio/tutorials/create_test_case_using_manual_mode.html"
    - "/katalon-studio/docs/create_test_case_using_manual_mode.html"
    - "/katalon-studio/tutorials/create_test_case_using_script_mode.html"
    - "/katalon-studio/docs/create_test_case_using_script_mode.html"
description:
---

After you have created your Katalon Project, it's time to generate your very first Test Case. With Katalon Studio, you can create your test case with no coding effort using our Manual mode, or you can still enjoy our script mode if you have programming background. Either way, you can switch between two modes in your Test Case.

In this tutorial, we will guide you through how to create a new test case, add your test steps in manual and script mode with a usage example, and use some special function to leverage your test case in Katalon Studio.

## Create a new Test Case

To create a new Test Case, first, open your desired Katalon Project. You can learn more about how to create projects at [Projects](link).

On the right side of Katalon Studio, you can see the **Test Explorer** section containing access to all folders of your projects. In the **Test Explorer**, do as follows:

1. Right-click on the **Test Cases** folder, select **New > Test Case**. The **New Test Case** dialog appears.

2. Enter your Test Case name, description, and tag. Try to create a relevant Test Case name and provide a detailed description for better management. After you are done, click **OK**. A new Test Case is created inside the **Test Cases** folder.

    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-2-15-93A593A10.png)  

    > Tag can help you manage large projects better. You can learn how to manipulate tag properties for efficient management at [Test Case Management With Tags](https://docs.katalon.com/katalon-studio/docs/test-case-management-with-tags.html).

2. Once a new test case is created, it is opened in **Manual** view. This view allows users to create automated tests with little programming skills required. You can switch to the **Script** tab to edit in script mode.

    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-8-18-133A533A45.png)  

## Generate Test Steps

Katalon Studio supports Keywords-Driven testing where Test Cases consist of keywords that represent actions of users on the Applications Under Test (AUT). This allows users with less experience in programming to generate automation test. The below tutorial will give you step-by-step instruction in order to create an automated test case in manual and script mode.

Given a sample test case with the steps as below:

* Open the browser
* Navigate to a website
* Click on certain control
* Validate if a control exists on the page
* Close the browser

## In Manural View

To add test steps in your test case using **Manual** mode, do as follows:

1. In the **Test Case Editor**, click **Add**. A list of option appears, including:



    > **Recent keywords** allow users quickly add any of the last 10 recent used keywords in **Item** list.

    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-8-18-133A543A48.png)

4. Select the **[Open Browser](/display/KD/%5BWebUI%5D+Open+Browser)** keyword. This keyword will open a browser and navigate to the specified URL if provided. (selected keywords will have their description displayed along for reference)  
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-8-18-143A13A24.png)

5. Add the **[Navigate To Url](/display/KD/%5BWebUI%5D+Navigate+to+Url)** keyword. This keyword will navigate to a specified URL. Double click on the **Input** cell to provide additional data (parameters) for the keyword.
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-8-18-143A363A31.png)

6. The **Input** dialog is displayed.
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-6-30-193A63A59.png)
    Where:

    <table><thead><tr><th>Field</th><th>Description</th></tr></thead><tbody><tr><td>No</td><td>The number of parameter for the selected keyword.</td></tr><tr><td>Param Name</td><td>The name of the parameter.</td></tr><tr><td>Param Type</td><td>The required data type for the parameter.</td></tr><tr><td>Value Type</td><td>The type of your input value (e.g. strings, <a class="external-link" href="/display/KD/Variable+Types" rel="nofollow">variables</a>, <a class="external-link" href="/display/KD/Manage+Test+Data" rel="nofollow">data sources</a>...)</td></tr><tr><td>Value</td><td><p>The input value for this parameter.</p><blockquote class="important"><p>Input value can be varied based on&nbsp;<strong>Value Type</strong>. Refer to&nbsp;<a class="external-link" href="/display/KD/Value+Types" rel="nofollow">Value Types in Katalon</a>&nbsp;for more details.</p></blockquote></td></tr></tbody></table>

    For now, enter the URL of Katalon demo AUT ([http://demoaut.katalon.com](http://demoaut.katalon.com)) into the **Value** column then click **OK**.

7. Add the **[Click](/display/KD/%5BWebUI%5D+Click)** keyword. This keyword represents the click action on a given object. Double click on the **Object** cell to provide the object for the keyword.
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-8-18-143A513A0.png)

8. All captured objects in **Object Repository** are displayed in the **Test Object Input** dialog (Refer to [Spy Object](/display/KD/Record+and+Spy+Utilities) for details regarding how to capture objects). Select your object then click **OK**.  
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-6-30-193A143A44.png)

9. Add the **[Verify Element Present](/display/KD/%5BWebUI%5D+Verify+Element+Present)** keyword. This keyword validates if a certain object is displayed on the executing browser. Similar to the previous step, you need to specify the object to be used with this keyword.  
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-8-18-143A543A15.png)
10. Add the **[Close Browser](/display/KD/%5BWebUI%5D+Close+Browser)** keyword and save your test case.  

    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-8-18-143A563A32.png)
11. Click on **Run** in the main toolbar to execute the test case.

    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-8-11-103A573A37.png)

    Katalon Studio should be able to execute all the steps of the sample test case.

### Recent Keywords

**Recent keywords** allow users quickly add any of the last 10 recent used keywords in **Item** list. For example, let's take test case above. To add another **_Verify Element Present_** after _Step 4_, **recent keywords** feature wouldaccomplished this in seconds.

Highlight _Step 4_. Click on **Recent Keywords** and select **_Verify Element Present_**. An extra step is added after _Step 4_ as illustrated below:

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-8-21-123A93A39.png)   ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-8-21-123A133A31.png)

### Recent Objects and Object Folders

Katalon Studio allows users to quickly select recently used **Object** or jump directly to recent used **Object Folder** in Object Repository.

Recent list will have two sections: **Object Folder** and **Test Object**

* **Test Object:** Display the names of the last 5 selected objects
* **Object Folder:** Display the names of 5 folders that contain anyrecent used objects

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/manual-view/image2017-8-25-173A293A39.png)

## In Script View

In addition to the [Manual view](/display/KD/Test+Case+Manual+View), Katalon Studio allows expert users to programmatically write automation test in the Script view of test cases. Users with Groovy/Java background can easily modify the test script as needed.

Given a sample test case with the steps as below:

* _Open the browser_
* _Navigate to a website_
* _Click on certain control_
* _Validate if a control exists on the page_
* _Close the browser_

Follow these steps to automate the above test scenario in **Script view**:

1. Select **File > New > Test Case** from the main menu. The **New Test Case** dialog will be displayed. Provide the name for the new test case, then click **OK**.  
   ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/script-view/image2017-2-15-93A593A10.png)

2. Once a new test case is created, you can switch to the **Script view** using the corresponding tab at the footer of the test case editor. Test steps specified in the **Manual view** are translated into a Groovy script in **Script view**.

   ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/script-view/image2017-6-30-193A243A19.png)

   The import statement in a test script allows referencing to classes to be used. Expand the **import** section to see all default imported classes by Katalon Studio. The name after 'as' in each import statement is an alias for the class. You can change the alias for each class. These classes are necessary for composing a test script.

   Katalon Studio is an automation tool that supports keyword-driven testing. All keywords are grouped into **[WebUI](http://docs.katalon.com/display/KD/Web+UI)**, **[Mobile](http://docs.katalon.com/display/KD/Mobile)** and **[WebService](http://docs.katalon.com/display/KD/Web+Service)** packages accordingly. Press **Ctrl + Space** to view these packages and functions from the imported classes.

3. In this scenario, you will create a Web application test script to make use of the **[Web UI](/x/VQAM) [built-in keywords](/x/VQAM)**. To use a built-in **WebUI** 
    
   ```groovy
   WebUI.
   ```

   The **Content Assist** function will be invoked after users enter the **dot** character. **Content Assist** provides users with a context-sensitive suggestion for code completion. Therefore, all the built-in keywords for WebUI testing will be displayed as below:

   ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/script-view/image2017-6-30-193A253A5.png)

4. After entering the dot character (.), all built-in keywords and their description for Web UI testing will appear as below:

   ![Content Assist Dialog Katalon Studio](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/tutorials/create_test_case_using_script_mode/4.-Content-Assist.png)

5. Select the **[Open Browser](/display/KD/%5BWebUI%5D+Open+Browser)** keyword. This keyword opens a browser and navigates to the specified URL if it is provided. Selected keywords will have their description displayed along for reference.
   ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/script-view/image2017-6-30-193A283A19.png)

6. Enter the **[Navigate To Url](/display/KD/%5BWebUI%5D+Navigate+to+Url)** keyword. This keyword navigates to a specified URL. For now, enter the URL of Katalon Studio ([katalon.com](http://katalon.com)) as the value of the parameter.
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/script-view/image2017-6-30-193A293A21.png)  

7. Enter the **[Click](/display/KD/%5BWebUI%5D+Click)** keyword. This keyword represents the click action on a given object. You need to specify an object for this action.
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/script-view/image2017-6-30-193A293A41.png)  

8. Use the following syntax to refer to an object in **Object Repository** (alternatively, you can drag and drop the object to test case editor to generate the syntax):

    ```groovy
    findTestObject('{Object ID}')
    ```
    
    Where **Object ID** is the ID of that object in Katalon Studio.
    
    > You can find object ID from its Properties dialog. For example:
    > 
    > ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/script-view/image2017-2-15-133A183A7.png)
    
9. Enter the **[Verify Element Present](/display/KD/%5BWebUI%5D+Verify+Element+Present)** keyword. This keyword validates if a certain object is displayed on the executing browser. Similar to the previous step, you need to specify the object to be used with this keyword.

    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/script-view/image2017-2-15-133A263A9.png)

10. Add the **[Close Browser](/display/KD/%5BWebUI%5D+Close+Browser)** keyword and save your test case.

    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/script-view/image2017-2-15-133A273A9.png)

    The following API docs may prove useful when working in Script view:
    
    | Class | Description |
    | --- | --- |
    | **[Builtin Keywords](http://api-docs.katalon.com/studio/v4.6.0.2/api/com/kms/katalon/core/keyword/BuiltinKeywords.html)** | List of common built-in keywords |
    | **[WebUI Builtin Keywords](http://api-docs.katalon.com/studio/v4.6.0.2/api/com/kms/katalon/core/webui/keyword/WebUiBuiltInKeywords.html)** | List of Web UI built-in keywords |
    | **[Web Service Builtin Keywords](http://api-docs.katalon.com/studio/v4.6.0.2/api/com/kms/katalon/core/webservice/keyword/WSBuiltInKeywords.html)** | List of Web Service built-in keywords |
    | **[Mobile Builtin Keywords](http://api-docs.katalon.com/studio/v4.6.0.2/api/com/kms/katalon/core/mobile/keyword/MobileBuiltInKeywords.html)** | List of Mobile built-in keywords |

10. Click on **Run** in the main toolbar to execute the test case.
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/script-view/image2017-8-11-103A563A26.png)

Katalon Studio should be able to execute all the steps of the sample test case.

The test execution results are shown in **Log Viewer** as below:

![Test execution Dialog](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/tutorials/create_test_case_using_script_mode/13b-Katalon-Log-viewer.png)

> Learn more with our Katalon Academy course: [Create and Execute Test Cases](https://academy.katalon.com/courses/create-execute-test-cases/?utm_source=kat_docs_create&utm_medium=bottom_link&utm_campaign=academy_promotion).