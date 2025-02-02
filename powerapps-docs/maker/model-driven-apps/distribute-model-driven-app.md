---
title: "Distribute a model-driven app using a solution | MicrosoftDocs"
description: "Learn how you distribute a model-driven app using solutions"
keywords: ""
ms.date: 08/06/2018
ms.service: powerapps
ms.custom: 
ms.topic: article
applies_to: 
  - "Dynamics 365 (online)"
  - "Dynamics 365 Version 9.x"
  - "powerapps"
ms.assetid: e82e7f64-37ad-41e5-acd7-16309881c6a2
author: "Mattp123"
ms.author: "matp"
manager: "kvivek"
ms.reviewer: 
ms.suite: 
ms.tgt_pltfrm: 
caps.latest.revision: 9
topic-status: Drafting
search.audienceType: 
  - maker
search.app: 
  - PowerApps
  - D365CE
---

# Distribute a model-driven app using a solution

Model-driven apps are distributed as solution components. After you have created a model-driven app, you can make it available for other environments to use by packaging the app into a solution and then exporting it into a zip file. After the solution (.zip file) is successfully imported in the target environment, the packaged app is available for use. 
  
## Add an app to a solution
In order to distribute your app, you create a solution so the app can be packaged for export.

1. Sign in to [PowerApps](https://make.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc).

2. Select **Solutions** and then select **New solution**.
3. Complete the fields on the **New Solution** page, and then select **Save**. More information: [Create a solution](../common-data-service/create-solution.md)
4. The **Solution** page appears. Select **Add Existing**, select **App**, select the app that you want to add to the solution, and then select **OK**. 

    ![Select solution components](media/select-solution-components.png)

5. If a **Missing Required Components** page appears we recommend that you select **Yes, include required components** to add necessary components such as entities, views, forms, charts, and site map that are part of the app. Select **OK**.
6. On the **Solution** page select **Save and Close**.

## Export a solution
To distribute your app so it can be imported into other environment or made available on [Microsoft AppSource](https://appsource.microsoft.com/), you export the solution to a zip file. Then, the zip file that contains the app and components can be imported into other environments.

1. Open the [Solutions page](advanced-navigation.md#solutions). 
2. Select the solution you want to export, and then on the toolbar select **Export**. 
3. On the **Publish Customizations** page, select **Next**.
4. If the **Missing Required Components** page appears, select **Next**. 
5. On the **Export System Settings** page, select the optional features that you want to include, and then select **Next**. 
6. On the **Package Type** page, select **Unmanaged** or **Managed**, and the select **Export**. For more information about solution package types, see [Solutions overview](../common-data-service/solutions-overview.md).
7. Depending on your browser and settings, a .zip package file is built and copied to the default downloads folder. The file name of the package is based on the unique name of the solution appended with underscores and the solution version number.

	> [!NOTE]
	> When you export an app by using a solution, the app URL is not exported.
  
## Import a solution  
When you receive a solution zip file which contains the app that you want to import, open the solutions component page and import the solution. When the solution has been successfully imported, the app will be available in your environment.

1. Sign in to [PowerApps](https://make.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc).

2. Select **Solutions** and then on the toolbar select **Import**.
3. Browse to the file you want to import, and then choose **Next**.
4. Select **Import**.

## See also
[Change the solution publisher prefix](../common-data-service/change-solution-publisher-prefix.md)
