---
title: 'Sync Sitefinity Users with Microsoft Exchange Contacts using Aspose .NET Exchange Sync for Sitefinity'
date: Tue, 06 Jan 2015 13:39:37 +0000
draft: false
url: /2015/01/06/sync-sitefinity-users-with-microsoft-exchange-contacts-using-aspose-.net-exchange-sync-for-sitefinity/
author: Zaheer Tariq
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![Aspose.Email for .NET][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/aspose-Email-for-net_100.png)Sitefinity Exchange Sync is an open source add-on from [Aspose][2] that links your Sitefinity users to Microsoft Exchange Server contacts without requiring any other software. It uses powerful features of [Aspose.Email for .NET][3] to allow you to easily sync your Exchange contacts and Sitefinity users.

This initial version of the add-on is enriched with the following features to make the sync process effective, simple and easy to use.

*   Exchange server credentials are encrypted and saved in database so that you don’t have to enter them every time you use this add-on.
*   Sync all or selected Exchange contacts to Sitefinity and vice versa.
*   Option to select one or more Sitefinity roles when performing Exchange to Sitefinity sync.
*   Existence of every contact/user in the destination system is checked before migration to make sure that the sync does not create duplicate records.
*   A brief summary of the sync process is shown upon completion.

\[caption id="attachment\_19313" align="aligncenter" width="300" caption="Aspose .NET Exchange Sync for Sitefinity"\][![Aspose .NET Exchange Sync for Sitefinity][4]](https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Aspose-.NET-Exchange-Sync-for-Sitefinity.png)\[/caption\] \[caption id="attachment\_19314" align="aligncenter" width="300" caption="Exchange to Sitefinity Sync"\][![Exchange to Sitefinity Sync][5]](https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Exchange-to-Sitefinity-Sync.png)\[/caption\] \[caption id="attachment\_19315" align="aligncenter" width="300" caption="Sitefinity to Exchange Sync"\][][6]\[/caption\]

## System Requirements

In order to setup Aspose .NET Exchange Sync for Sitefinity add-on you need to have the following requirements met:

*   Sitefinity CMS running on ASP.NET 4.0

Please feel free to contact us if you have any issues setting up this Sitefinity Add-on.

## Installing and Configuring the Aspose .NET Exchange Sync for Sitefinity Add-on

You can download the Aspose .NET Exchange Sync for Sitefinity add-on from one of the following locations:

*   Download from [CodePlex][7]
*   Download from [GitHub][8]

Once downloaded, please follow these steps to install the Add-on into your Sitefinity website:

**Step 1: Copy files to your Sitefinity installation**

Please extract the downloaded ZIP file. You will need FTP or direct access to the Sitefinity installation folder on the server to perform the following:

1.  Copy Aspose.Email.dll and Aspose.SiteFinity.ExchangeSync.dll into the **bin** folder of the Sitefinity installation.
2.  Copy the **Addons** folder on the root of the Sitefinity installation where the **bin** folder is located.

**Step 2: Register the Aspose .NET Exchange Sync for Sitefinity add-on in Sitefinity**

1.  Log into your Sitefinity CMS with an ‘**Administrator**’ account. The login page can be reached by [http://www.mywebsite.com/sitefinity][9]
2.  Click **Administration** and then **Settings**.  
    The Basic Settings page appears.
3.  **Click the Advanced  link.  
    **The Settings  page appears.
4.  In the left pane, click **Toolboxes**  followed by **Toolboxes**, then **PageControls**, **Sections** and **ContentToolboxSection**, then **Tools.**
5.  Click **Create new**.  
    The widget registration form appears.
6.  Fill the form fields as follows:
    1.  Make sure **Enabled** is selected.
    2.  Add ~/Addons/AsposeExchangeSync/AsposeExchangeSync.ascx in the **Control CLR Type or Virtual Path** field.
    3.  Add **Name**, **Title** and **Description** as follows:  
        AsposeExchangeSync  
        Aspose Exchange Sync  
        Sync Sitefinity Users with Microsoft Exchange Contacts using Aspose .NET Exchange Sync for Sitefinity
    4.  You may leave all other fields as they are.
7.  When finished, click **Save changes**.  
    The widget is registered in the toolbox and can be used in Sitefinity. The settings are also shown in the picture below

\[caption id="attachment\_19312" align="aligncenter" width="287" caption="Registering Aspose .NET Exchange Sync for Sitefinity Add-on in Sitefinity"\][![Registering Aspose .NET Exchange Sync for Sitefinity Add-on in Sitefinity][10]](https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/How-to-use-Aspose-.NET-Exchange-Sync-for-Sitefinity.png)\[/caption\]

## Using the Aspose .NET Exchange Sync for Sitefinity Add-on

After you have installed and configured the Aspose .NET Exchange Sync for Sitefinity add-on it is really simple to start using it on your website. Please follow these simple steps to get started:

1.  Make sure you are logged-in to Sitefinity with an Administrator level account.
2.  Navigate to the page where you want to add the Exchange Sync add-on. Make sure the page is opened in edit mode.
3.  From the **Drag Widgets** menu on the right, select Aspose Exchange Sync and drag it into position.

[](https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Using-Aspose-.NET-Exchange-Sync-for-Sitefinity.png)You have successfully installed and added Aspose .NET Exchange Sync for Sitefinity add-on to your page. You will be presented with three simple options to get started

*   Exchange to Sitefinity Sync
*   Sitefinity to Exchange Sync
*   Exchange Settings

You will asked to enter Exchange Server details when clicking on any option for the first time. A simple form takes all the required details to connect to your Exchange account and then these details will be encrypted and saved in the database for later use.

[](https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Exchange-server-details.png)Once the sync process is completed, a brief summary of migrated records count and list of records that already existed and are not imported is shown.

## Video

Please check [this video][11] to see it in action.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/aspose-Email-for-net_100.png "aspose-Email-for-net_100"
[2]: http://www.aspose.com/
[3]: https://products.aspose.com/email
[4]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Aspose-.NET-Exchange-Sync-for-Sitefinity-300x85.png "Aspose .NET Exchange Sync for Sitefinity"
[5]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Exchange-to-Sitefinity-Sync-300x221.png "Exchange to Sitefinity Sync"
[6]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Sitefinity-to-Exchange-Sync.png
[7]: https://docs.aspose.com/
[8]: https://github.com/asposemarketplace/Aspose_for_Sitefinity/releases
[9]: http://www.mywebsite.com/sitefinity
[10]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/How-to-use-Aspose-.NET-Exchange-Sync-for-Sitefinity-287x300.png "How to use Aspose .NET Exchange Sync for Sitefinity"
[11]: https://www.youtube.com/watch?v=56Zqc7SghEE




