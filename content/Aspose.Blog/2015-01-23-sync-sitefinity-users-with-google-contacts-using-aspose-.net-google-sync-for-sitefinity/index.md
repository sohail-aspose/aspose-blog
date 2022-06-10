---
title: 'Sync Sitefinity Users with Google Contacts using Aspose .NET Google Sync for Sitefinity'
date: Fri, 23 Jan 2015 10:14:59 +0000
draft: false
url: /2015/01/23/sync-sitefinity-users-with-google-contacts-using-aspose-.net-google-sync-for-sitefinity/
author: Zaheer Tariq
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![Aspose.Email for .NET][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/aspose-Email-for-net_100.png)Sitefinity Google Sync is an open source add-on from [Aspose][2] that links your Sitefinity users to Google/Gmail contacts without requiring any other software. It uses powerful features of [Aspose.Email for .NET][3] to allow you to easily sync your Google contacts and Sitefinity users.

This initial version of the module is enriched with the following features to make the sync process effective, simple and easy to use.

*   Google/Gmail server credentials are encrypted and saved in the database so that you don’t have to enter them every time you use the module.
*   Sync all or selected Gmail contacts to Google and vice versa.
*   Option to select one or more Sitefinity user when performing Google/Gmail to Sitefinity sync.
*   Existence of every contact/user in the destination system is checked before migration to make sure that the sync does not create duplicate records.
*   The contacts migrated to Google/Gmail are put in Other Contacts group so that you can verify and move only required ones to My Contacts.
*   A brief summary of the sync process is shown upon completion.

\[caption id="attachment\_19628" align="aligncenter" width="300" caption="Aspose .NET Google Sync for Sitefinity"\][![Aspose .NET Google Sync for Sitefinity][4]](https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Aspose-.NET-Google-Sync-for-Sitefinity.png)\[/caption\] \[caption id="attachment\_19629" align="aligncenter" width="300" caption="Google to Sitefinity Sync"\][![Google to Sitefinity Sync][5]](https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Google-to-Sitefinity-Sync.png)\[/caption\] \[caption id="attachment\_19630" align="aligncenter" width="300" caption="Sitefinity to Google Sync"\][][6]\[/caption\]

## System Requirements

In order to setup Aspose .NET Google Sync for Sitefinity add-on you need to have the following requirements met:

*   Sitefinity CMS running on ASP.NET 4.0

Please feel free to contact us if you have any issues setting up this Sitefinity Add-on.

## Installing and Configuring the Aspose .NET Google Sync for Sitefinity Add-on

You can download the Aspose .NET Google Sync for Sitefinity add-on from one of the following locations:

*   Download from [CodePlex][7]
*   Download from [GitHub][8]

Once downloaded, please follow these steps to install the Add-on into your Sitefinity website:

**Step 1: Copy files to your Sitefinity installation**

Please extract the downloaded ZIP file. You will need FTP or direct access to the Sitefinity installation folder on the server to perform the following:

1.  Copy Aspose.Email.dll and Aspose.SiteFinity.GoogleSync.dll into the **bin** folder of the Sitefinity installation.
2.  Copy the **Addons** folder on the root of the Sitefinity installation where the **bin** folder is located.

**Step 2: Register the Aspose .NET Google Sync for Sitefinity add-on in Sitefinity**

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
    2.  Add ~/Addons/AsposeGoogleSync/AsposeGoogleSync.ascx in the **Control CLR Type or Virtual Path** field.
    3.  Add **Name**, **Title** and **Description** as follows:  
        AsposeGoogleSync  
        Aspose Google Sync  
        Sync Sitefinity Users with Google Contacts using Aspose .NET Google Sync for Sitefinity
    4.  You may leave all other fields as they are.
7.  When finished, click **Save changes**.  
    The widget is registered in the toolbox and can be used in Sitefinity. The settings are also shown in the picture below

\[caption id="attachment\_19627" align="aligncenter" width="282" caption="Registering Aspose .NET Google Sync for Sitefinity Add-on in Sitefinity"\][![Registering Aspose .NET Google Sync for Sitefinity Add-on in Sitefinity][10]](https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/How-to-register-Aspose-.NET-Google-Sync-for-Sitefinity.png)\[/caption\]

## Using the Aspose .NET Google Sync for Sitefinity Add-on

After you have installed and configured the Aspose .NET Google Sync for Sitefinity add-on it is really simple to start using it on your website. Please follow these simple steps to get started:

1.  Make sure you are logged-in to Sitefinity with an Administrator level account.
2.  Navigate to the page where you want to add the Google Sync add-on. Make sure the page is opened in edit mode.
3.  From the **Drag Widgets** menu on the right, select Aspose Google Sync and drag it into position.

\[caption id="attachment\_19626" align="aligncenter" width="300" caption="Using Sitefinity Google Sync Add-on"\][][11]\[/caption\]

You have successfully installed and added Aspose .NET Google Sync for Sitefinity Module to your page. You will be presented with three simple options to get started

*   Google to Sitefinity Sync
*   Sitefinity to Google Sync
*   Google Settings

You will asked to enter Google Server details when clicking on any option for the first time. A simple form takes all the required details to connect to your Google account and then these details will be encrypted and saved in the database for later use.

[](https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Google-server-details.png)Once the sync process is completed, a brief summary of migrated records count and list of records that already existed and are not imported is shown.

## Video

Please check [this video][12] to see it in action.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/aspose-Email-for-net_100.png "aspose-Email-for-net_100"
[2]: http://www.aspose.com/
[3]: https://products.aspose.com/email
[4]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Aspose-.NET-Google-Sync-for-Sitefinity-300x87.png "Aspose .NET Google Sync for Sitefinity"
[5]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Google-to-Sitefinity-Sync-300x250.png "Google to Sitefinity Sync"
[6]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Sitefinity-to-Google-Sync.png
[7]: https://docs.aspose.com/
[8]: https://github.com/asposemarketplace/Aspose_for_Sitefinity/releases
[9]: http://www.mywebsite.com/sitefinity
[10]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/How-to-register-Aspose-.NET-Google-Sync-for-Sitefinity-282x300.png "Registering Aspose .NET Google Sync for Sitefinity Add-on in Sitefinity"
[11]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/01/Using-Aspose-.NET-Google-Sync-for-Sitefinity.png
[12]: https://www.youtube.com/watch?v=N3Vv4Bh84Zw




