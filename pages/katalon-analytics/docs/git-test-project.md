---
title: "Upload Test Scripts from a Git Repository" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-analytics/docs/git-test-project.html 
description: 
---

You can create a Git Script Repository in Katalon TestOps. By doing so, you can store your Test Scripts in Git and execute them in Katalon TestOps, because Katalon TestOps upload Test Scripts automatically from a Git Repository.

You do not have to upload Test Scripts manually to TestOps Projects.

## Create Git Script Repository

Follow these steps:

1. Sign in to [Katalon TestOps]( https://testops.katalon.io/login) and go to the Project you want to create a Git Repository for.

   Go to **Configurations** > **Script Repositories**.
   
   The **Script Repositories** page appears as below.

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-june-git-test-project/script-repo-screen-in-testops-config-new.png" width=100%>

2. Click **Create Git Script Repository**.

3. Fill in the required information.

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-june-git-test-project/scrip-repo-page-after-creating-git-repo.png" width=100%>

   * **Source Type**: choose **Github**.
   * **Repository URL**: enter your Git Repository. For example, https://github.com/katalon-studio-samples/ci-samples.
   * **Username**: enter your Git Username.
   * **Personal Access Token**: enter your Personal Access Token.
   
      > Notes:
      >
      > You can create an individual access token in GitHub.
      >
      > See: [Create a Personal Access Token](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line).
      >
      > Follow the instruction and make sure you choose **repo** in the **Select scopes** section in the **New personal access token** page.
      <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-june-git-test-project/new-personal-access-toke-page-git.png" width=100%>

4. Click **Connect**.

   Additional sections appear as below.

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-analytics/docs/testops-revamp-june-git-test-project/script-repo-page-after-clicking-connect.png" width=100%>

   * **Branch**: choose a branch.
   * **Name**: enter your Project’s name.

5. Click **Create**.

You have created a new Git Script Repository.

See also:
* [Set up Configurations for Remote Execution](https://docs.katalon.com/katalon-analytics/docs/test-run-config.html).

* [Upload Test Scripts to a Script Repository](https://docs.katalon.com/katalon-analytics/docs/code-repo.html#upload-a-zip-file-to-a-script-repository).

* [Schedule Test Runs](https://docs.katalon.com/katalon-analytics/docs/create-plan.html).

 * [Execute Test Runs by a Trigger](https://docs.katalon.com/katalon-analytics/docs/kt-scheduler.html).