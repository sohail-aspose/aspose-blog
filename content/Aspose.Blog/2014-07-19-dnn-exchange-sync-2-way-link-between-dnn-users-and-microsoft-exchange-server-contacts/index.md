---
title: 'DNN Exchange Sync – 2 Way Link between DNN Users and Microsoft Exchange Server Contacts'
date: Sat, 19 Jul 2014 12:55:03 +0000
draft: false
url: /2014/07/19/dnn-exchange-sync-2-way-link-between-dnn-users-and-microsoft-exchange-server-contacts/
author: Zaheer Tariq
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![aspose Email for net 100 Reading Named Properties from Message Attachments Supported by Aspose.Email for .NET 4.3.0][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/aspose-Email-for-net_100.png)DNN Exchange Sync is an open source module from [Aspose][2] that links your DNN users to Microsoft Exchange Server contacts without requiring any other software. It uses powerful features of [Aspose.Email for .NET][3] to allow you to easily sync your Exchange contacts and DNN users. The contact details from Exchange server and DNN user profile are smartly mapped so that all the information associated with a DNN user or Exchange contact is migrated properly from one system to the other.

This initial version of the module is enriched with the following cool features to make the sync process simple and easy to use.

*   Exchange server credentials are encrypted and saved in database so that you don't have to enter them every time you use this module.
*   Sync all or selected Exchange contacts to DNN and vice versa.
*   Option to select one or more DNN roles when performing Exchange to DNN sync.
*   Existence of every contact/user in the destination system is checked before migration to make sure that the sync does not create duplicate records.
*   A brief summary of the sync process is shown upon completion.

\[caption id="attachment\_15722" align="aligncenter" width="300" caption="DNN Exchange Sync Module"\][][4]\[/caption\] \[caption id="attachment\_15723" align="aligncenter" width="300" caption="Exchange to DNN Sync"\][][5]\[/caption\] \[caption id="attachment\_15724" align="aligncenter" width="300" caption="DNN to Microsoft Exchange Server Sync"\][][6]\[/caption\]

## Installing the DNN Exchange Sync Module

You can download the DNN Exchange Sync module from one of the following locations:

*   Download from [CodePlex][7]
*   Download from [DNN Store][8]

Once downloaded, please follow these steps to install the module to your DNN website:

1.  Log into your site as either Host or another Supersuser level account.
2.  Navigate to the **Host** menu and select **Extensions**.
3.  Click on **Install Extension Wizard**.
4.  As directed, browse to the location of the downloaded ZIP file, select it then click **Open**.
5.  Click **Next**, accept the license and continue through the install.
6.  When finished, click **Return**.

Please check [this module installation video][9] from DNN for more details.

**Note:** If you get an error while uploading the module this is due to the maxRequestLength  limit in your DNN installation’s web.config. Open web.config and update maxRequestLength to 20MB by setting **maxRequestLength=”20480″** and  try to upload the module again.

## Using DNN Exchange Sync Module

After you have installed DNN Exchange Sync module it is really simple to start using it on your website. Please follow these simple steps to get started

1.  Make sure you are logged-in to DNN as a Host or Admin level account.
2.  Navigate to the page where you want to add the DNN Exchange Sync Module.
3.  Select **Modules** followed by **Add New Module** from the top ribbon.  
      
    [![DNN Exchange Sync add module to page][10]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/DNN-Exchange-Sync-add-module-to-page.png)
4.  From the list select, **Aspose** **DNN Exchange Sync** and drag it to a place of your choice on the page.

You have successfully added DNN Exchange Sync Module to your page. You will be presented with 3 simple options to get started

*   Exchange to DNN Sync
*   DNN to Exchange Sync
*   Exchange Settings

You are asked to enter Microsoft Exchange Server details when clicking on any option for the first time. A simple form takes all the required details to connect to your Exchange account and then these details will be encrypted and saved in the database for later use.

\[caption id="attachment\_15721" align="aligncenter" width="300" caption="DNN Exchange Sync - Microsoft Exchange Server Details"\][![DNN Exchange Sync Exchange Server Details][11]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/DNN-Exchange-Sync-Exchange-Server-Details.png)\[/caption\]

Once the sync process is completed, a brief summary of migrated records count and list of records that already existed and are not imported is shown.

## Video

Please check [the video][12] below to see it in action.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/aspose-Email-for-net_100.png "aspose-Email-for-net_100"
[2]: http://www.aspose.com/
[3]: https://products.aspose.com/email
[4]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/DNN-Exchange-Sync-home.png
[5]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/Exchange-to-DNN-Sync.png
[6]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/DNN-to-Exchange-Sync.png
[7]: https://docs.aspose.com/
[8]: http://store.dnnsoftware.com/home/product-details/dnn-exchange-sync-2-way-link-between-dnn-and-microsoft-exchange-server
[9]: http://www.dnnsoftware.com/community/learn/video-library/view-video/video/542/view/details/how-to-install-a-module-in-dotnetnuke-7
[10]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/DNN-Exchange-Sync-add-module-to-page-300x132.png "DNN Exchange Sync add module to page"
[11]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/07/DNN-Exchange-Sync-Exchange-Server-Details-300x178.png "DNN Exchange Sync Exchange Server Details"
[12]: https://www.youtube.com/watch?v=LqEiYz287GA




