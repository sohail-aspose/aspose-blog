---
title: 'Umbraco Export to Microsoft Word using Aspose.Words'
date: Wed, 15 Jan 2014 09:43:13 +0000
draft: false
url: /2014/01/15/umbraco-export-to-word-using-aspose.words/
author: Zaheer Tariq
summary: ''
tags: ['Export to Doc', 'Export to Docx', 'Export to Word', 'File Format API', 'HTML to Doc', 'HTML to Docx', 'HTML to Word', 'Macro', 'Umbraco']
categories: ['Aspose.Words Product Family']
---

Umbraco's Export to Word macro allow users to export online content into a Microsoft Word document using [Aspose.Words][1]. This macro makes it super simple to get an offline copy of your favorite online content for editing, sharing and printing in most popular Microsoft Word formats (DOC/DOCX). It adds a simple **Export to Word** button at any desired location on the web page. Clicking the button exports the page content to a Word document and automatically downloads the file to a disk location selected by the user in just seconds.



{{< figure align=center src="images/Export-to-word.png" alt="Export to Word using Aspose.Words" caption="Export to Word using Aspose.Words">}}




{{< figure align=center src="images/Export-to-word-generated-output.png" alt="Export to Word output Word document" caption="Export to Word output Word document">}}


## Installing the Export to Word Macro

Download the Export to Word macro package from one of the following locations:

*   Download from [CodePlex][2]
*   Download from [Umbraco Projects][3]

Once downloaded, please follow these steps to install a package into your Umbraco website:

1.  Login to Umbraco **Developer** section, for example http://www.myblog.com/umbraco/
2.  From the tree, expand the **Packages** folder.
3.  From here there are two ways to install a package: select **Install local package** or browse the **Umbraco Package Respository.**
4.  If you install **local package**, do not unzip the package but load the zip into Umbraco.
5.  Follow the instructions on screen

**Note:** You may get a ‘Maximum request length exceeded’ error when installing. You can easily fix this issue by updating the ‘maxRequestLength’ value in your Umbraco web.config file.

```
<httpRuntime requestValidationMode="2.0" enableVersionHeader="false" 
             maxRequestLength="25000" />

```

## Using the Export to Word Macro

After you have installed the Export to Word macro it is really simple to start using it on your website. Please follow these simple steps to get started:

1.  Make sure you are logged-in to Umbraco **Developer** section, for example http://www.myblog.com/umbraco/
2.  Click **Settings** in the list of sections in bottom left of the screen.
3.  Expand the **Templates** node and select the template that you want to add the Export to Word feature to, for example Blog post.
4.  Select the position in the selected template where you want to export button to be added. Usually you probably want to add it to the top right of the page, or the bottom of the page.
5.  Click **Insert Macro** on the top ribbon.
6.  From **Choose a macro**, select the recently installed Export to Word using Aspose.Words macro and click **OK**.  
    Please check the screenshot below for details.



{{< figure align=center src="images/how-to-use-export-to-word-macro.png" alt="How to use ‘Export to Word’ macro" caption="How to use ‘Export to Word’ macro">}}


You have successfully added Export to Word to the template. A button titled **Export to Word** will now appear on all pages created using this template. Anyone can simply click the button and export the content of the page into a Word document.

## Video

Please check the video below to see this macro in action.

<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">https://youtu.be/3EHf3Giq6l0</div></figure>




[1]: https://products.aspose.com/words
[2]: https://docs.aspose.com/
[3]: http://our.umbraco.org/projects/developer-tools/export-to-word-using-asposewords




