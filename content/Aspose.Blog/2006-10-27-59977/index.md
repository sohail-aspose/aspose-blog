---
title: 'Aspose Customer Newsletter, October 2006'
date: Fri, 27 Oct 2006 21:04:00 +0000
draft: false
url: /2006/10/27/59977/
author: DannyCooper
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue**...  
  
• Welcome!  
• Product Spotlight - **[Aspose.Grid][1]**  
• Aspose.Words 4.0 Released!  
• Aspose.Barcode now supports Barcode Recognition  
• Tech Tip - Using Aspose.Words to guard against macro viruses

**Welcome!**  
  
Welcome to the October 2006 issue of the Aspose Newsletter!  This month we've added a new Tech Tip column.  The Tech Tip column is provided by our development staff and each month they will show you helpful tips and tricks for using Aspose components.

In this month's newsletter we will take a closer look at our spotlight product: Aspose.Grid.  We will also look at the release of Aspose.Words 4.0, Barcode Recognition in Aspose.Barcode and the new Tech Tip section.  Remember, if you wish to no longer receive our newsletter, simply click here to unsubscribe and you will be removed from our mailing list.

[](/Products/Aspose.Grid/Splash/)**[Aspose.Grid][2]**  
  
Aspose.Grid is just one of the many grid components you will find available for VS.NET.  However, Aspose.Grid is different.  It isn't just another option, it's the best value for your money.  We have focused on ease of use, price, features, performance and support in order to make Aspose.Grid best option on the market.  Whether you are developing desktop applications or ASP.NET applications, whether you are developing in VB.NET or C# - Aspose.Grid is the solution you want.

We invite you to download the free evaluation version of Aspose.Grid so that you can better see how this great component can improve your development experience.  

**Aspose.Words 4.0 Released!**

After many long months of hard work and effort, Aspose.Words 4.0 is ready for download.  Aspose.Words 4.0 boasts several new features such as: support for drawing objects and textboxes, a rich API for managing drawing objects, RTF export, WordML export, improved HTML export and more!  Furthermore, you will find a wealth of enhancements and bug fixes.  Click here to read the full story... 

If your subscription for Aspose.Words has expired but you have not yet renewed, now is the time to do it!  Or, if you have not yet had a chance to try Aspose.Words be sure to download the free evaluation version and learn why it has become the leading document management component.

**Aspose.Barcode 2.0 now supports barcode recognition!**

Aspose.Barcode is a full featured barcode component that allows developers to add barcode support to any kind of .NET application. Aspose.Barcode can generate and recognize most popular linear and 2D symbology of barcodes.  Aspose.Barcode is an all in one barcode solution for windows applications, console applications, web applications and smart device applications.

With the addition of the barcode recognition feature in Aspose.Barcode 2.0 it has become the complete barcode solution for ANY .NET application.  Barcode encoding and decoding is now straight forward and easy to use! Download the free evaluation version to experience the full power of Aspose.Barcode for yourself!

**Tech Tip**

**Using Aspose.Words to Guard Against Macro Viruses**

It is well known that macros stored in Microsoft Word documents might be malicious. They may contain macro viruses or other destructive code. See [Frequently Asked Questions About Word Macro Viruses][3] in the Microsoft Knowledge Base for more information.

Aspose.Words is a Word document processing component that is fully aware of macros (the VBA project) in the following ways:

*   Aspose.Words is completely safe against macro viruses because it never executes them (simply because it has no means to execute macros).
*   By default, Aspose.Words fully preserves existing macros in Words documents, including their digital signatures.
*   Aspose.Words allows one to quickly remove all macros from a document to ensure it is free from any harmful code.

To remove all macros from a Word document using Aspose.Words, call the **Document.RemoveMacros** method:

\[C#\]

Document doc = new Document("DangerousDocument.doc");

doc.RemoveMacros();

doc.Save("PureDocument.doc");

\[VB .NET\]

Dim doc As Document = New Document("DangerousDocument.doc")

doc.RemoveMacros()

doc.Save("PureDocument.doc")

\[Java\]

Document doc = new Document("DangerousDocument.doc");

doc.removeMacros();

doc.save("PureDocument.doc");




[1]: /Products/Aspose.Grid/Splash/
[2]: /Products/Aspose.Grid/Splash/
[3]: https://www.microsoft.com/en-pk



