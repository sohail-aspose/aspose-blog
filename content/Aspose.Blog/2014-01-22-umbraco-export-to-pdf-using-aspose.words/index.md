---
title: 'Umbraco Export to PDF using Aspose.Words'
date: Wed, 22 Jan 2014 05:14:41 +0000
draft: false
url: /2014/01/22/umbraco-export-to-pdf-using-aspose.words/
author: Zaheer Tariq
summary: ''
tags: ['Document Export', 'Export to PDF', 'HTML to PDF', 'Online content Export', 'Umbraco', 'Umbraco Export']
categories: ['Aspose.Words Product Family']
---

The Umbraco **Export to PDF** macro allows users to export online content to a PDF document using [Aspose.Words][1]. This macro makes it very easy and simple to have an offline copy of your favorite online content for sharing and printing etc. in the popular PDF format. It adds a simple **Export to PDF** button at any desired location on the page and clicking it exports the content of the page to a PDF document and automatically downloads the file to the location selected by the user in just a couple of seconds.



{{< figure align=center src="images/Export-to-pdf1.png" alt="" caption="Export to PDF using Aspose.Words">}}




{{< figure align=center src="images/Export-to-pdf-generated-output1.png" alt="" caption="Export to PDF generated output document">}}


## Installing the Export to PDF Macro

Download the Export to PDF macro package from one of the following locations:

*   Download from [CodePlex][2].
*   Download from [Umbraco Projects][3].

Once downloaded, please follow these steps to install this package into your Umbraco website:

1.  Log in to the Umbraco **Developer** section, for example, http://www.myblog.com/umbraco/
2.  From the tree, expand the **Packages** folder.
3.  From here there are two ways to install a package: select **Install local package** or browse the **Umbraco Package Respository.**
4.  If you install **local package**, do not unzip the package but load the zip into Umbraco.
5.  Follow the instructions on screen.

**Note:** You may get a ‘Maximum request length exceeded’ error when installing. You can easily fix this issue by updating the ‘maxRequestLength’ value in your Umbraco web.config file.

```
<httpRuntime requestValidationMode="2.0" enableVersionHeader="false" maxRequestLength="25000" /> 
```

## Using the Export to PDF Macro

After you have installed the Export to PDF macro it is really simple to start using it on your website. Please follow these simple steps to get started:

1.  Make sure you are logged in to the Umbraco **Developer** section, for example, http://www.myblog.com/umbraco/
2.  Click **Settings** in the list of sections in the bottom left of the screen.
3.  Expand the Templates node and select the template that you want to add the Export to PDF feature to, for example, Blog post.
4.  Select the position in the selected template where you want to export the button to be added. Usually, you want to add it to the top right of the page, or the bottom of the page.
5.  Click **Insert Macro** on the top ribbon.
6.  From **Choose a macro**, select the recently installed Export to PDF using Aspose.Words macro and click **OK**.  
    Please check the screenshot below for details.



{{< figure align=center src="images/how-to-use-export-to-pdf-macro.png" alt="How to use Export to PDF macro" caption="How to use Export to Pdf macro">}}


You have successfully added Export to Pdf to the template. A button titled **Export to Pdf** now appears on all pages created using this template. Anyone can simply click the button and export the content of the page into a PDF document.

## Demo Video

Please check the video below to see this macro in action.

<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">https://youtu.be/EcZZzswqybc</div></figure>




[1]: http://www.aspose.com/word-component-suite.aspx
[2]: https://docs.aspose.com/
[3]: http://our.umbraco.org/projects/developer-tools/export-to-pdf-using-asposewords




