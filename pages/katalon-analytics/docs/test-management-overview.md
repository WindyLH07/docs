---
title: "Test Management Overview"
sidebar: katalon_studio_docs_sidebar
permalink: katalon-analytics/docs/test-mgt-overview.html
redirect_from:
---

Test Management allows you to monitor test analytics for your projects.

You can also leverage it to gain critical insights into test results and integrate seamlessly with Katalon Studio and Jira for more efficient project management.

## Requirements

A requirement represents the Jira issue that is linked to a test case.

> Notes:
>
> You can link a test case to a Jira issue by following this guide: [Link Test Cases to Jira Requirements](https://docs.katalon.com/katalon-analytics/docs/ka-integration-jira.html).

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-ka-integration-jira/test-mgt-overview.png"  width=100% alt="requirement page">

On the **Requirements** page, you can check the following information:

* The total number of requirements (Jira issues and BDD Features).

    > Notes:
    > In Katalon TestOps, BDD Features are displayed as Requirements and BDD Scenarios are displayed as Test Cases. See: [View BDD Test Results](https://docs.katalon.com/katalon-analytics/docs/bdd-test-results.html).
    
* Reports on Test Run Coverage and Traceability Matrix.
    
    * The **Test Run Coverage** tab will show you the number of test cases, test runs and failures that belongs to a requirement.

    * The **Traceability Matrix** tab will show you a list of requirements, with their test cases, test results and defects.
    
* The list of all requirements in details.

## Test Cases

On the **Test Cases** page, you can check the following information:

* The total number of test cases (including both the passed and failed ones).
* Reports on test flakiness and Platform Coverage.

    * The **Flaky** tab will show you the most unreliable test cases.
    * The **Platform Coverage** tab will show you test case quality based on Operating System (OP) and browsers.

* The list of all test cases in details.

## Test Suites

On the **Test Suites** page, you can check the following information:
* The total number of test suites (including both the passed and failed ones).
* The list of all test suites in details.

## Defects

On the **Defects** page, you can see the list of all Jira bugs in details.

> Notes:
>
> You can link a test result to a Jira bug by following this guide: [Defects](https://docs.katalon.com/katalon-analytics/docs/ka-defects.html).