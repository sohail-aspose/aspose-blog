---
title: 'Aspose Customer Newsletter, November 2006'
date: Sat, 02 Dec 2006 14:46:00 +0000
draft: false
url: /2006/12/02/62643/
author: DannyCooper
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue**...  
  
• Welcome!  
• Cool Holiday Savings  
• Product Spotlight - **[Aspose.Editor][1]**  
• Aspose.Pdf.Kit for .NET 2.2 Released  
• Tech Tip - Aspose.Grid Web Tips - Using your own icons instead of the default icons.  
• Aspose products have their own blogs  

**Welcome!**  
  
Welcome to the November 2006 issue of the Aspose Newsletter! In this month's newsletter we offer to you a 10% savings on any product or product suite! This is our way of saying Thanks for your business!

This month we will take a closer look at our spotlight product: Aspose.Editor, the release of Aspose.Pdf.Kit for .NET 2.2, and the new blog structure for Aspose products. We will also look at the Tech Tip section which covers Aspose.Grid Web Tips.  Remember, if you wish to no longer receive our newsletter, simply click here to unsubscribe and you will be removed from our mailing list.

[](/Products/Aspose.Editor/Splash/)**[Aspose.Editor][2]**

Looking for that new breed of word processor control? Well look no further! Aspose.Editor is the new breed of word processor control for Windows Forms .NET that you have been looking for! A specially crafted page layout engine displays, edits and prints pages a lot like Microsoft Word, but inside your application. The native format for documents in Aspose.Editor is WordprocessingML with a unique feature of roundtripping even for complex documents.  

We invite you to download the free evaluation version of Aspose.Editor so that you can better see how this great component can improve your development experience.

**Aspose.Pdf.Kit for .NET 2.2 Released**  
  
Aspose.Pdf.Kit for .NET is a PDF® document manipulating component that enables .NET applications to manipulate PDF® documents without utilizing Adobe Acrobat®. It includes features such as: splitting, concatenation, stamping, encryption and decryption, form filling, image and text extraction. Aspose.Pdf.Kit is very easy to use and is provided with several featured demos and examples.

In version 2.2 you will find improved support for annotations, bookmarks, action script and more!  For more details be sure to visit the online product announcement by clicking here.  
  
If you have not yet tried Aspose.Pdf.Kit, feel free to download the free evaluation version so you can see how this great component can better improve your development experience.

**Tech Tip**

**Aspose.Grid Web Tips**

**Using your own icons instead of the default icons**

The control's default icons are located in the url path /agw\_client/, and the file path is c:\\program files\\aspose\\aspose.grid\\agw\_client by default. You may see some images files like submit.gif, save.gif etc. in that folder. If you want to replace these images with your own images, you should add a config section to the web.config file of your web application.

<appSettings> <add key="aspose.grid.web.agw\_client\_path" value="/agw\_client/" /> </appSettings>

You may have noticed that this configuration can only affect the control images path and it can't affect the control's client-scripts path. For example, if you run your page with the GridWeb control and check the source file in the browser, you may find that the agw\_client\_path property of the grid's DIV element still looks like “/yourApp/webform1.aspx/”. In some cases, you may need to use redefine the client-script path. To force the control use the redefined image path as the client-script path, you should add another config setting in the appSettings section:

<add key="aspose.grid.web.force\_script\_path" value="true" /> Note This config is only take effect with licensed control.

**Aspose Products Have Their Own Blogs**  
  
In the past our product releases were intermingled with the blogs from our team members. Now, all of our product updates are done in their own blog category. Therefore, anyone interested in staying up-to-date with the latest versions of our products can simply subscribe to the product only RSS feed: http://www.aspose.com/Community/blogs/default.aspx?GroupID=39




[1]: /Products/Aspose.Editor/Default.aspx
[2]: /Products/Aspose.Editor/Default.aspx



