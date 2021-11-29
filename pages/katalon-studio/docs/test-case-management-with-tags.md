---
title: "Test Case Management With Tags" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/test-case-management-with-tags.html

description: 
---

To manage test cases better in Katalon Studio, you can manipulate tag properties by utilizing the existing tag values. You can also view all tags in the project and save your time by appending existing tags to test cases.

This document shows you how to append and manage tags, search for test cases with multiple tags, and execute test cases with certain tags in console mode.

## Append and Manage Tags

To append and manage tags, do as follows:

1. Open your desired test case.
2. Switch to the **Properties** tab. In this tab, you can find detailed information of a test case, including all tags.
3. Input your tag values, separate them by commas or semi-colons.

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-case-management-with-tags/Tags_3.png)

In case the tag properties have already had value, the tag token will be automatically separated by colons and semi-colons.
Open a test case > Properties > Click Manage Tags > select tags to append > click Append Tags

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-case-management-with-tags/Tags_4.png)

Please note that the existing tags cannot be removed by unchecking the boxes, this feature is just for appending tags to test cases.


**Search For Test Cases With Multiple Tags**

This feature will be enabled in Query Provider of Dynamic Querying Test Suite after you successfully install Test Case Management With Tags plugins.

To search for test artifacts labeled with Multiple Tags, directly type on the search box follow this syntax: Tags = (NameOfTag1, NameOfTag2)

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/test-case-management-with-tags/tags-search.png)

**Execute Test Cases With Certain Tags in Console Mode**

You can execute only the Test Cases with the `<tag1>` and `<tag2>` tags in a Test Suite by including the argument `testCaseTags="<tag1>,<tag2>"` in your command.

Assuming that the Test Suite being executed has three Test Cases, below is an example:
```
----------------- TEST CASE TAGS PLUGIN START FILTERING -----------------
Test Cases/Test Case with both <tag 1> and <tag 2> are to be run
Test Case/Test Case with only <tag 1> is filftered out
Test Case/Test Case with only <tag 2> is filtered out
----------------- TEST CASE TAGS PLUGIN FINISH FILTERING -----------------
```

