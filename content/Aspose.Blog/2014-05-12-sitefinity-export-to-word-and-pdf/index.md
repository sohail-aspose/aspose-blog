---
title: 'Sitefinity Export to Microsoft Word (DOCX/DOC) and PDF Files'
date: Mon, 12 May 2014 07:54:43 +0000
draft: false
url: /2014/05/12/sitefinity-export-to-word-and-pdf/
author: Zaheer Tariq
summary: ''
tags: ['Aspose.Words', 'Content Export', 'Export to Doc', 'Export to Docx', 'Export to PDF', 'Export to Word']
categories: ['Aspose.Words Product Family']
---

The Aspose Sitefinity Content Export add-on allows users to export online content into Microsoft Word or Adobe Acrobat PDF documents using [Aspose.Words][1]. This add-on makes it very simple to have an offline copy of your favorite online content for editing, sharing and printing etc. in popular Microsoft Word DOC/DOCX or PDF format. It adds a simple **Export to Word** and **Export to Pdf** buttons at any desired location on the page. Clicking the button dynamically exports the content of the page into Microsoft Word or PDF document. The exported file is then automatically presented for downloading to any disk location selected by the user in just couple of seconds.



{{< figure align=center src="images/Sitefinity-content-export-to-microsoft-word-and-pdf-300x128.png" alt="Sitefinity export to Word document" caption="Sitefinity Export to Microsoft Word and PDF using Aspose.Words">}}




{{< figure align=center src="images/Sitefinity-exported-microsoft-word-document-using-Aspose.Words_-300x182.png" alt="Sitefinity exported Microsoft Word Document using Aspose.Words" caption="Sitefinity exported Microsoft Word Document using Aspose.Words">}}


## Installing and Configuring the Aspose Sitefinity Content Export Add-on

You can download the Aspose Sitefinity Content Export add-on from one of the following locations:

*   Download from [CodePlex][2]
*   Download from [GitHub][3]

Once downloaded, please follow these steps to install the Add-on into your Sitefinity website:

**Step 1: Copy files to your Sitefinity installation**

Please extract the downloaded ZIP file. You will need FTP or direct access to the Sitefinity installation folder on the server to perform the following:

1.  Copy Aspose.Words.dll and Aspose.SiteFinity.ContentExport.dll into the **bin** folder of the Sitefinity installation.
2.  Copy the **Addons** folder on the root of the Sitefinity installation where the **bin** folder is located.

**Step 2: Register the Aspose Sitefinity Content Export add-on in Sitefinity**

1.  Log into your Sitefinity CMS with an ‘**Administrator**’ account. The login page can be reached by [http://www.mywebsite.com/sitefinity][4]
2.  Click **Administration** and then **Settings**.  
    The Basic Settings page appears.
3.  Click the **Advanced**  link.  
    The Settings  page appears.
4.  In the left pane, click **Toolboxes**  followed by **Toolboxes**, then **PageControls**, **Sections** and **ContentToolboxSection**, then **Tools.**
5.  Click **Create new**.  
    The widget registration form appears.
6.  Fill the form fields as follows:
    1.  Make sure **Enabled** is selected.
    2.  Add ~/Addons/AsposeContentExport.ascx in the **Control CLR Type or Virtual Path** field.
    3.  Add **Name**, **Title** and **Description** as follows:  
        AsposeContentExport  
        Aspose Content Export  
        Export online content into Microsoft Word or PDF document using Aspose.Words
    4.  You may leave all other fields as they are.
7.  When finished, click **Save changes**.  
    The widget is registered in the toolbox and can be used in Sitefinity. The settings are also shown in the picture below



{{< figure align=center src="images/Registering-Aspose-Sitefinity-Content-Export-Add-on-in-Sitefinity-268x300.png" alt="Registering Aspose Sitefinity Content Export Add-on in Sitefinity" caption="Registering Aspose Sitefinity Content Export Add-on in Sitefinity">}}


## Using the Aspose Sitefinity Content Export Add-on

After you have installed and configured the Aspose Sitefinity Content Export add-on it is really simple to start using it on your website. Please follow these simple steps to get started:

1.  Make sure you are logged-in to Sitefinity with an Administrator level account.
2.  Navigate to the page where you want to add the Export add-on. Make sure the page is opened in edit mode.
3.  From the **Drag Widgets** menu on the right, select Aspose Content Export and drag it into position.

You have successfully added Aspose Sitefinity Content Export to your page. Two buttons, **Export to Word** and **Export to Pdf**, now appear on the page. Anyone can simply click a buttons and export the content of the page into a Microsoft Word or PDF document.

## Video

Please check [the video][5] below to see it in action.




[1]: http://www.aspose.com/word-component-suite.aspx
[2]: https://docs.aspose.com/
[3]: https://github.com/asposemarketplace/Aspose_for_Sitefinity/releases
[4]: http://www.mywebsite.com/sitefinity
[5]: https://www.youtube.com/watch?v=mopEZvGn_30




