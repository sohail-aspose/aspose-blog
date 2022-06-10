---
title: 'Use PDF Measurement Tool in C# or VB.NET'
date: Wed, 13 Aug 2014 19:37:07 +0000
draft: false
url: /2014/08/13/pdf-measurement-tool-in-csharp-or-vb.net-pdf-library/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Csharp PDF Measurement Tool']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


We are very excited to announce the release of [Aspose.PDF for .NET 9.5.0][1] which introduces some great new features. The development team has been working hard to implement these features and is pleased to make them available in our public API.

## PDF Measurement Tool using C#

Recently we received a requirement to add measurement elements using Aspose.PDF for .NET (like we can use [the measurement tool in Adobe Acrobat][2] to a PDF document. In order to accomplish this requirement, a class named Measure is added to the Aspose.InteractiveFeatures.Annotations namespace and it describes the measurement coordinate system. For further details regarding this feature, please visit [Use API as PDF Measurement Tool][3].

## Remove Extended Rights Feature

The PDF feature extended rights enables end-users to fill data into form fields by using Adobe Reader and then save the filled form copy. However, it ensures that the PDF file is not modified and, if any modification to the structure of PDF is made, the extended rights feature is lost so that when viewing such a document, an error message is displayed stating that extended rights have been removed because the document was modified. Recently we received a requirement to remove extended rights from PDF document. We are pleased to share that this feature is implemented in the latest release of Aspose.Pdf for .NET, version 9.5.0. Please visit the following link for further details on how to remove the extended rights feature from a PDF file.

## Support HTML Contents in DOM

The Aspose.Pdf.Generator.Text class contains a property named IsHtmlTagSupported which provides the feature to add HTML tags/contents to a PDF file. Content added this way is rendered in native HTML tags instead of appearing as simple text strings. To support a similar feature in the new Document Object Model (DOM) of the Aspose.Pdf namespace, we have introduced the HtmlFragmentclass. For more information and details regarding this feature, please visit [Add HTML Contents using DOM Approach.][4]

## PDF to HTML - Save HTML, CSS, Image and Font Resources in a Stream Object

During PDF to HTML conversion, fonts, images, and CSS files containing style information for the PDF contents are generated. These resources are necessary to maintain the formatting of the output HTML file. However, there might be a scenario when you want to load the PDF file Stream object and you do not need to store or save these resource files on the system or drive. For example, if you don't have the permissions to saving intermediate resource files or you do not want to save these resources but need to perform the conversion on the fly (the file will only be viewed once and is not required for later processing). For further details, please visit [PDF to HTML - Save HTML, CSS, Image and Font Resources in a Stream Object][5]

## Get/Set FieldLimit

The FormEditor class' SetFieldLimit("textbox1", 20) method supports the feature to set the field limit, that is the maximum number of characters that can be placed or inserted into a field, as shown below.

```
// Adding field with limit
Aspose.Pdf.Facades.FormEditor form = new Aspose.Pdf.Facades.FormEditor();
form.BindPdf("input.pdf");
form.SetFieldLimit("textbox1", 15);
form.Save("output.pdf");
```

Similarly, we have created a new method to get field limits using the DOM approach. The following code snippet shows the steps to get the field limit value.

```
// Getting maximum field limit using DOM
Document doc = new Document("output.pdf");
Console.WriteLine("Limit: " + (doc.Form\["textbox1"\] as TextBoxField).MaxLen);
```

We can also get the same value using the Aspose.Pdf.Facades namespace. Please try using the following code snippet.

```
// Getting maximum field limit using Facades
Aspose.Pdf.Facades.Form form = new Aspose.Pdf.Facades.Form();
form.BindPdf("output.pdf");
Console.WriteLine("Limit: " + form.GetFieldLimit("textbox1"));
```

As well as the above features, this release includes fixes for many issues and it is a major release. Please go ahead, download, and start exploring the new release of [Aspose.PDF for .NET 9.5.0.][6]




[1]: https://downloads.aspose.com/pdf/net
[2]: http://help.adobe.com/en_US/acrobat/X/standard/using/WS58a04a822e3e50102bd615109794195ff-7f9d.w.html#WS58a04a822e3e50102bd615109794195ff-7f91.w>)
[3]: https://docs.aspose.com/
[4]: https://docs.aspose.com/display/pdfnet/Add+Text+to+a+PDF+file#AddTexttoaPDFfile-AddHTMLStringusingDOM
[5]: https://docs.aspose.com/display/pdfnet/Convert+PDF+File+into+HTML+Format#ConvertPDFFileintoHTMLFormat-PDFtoHTML-SaveHTML,CSS,Image,andFontResourcesinStreamObject
[6]: https://downloads.aspose.com/pdf/net




