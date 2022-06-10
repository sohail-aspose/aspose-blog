---
title: 'Aspose Customer Newsletter, December 2006'
date: Tue, 02 Jan 2007 13:28:00 +0000
draft: false
url: /2007/01/02/64344/
author: DannyCooper
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue**...  
  
• Welcome!  
• Product Spotlight - **[Aspose.Cells][1]**• What Aspose Word Processing Component Do You Need?  
• Tech Tip - Making Changes after a Conversion from Word to PDF  
• Aspose.Slides bug fixes and enhancements added in December.

**Welcome!**  
  
Welcome to the December 2006 issue of the Aspose Newsletter! In this month's newsletter we will take a closer look at our spotlight product: Aspose.Cells. We will also look at the Tech Tip section which covers making changes after a conversion from Word to PDF as well as go over some tips in helping you choose the right Aspose Word Processing Component.

[![][2]](https://blog.aspose.com/category/words/)**[Aspose.Cells][3]**

Aspose.Cells strives to demonstrate three major services: quality, reliability and performance. In doing so, Aspose.Cells offers easy to use APIs that supports a wide variety of features with opening and saving native Excel files as its core feature. It has many common features including worksheet management, manipulating rows and columns, data formats, manipulating cells, formatting cells, shaping borders, setting colors, setting fonts and inserting/deleting a range of cells.

Besides supporting common features, Aspose.Cells also supports many advanced features such as opening and saving Excel files to and from streams, sending output to a client browser, and many more.

We invite you to download the [free evaluation][4] version of Aspose.Cells so that you can better see how this great component can improve your development experience.

**What Aspose Word Processing Component Do You Need?**

Can't decide which Aspose Word Processing component to pick? Troubled by the issue of what to choose and worry that you won't choose the right component for your development?

Well we have the solution for you! We have laid out the differences in Aspose.Words and Aspose.Editor to help you in the decision of which one is the right Aspose Word Processing Component to pick.

[Click here][5] for more information!  

**![](https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/total/272x272/aspose_total-for-net.png)Tech Tip**

**Making Changes after a Conversion from Word to PDF**

A very common use for Aspose.Pdf is the conversion of Word Documents to PDF. However, from time to time one may have a need to make further changes to a document after such a conversion. For example, suppose you would like to import the headings from a Word document and then convert them to bookmarks in the resulting PDF. How would you achieve that? Just simply do as follows…

\[C#\]

Aspose.Pdf.Pdf pdf = new Aspose.Pdf.Pdf();  
//Object xmlDoc contains all contents from original word document in XML format defined in Aspose.PDF  
//XML Schema.  
pdf.BindXML(xmlDoc,null);  
//Before saving, to add bookmarks from headings.  
pdf.IsBookmarked = true;  
foreach(Aspose.Pdf.Section sec in pdf.Sections)  
{  
  foreach(Aspose.Pdf.Paragraph para in sec.Paragraphs)  
 {  
   if(para is Heading)  
   {  
     Heading h = para as Heading;  
     h.IsInList = true;  
   }  
 }  
}  
pdf.Save(outputFile);  

\[VB.Net\]

Dim pdf As Aspose.Pdf.Pdf = New Aspose.Pdf.Pdf()  
'Object xmlDoc contains all contents from original word document in XML format defined in Aspose.PDF  
'XML Schema.  
pdf.BindXML(xmlDoc,Nothing)  
'Before saving, to add bookmarks from headings.  
pdf.IsBookmarked = True  
Dim sec As Aspose.Pdf.Section  
For Each sec In pdf.Sections  
 Dim para As Aspose.Pdf.Paragraph  
 For Each para In sec.Paragraphs  
  If TypeOf para Is Heading Then  
   Dim h As Heading = para as Heading  
   h.IsInList = True  
  End If  
 Next  
Next  
pdf.Save(outputFile)  

With that is mind you can easily see that when doing a conversion from any supported format to PDF, Aspose.Pdf provides you an easy yet powerful API for further modification.

**Aspose.Slides Bug Fixes and Enhancements added in December.**  
  
In the month of December, several new enhancements, bug fixes and changes were added to Aspose.Slides. Some of these included adding the reading, creating and rendering connectors, the changing of the default style of curve connectors, fixing the read/write/clone slides, and fixing the reading text holders where in some cases, Aspose.Slides could not read text inside the text holder.

For more information or to see more enhancements, bug fixes or changes on Aspose.Slides, please see our blogs by clicking [here][6].




[1]: https://downloads.aspose.com/cells
[2]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/total/272x272/aspose_total-for-sharepoint.png
[3]: https://downloads.aspose.com/cells
[4]: https://downloads.aspose.com/cells
[5]: https://blog.aspose.com/category/words/
[6]: https://docs.aspose.com/display/wordsjava/Home



