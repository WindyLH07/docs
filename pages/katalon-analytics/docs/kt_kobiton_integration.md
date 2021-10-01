---
title: "How to configure Kobiton integration with Katalon TestOps"
sidebar: katalon_studio_docs_sidebar
permalink: katalon-analytics/docs/kt_kobiton_integration.html
---

You can enable Kobiton integration in Katalon TestOps to enhance your real-device testing experiences.

> Requirements:
>
> You have already registered a [Kobiton](https://kobiton.com/) account.

## Integrate Kobiton with Katalon TestOps

Follow these steps:

1. Sign in to [Katalon TestOps](https://testops.katalon.io/login) and go to your Project.
2. Go to **Configurations** > **Integrations**.

    The **Integrations** page appears.
3. Select **Kobiton** in the dropdown list.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-june-schedule-test-runs/schedule-test-run-button.png" width=100% alt="kobiton dropdown">

4. Fill in the required information.

    * **Kobiton Device URL**: enter the URL from your Kobiton Device.
    * **Username**: enter your Kobiton username.
    * **Kobiton's API Key**: enter your 

We can configure Kobiton Integration with Katalon TestOps. First, on the board Katalon Integration, we assign the Kobiton Device URL (1), Username (2), Kobiton's API Key (3). Then, we click the buttons **Test Connection** (4) and **Save** (5).

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/kt_kobiton_integration/kt_kobiton_integration.png)

We must have a Script Repository on Katalon TestOps. Click to a Script Repository.

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/kt_kobiton_integration/kt_script_repo_ex.png)

The Script Repository displays the list of Test Suite Collection. We choose Test Suite Collection, which we want to test.

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/kt_kobiton_integration/kt_open_script_repo.png)

In the board **Test run type**, we choose and type information in the cells (select **Scrip Repository**, **Name**, and **Type** in **Configure Test Run**).

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/kt_kobiton_integration/kt_test_run_type_1.png)

We choose a Test Suite Collection, which we want to run. We choose **Enable Kobiton Integration** and type the ID of the device in **Kobiton Device ID**. We select the **Test Environment Type**.

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/kt_kobiton_integration/kt_test_run_type_2.png)

Choose a Test Environment and a suitable Katalon Studio version.

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/kt_kobiton_integration/kt_test_run_type_3.png)

Click the button Create for creating a Test Run Type.

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/kt_kobiton_integration/kt_test_run_type_4.png)

Start Agent. Running a Test Run with Agent on Katalon TestOps can be seen [here](https://docs.katalon.com/katalon-analytics/docs/agents.html).

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/kt_kobiton_integration/kt_start_agent.png)

A new Test Run Type displays, we click the button Run for running.

![](https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/kt_kobiton_integration/kt_test_plan_run_scrip_repo.png)