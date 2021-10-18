---
title: "Spy Web Utility" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/spy-web-utility.html 
redirect_from:
    - "/display/KD/Spy+Web+Utility/"
    - "/display/KD/Spy%20Web%20Utility/"
    - "/x/5BZO/"
    - "/katalon-studio/docs/spy-web-utility/"
    - "/x/jwBO/"
    - "/katalon-studio/docs/spy-web-utility-version-48-and-below/"
    - "/katalon-studio/docs/spy-web-utility-version-48-and-below.html"
description: 
---

Enhanced Spy Web Utility is more compact and more intelligent for capturing objects. You can specify Object properties and locating methods. The built-in **Verify and Highlight** feature assures that Katalon Studio can identify the objects. Spy Web Utility window can be **pinned** or **unpinned** for users' convenience while spying.

This guide will show step-by-step how to use Spy Web Utility.

Capture objects using Spy Web Utility
------------------------------------

1.  Click on **Spy Web** from the main toolbar.  
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/spy-web-utility/image2017-2-23-133A203A14.png)  
      
    
2.  The **Object Spy** dialog will be displayed.  
      
    
3.  Click on **Start** to begin capturing objects from the web browser.
    
    <table><thead><tr><th>Type</th><th>Description</th><th>Note</th></tr></thead><tbody><tr><td>New Browsers</td><td>Start a new browser and start spying web objects from that browser.</td><td><strong>Supported browsers:</strong><br>- Firefox<br>- Chrome<br>- Internet Explorer (only on Windows)</td></tr><tr><td>Active Browsers</td><td>Focus on <strong>the current active Chrome browser</strong> and start spying web objects from it.</td><td>Katalon Studio will install <a class="external-link" href="https://chrome.google.com/webstore/detail/katalon-recorder-selenium/ljdobmomdgdljniojadhoplhkpialdid" rel="nofollow">Katalon Recorder</a> as an add-on to help with recording for this type of browser<br><br><strong>Supported browsers:</strong><br>- Chrome<br>- Firefox (coming soon)<p>You will be asked for installation of <em>Katalon Utility</em>:</p><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/spy-web-utility/image2017-2-23-113A543A29.png"></p><p>Refer to <a href="/display/KD/Katalon+Addon+for+Chrome">Katalon Addon for Chrome</a> for more details.</p></td></tr></tbody></table>
    
4. Katalon Studio will launch the selected browser. Navigate to your website, then hover the **mouse cursor** over the web object to be captured.  
    Web Utility will highlight the web object with a **red border**. An **overlay pane** will also be displayed at the edge of the screen to show relevant **XPath** info.  
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/spy-web-utility/image2016-12-29-163A553A52.png)  
      
    
5.  Press the combination of **<Alt + back quote>** keys on the keyboard to capture the object. The object will be highlighted with the **green border**.   
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/spy-web-utility/image2016-12-29-173A43A7.png)  
      
    
6.  Captured objects will appear in the **Object Spy** dialog.  
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/spy-web-utility/image2018-9-5-183A13A21.png)  
      
    
7.  Select the object in the **Captured Objects** tree, its details will be displayed in the **Object Properties** section.   
> Learn more about [Selection Method](https://docs.katalon.com/katalon-studio/docs/working-with-objects-selection-method-for-spyrecord-web.html).
    
<table>
   <thead>
      <tr>
         <th>Field</th>
         <th>Description</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td><strong>Selection Method</strong></td>
         <td>
            <p>The method which Katalon Studio will be using to detect web elements.</p>
            <table>
               <thead>
                  <tr>
                     <th>Options</th>
                     <th>&nbsp;</th>
                  </tr>
               </thead>
               <tbody>
                  <tr>
                     <td><strong>Attributes</strong></td>
                     <td>Katalon Studio automatically generate an XPath combine with objects' properties.</td>
                  </tr>
                  <tr>
                     <td><strong>XPath</strong></td>
                     <td>Katalon Studio <strong>Relative XPath</strong>. If an element cannot be consistently located using its direct attributes, Katalon Studio will identify by using its more robust neighbors.</td>
                  </tr>
                  <tr>
                     <td><strong>CSS</strong></td>
                     <td>Users are allowed to input CSS selector manually into Object Detect Editor.</td>
                  </tr>
               </tbody>
            </table>
         </td>
      </tr>
      <tr>
         <td><strong>Properties Grid</strong></td>
         <td>All the captured properties of the selected object. You can edit the value of any property.</td>
      </tr>
      <tr>
         <td><strong>Selector Editor</strong></td>
         <td>
            <p>Display object locator based on <strong>selected</strong> <strong>method</strong></p>
            <table>
               <thead>
                  <tr>
                     <th>Options</th>
                     <th>&nbsp;</th>
                  </tr>
               </thead>
               <tbody>
                  <tr>
                     <td><strong>Basic </strong>or<strong> XPath</strong></td>
                     <td>Katalon Studio generated XPath will be displayed.</td>
                  </tr>
                  <tr>
                     <td><strong>CSS</strong></td>
                     <td>Editable text field allows users to manually input object's locator.</td>
                  </tr>
               </tbody>
            </table>
         </td>
      </tr>
   </tbody>
</table>
    
For more information on WebUI test objects, click [here](/x/tQTR). 
    
8.  Click on **Save** to add those objects to **Object Repository**.  

9.  Check on those captured objects in the **left pane** that you would like to save into Katalon Studio.   
    The structure of your **Object Repository** is displayed on the **right pane**. Select the folder to add the captured objects into. Click **OK** when done.  
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/spy-web-utility/image2016-12-29-173A153A54.png)  
      
    
10.  The captured objects will be added to **Object Repository** accordingly.

Define additional objects manually
----------------------------------

> The **name** of the manually added **element** is generated automatically by Katalon Studio.

1.  **Add a Page element**: Web objects need a web page to hold it. Click on **New page** from the toolbar to add a new Page element manually.  
      
    
2.  **Add a Frame element**: If the new object is a nested object, a frame is needed to locate the element. Frames are web elements that usually contain many other web objects. 
    
    Click on **New frame** from toolbar to manually add a new Frame element.  
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/spy-web-utility/image2018-9-5-183A103A53.png)
    
3.  **Add an Object element**: Click on the **New object** from the toolbar to manually add a web object. Click **Delete** to remove any unwanted element.   
      
    
4.  In Object Properties section, provide **Object Name** for the recently added object, choose **Selection Method** options and specify **properties** for the _New_ web object.
    
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/spy-web-utility/image2018-9-5-183A133A52.png)  
      
    
5.  Click **Verify and Highlight** to make sure the object can be located by Katalon Studio.
    If there is a web object with matched **Selector Editor** value, it will be highlighted **red** in opened browser and message **"Found X element using XPath Selector"** will be displayed.
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/spy-web-utility/image2018-9-5-183A133A16.png)  
      
    
6.  Once finished, click **Save** to add object to **Object Repository** as normal.
    

How to get web objects XPath or CSS Locator
-------------------------------------------

1.  In active opened spying browser, **Right** click on target web element. Select **Inspect**  
    **![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/spy-web-utility/image2017-10-16-133A263A34.png)**  
      
    
2.  An element **inspector window** will be displayed on the right with highlighted line which indicates the location of the target element in the HTML DOM. **Right** click on the hightlighted line > Select **Copy** \> Choose **Copy XPath** or **Copy Selector**  
    ![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/spy-web-utility/image2017-10-16-133A363A58.png)  
      
    
3.  Navigate back to _Object Spy_ window and paste into _CSS Selector Editor_ or _Object Properties Grid_.   
      
    
4.  Click Verify and Hightlight button to check if Katalon Studio can locate the object.  
      
    
5.  Once finished, click **Save** to add object to **Object Repository** as normal.

**See also**

> * [Working with Object Properties](https://docs.katalon.com/katalon-studio/docs/manage-web-test-object.html)
> * [Object Identification Best Practices](https://docs.katalon.com/katalon-studio/docs/optimizing-object-identification-and-tools.html)
> * [Configure Web Object Locators Settings](https://docs.katalon.com/katalon-studio/docs/web-locators-settings-since-v571.html)