---
title: "Upload Test Results to Katalon TestOps from Katalon Studio" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/katalon-analytics-beta-integration.html
redirect_from:
    - "/display/KD/Katalon+Analytics+%28Beta%29+Integration/"
    - "/display/KD/Katalon%20Analytics%20%28Beta%29%20Integration/"
    - "/x/KRhO/"
    - "/display/KA/Integration+with+Katalon+Studio/"
    - "/display/KA/Integration%20with%20Katalon%20Studio/"
    - "/katalon-analytics/docs/ka-integration-katalon-studio/"
    - "/katalon-analytics/docs/ka-integration-katalon-studio.html"
    - "/katalon-analytics/docs/view-reports/"
    - "/x/mw3R/"
    - "/katalon-analytics/docs/integration-with-katalon-studio.html"
    - "/katalon-analytics/docs/upload-reports-overview.html"
    - "/katalon-analytics/docs/project-management-import-KS.html"
    - "/katalon-analytics/docs/ks_upload_project_kt.html"
---

> Notes:
> * Katalon Studio version 7.0 onwards supports video capture of Test Results when uploading them to Katalon TestOps.

From Katalon Studio, you can upload Test Results to Katalon TestOps manually or automatically.

## Upload Test Results automatically

Follow these steps:

1. Open Katalon Studio.

2. Go to **Project** > **Settings** > **Katalon TestOps**.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-test-uploads-to-kto-from-ks/KS-TESTOPS-Integration.png"  width=100% alt="ks project setting testops integration">

    Alternatively, you can also click **TestOps** icon from the main toolbar to navigate to the TestOps settings.

    <img src="url"  width=100% alt="TestOps icon">

3. Tick on the **Enable Katalon TestOps Integration** checkbox.

    Wait for Katalon Studio to connect to Katalon TestOps.
    
    Once the connection is successful, Katalon Studio retrieves all Teams and Projects from the Organization you belong to.
    
4. Choose your Team and Project in a dropdown menu of the **Team** and **Project** sections.

    If you are the Owner or Admin, you can also click **New Project** to create a new Project instead.

5. Click **Apply and Close**.

Once you have enabled Katalon TestOps integration in Katalon Studio, your Test Results are automatically uploaded to Katalon TestOps every time you run Test Suites in Katalon Studio.
    
<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-test-uploads-to-kto-from-ks/KS-TESTOPS-Upload-results-automatically.png"  width=100% alt="automatic upload of test reports to kto">

## Upload Test Results manually

You can also upload Test Results manually by following these steps:

1. Open Katalon Studio and go to the Project you are working on.

2. Go to **Test Suites** or **Test Suite Collection** and choose your Test Suite.

    Select the **Result** tab.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-test-uploads-to-kto-from-ks/KS-TESTOPS-Upload-result-manually.png" width=100% alt="upload manually from ks to testops">

3. Click on the **Katalon TestOps** tab at the top right corner and select **Upload**.

4. Choose the Team and Project you want to upload Test Results to.

5. Click **Upload**.

You have uploaded Test Results manually to Katalon Testops.

## Switch Organization in Katalon Studio

You can switch to a different Organization in Katalon Studio by following these steps:

1. Open Katalon Studio and click on the *Profile* icon at the top right corner.

    <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-test-uploads-to-kto-from-ks/KS-TESTOPS-Profile-icon.png" width=100% alt="switch organization in ks">

2. Select **Log out**.

    The **Katalon Studio Activation** box displays.
    
3. Type the new email address and password, then click **Activate**.

You have logged in to a different Organization.

To verify that you have overridden the authentication successfully, click on the *Profile* icon again and select **View Dashboard**.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-july-test-uploads-to-kto-from-ks/KS-TESTOPS-View-dashboard.png" width=100% alt="view dashboard button in ks">

You will be navigated to the new Organization in Katalon TestOps.
