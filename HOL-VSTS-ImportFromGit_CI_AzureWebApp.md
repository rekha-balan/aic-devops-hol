# Setting up existing GitHub Repo in VSTS

## Step 1 : Connect to GitHub

![Import From GitHub](https://swaminathanvetri.blob.core.windows.net/aic-images/VSTS-ImportFromGit.png)

### Once import is complete, it will show up the below page and take you to the repository's landing page

![](https://swaminathanvetri.blob.core.windows.net/aic-images/VSTS-ImportSuccessful.png)

## Step 2 : Create a build definition

To create a new build for the recently imported code base click on the **Set up Build** on the right corner

![Set up Build](https://swaminathanvetri.blob.core.windows.net/aic-images/VSTS-SetupBuild.png)

## Step 2.1 : Choose the template

Choose the appropriate template for the type of project you have selected. The project which was imported fro GitHub was an asp.net core codebase. So, select Azure App Service template from the list

## Step 2.2 Modify the build tasks

Once the Azure App Service template is chosen, you should be seeing the below set of tasks with the Process tab highlighted 

![Build Process](https://swaminathanvetri.blob.core.windows.net/aic-images/VSTS-Build-Process.png)

* Provide values for **Name**
* Choose **Hosted Agent** for Agent-queue
* Provide values for **Azure Subscription**
* Provide values for **App Service Name**

The build tasks that are available as a part of this template are listed below.

![Build tasks](https://swaminathanvetri.blob.core.windows.net/aic-images/VSTS-Build-Tasks.png)

## Step 2.3 Update the Run on Agents settings

Specify the agent settings on which the build task should run 

![Run on Agent](https://swaminathanvetri.blob.core.windows.net/aic-images/VSTS-Build-RunOnAgent.png)

## Step 2.4 Check the sources for build

Choose the appropriate version control system from where the source code needs to be downloaded from

![Get Sources](https://swaminathanvetri.blob.core.windows.net/aic-images/VSTS-Build-GetSources.png)

## Step 2.5 Enable Continuous Integration

Click on the **Triggers** tab and Check mark the Enable Continuous Integration and choose the appropriate branch

![Enable CI](https://swaminathanvetri.blob.core.windows.net/aic-images/VSTS-Build-EnableCI.png)

## Step 2.6 Save and Queue the build

![Queue the Build](https://swaminathanvetri.blob.core.windows.net/aic-images/VSTS-Build-SavenQueue.png)

![Build Queued](https://swaminathanvetri.blob.core.windows.net/aic-images/VSTS-BuildQueued.png)