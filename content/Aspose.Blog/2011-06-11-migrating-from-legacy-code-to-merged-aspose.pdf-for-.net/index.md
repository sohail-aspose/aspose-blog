---
title: 'Migrating from Legacy Code to Merged Aspose.PDF for .NET'
date: Sat, 11 Jun 2011 11:00:43 +0000
draft: false
url: /2011/06/11/migrating-from-legacy-code-to-merged-aspose.pdf-for-.net/
author: Shahzad Latif
summary: ''
tags: ['Shahzad Latif', 'Merged Aspose.Pdf', 'PDF', 'migrating code']
---

As we're moving close towards the release of the merged [Aspose.PDF for .NET][1], it is better to share some details regarding the migration of legacy Aspose.Pdf and Aspose.Pdf.Kit code to new merged Aspose.Pdf.

In this post, I'll share with you that how the license for the merged Aspose.Pdf will work. I'll also elaborate a couple of things which will be helpful while migrating your code from old Aspose.Pdf and Aspose.Pdf.Kit to merged Aspose.Pdf.

## Setting License

The existing users of Aspose.Pdf or Aspose.Pdf.Kit have license for their respective product. If you have any of these two licenses at the moment, you'll be able to use this license with the merged Aspose.Pdf. The code to use the license with merged Aspose.Pdf is same as the old Aspose.Pdf. You can see the code snippet below to use both of the old licenses:

> //using old Aspose.Pdf license  
> Aspose.Pdf.License license = new Aspose.Pdf.License();  
> license.SetLicense("Aspose.Pdf.lic");
> 
> //using old Aspose.Pdf.Kit license  
> Aspose.Pdf.License license = new Aspose.Pdf.License();  
> license.SetLicense("Aspose.Pdf.Kit.lic");

## Migrating Legacy Aspose.Pdf Code to Merged Aspose.Pdf

In order to migrate your code from old Aspose.Pdf to merged Aspose.Pdf, you need to make only minor changes. Previously, all the classes were present under Aspose.Pdf namespace. However, with the merged product all the classes of the Aspose.Pdf component have been moved under Aspose.Pdf.Generator namespace. If you were only importing Aspose.Pdf namespace then you only need to change it to Aspose.Pdf.Generator. However, if you were using the namespace along with the classes then you'll have to change the namespace in the code wherever you had used it. You can get the idea from the following example:

> //Instantiate PDF instance by calling empty constructor  
> Aspose.Pdf.Generator.Pdf newPdf = new Aspose.Pdf.Generator.Pdf();  
> //Create a section in the pdf document  
> Aspose.Pdf.Generator.Section sec1 = newPdf.Sections.Add();  
> //add a sample text paragraph to paragraphs collection of section object  
> sec1.Paragraphs.Add(new Aspose.Pdf.Generator.Text("Hello World"));  
> // Save the resultant PDF document  
> newPdf .Save("HelloWorld.pdf");

## Migrating Legacy Aspose.Pdf.Kit Code to Merged Aspose.Pdf

All the classes of old Aspose.Pdf.Kit have been moved under Aspose.Pdf.Facades. We have made a couple of changes on some places in the old API, which you'll have to incorporate in your code before migrating it to the merged Aspose.Pdf. However, these changes are very small in nature. And these changes were introduced in order to exploit the full potential of the new PDF engine via Aspose.Pdf.Facades as well.

However, the most important change is the namespace; you'll be using Aspose.Pdf.Facades, instead of Aspose.Pdf.Kit, in order to migrate your code to the merged Aspose.Pdf API.  You can see a sample code snippet below:

> //create PdfFileMend object to add text  
> Aspose.Pdf.Facades.PdfFileMend mender = new Aspose.Pdf.Facades.PdfFileMend("input.pdf", "output.pdf");
> 
> //create formatted text  
> Aspose.Pdf.Facades.FormattedText text = new Aspose.Pdf.Facades.FormattedText("Aspose - Your File Format Experts!",  
> System.Drawing.Color.AliceBlue,  
> System.Drawing.Color.Gray,  
> Aspose.Pdf.Facades.FontStyle.Courier,  
> EncodingType.Winansi,  
> true,  
> 14  
> );
> 
> //set whether to use Word Wrap or not and using which mode  
> mender.IsWordWrap = true;  
> mender.WrapMode = WordWrapMode.Default;
> 
> //add text in the PDF file  
> mender.AddText(text, 1, 100, 200, 200, 400);
> 
> //close PdfFileMend object  
> mender.Close();

Other changes belong to the Annotations, Bookmarks and Attachment areas. I'll elaborate those changes separately, along with the code snippets, in my next post.




[1]: https://products.aspose.com/pdf



