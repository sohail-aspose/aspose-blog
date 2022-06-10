---
title: 'Import Contents from Microcoft Word and PDF Files to Umbraco Sites'
date: Wed, 19 Feb 2014 12:07:54 +0000
draft: false
url: /2014/02/19/import-contents-from-word-and-pdf-files-to-umbraco-sites/
author: Zeeshan Shafqat
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

We are pleased to announce the release of more macros in Umbraco. The macros involved in this release are below:

*   [Umbraco Import from Words using Aspose.Words][1]
*   [Umbraco Import from PDF using Aspose.PDF][2]

You can download the macro from the social coding website of your choice. The macros include an **Import from Word/PDF** button that displays the uploaded document. These will help you to get the contents of your document using Aspose.Words and Aspose.PDF whether you have Microsoft Word or Adobe Reader installed on your machine or not.

## Installing the Macro

Download the macro package from one of the following locations:

*   Download from [CodePlex][3].
*   Download from [Umbraco Projects][4].

Once downloaded, please follow these steps to install this package into your Umbraco website:

1.  Log in to the Umbraco **Developer** section, for example http://www.myblog.com/umbraco/
2.  From the tree, expand the **Packages** folder.  
    From here there are two ways to install a package: select **Install local package** or browse the **Umbraco Package Respository.**
3.  If you install **local package**, do not unzip the package but load the zip into Umbraco.
4.  Follow the instructions on screen.

**Note:** You may get a ‘Maximum request length exceeded’ error when installing. You can easily fix this issue by updating the ‘maxRequestLength’ value in your Umbraco web.config file.

```
<httpRuntime requestValidationMode="2.0" enableVersionHeader="false" 
             maxRequestLength="25000" /> 
```

## Using the Macro

After you have installed the macro it is really simple to start using it on your website:

1.  Make sure you are logged in to the Umbraco **Developer** section, for example http://www.myblog.com/umbraco/
2.  Click **Settings** in the list of sections at the bottom left of the screen.
3.  Expand the **Templates** node and select the template that you want to add macro to, for example Blog post.
4.  Select the position in the selected template where you want to the button.
5.  Click **Insert Macro** on the top ribbon.
6.  From **Choose a macro**, select the installed macro and click **OK**.

You have successfully added the template. A button titled **Import to Word/Pdf** now appears on all pages created using this template. Anyone can simply click the button and import the contents from a Word or PDF document.

## Video

Please check the video below to see macro in action.

[Umbraco Macro for Import Word and Pdf][5]




[1]: https://docs.aspose.com/
[2]: https://docs.aspose.com/
[3]: https://docs.aspose.com/
[4]: https://bitbucket.org/asposemarketplace/aspose-for-umbraco/overview
[5]: http://www.youtube.com/watch?v=SSggrpVYkXs




