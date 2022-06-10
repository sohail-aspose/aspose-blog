---
title: 'PDF to HTML - Save Images in Raster Format using C#'
date: Sun, 16 Feb 2014 06:26:58 +0000
draft: false
url: /2014/02/16/pdf-to-html-save-images-in-raster-format-using-csharp/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


PDF to HTML conversion is one of the prominent features [Aspose.PDF for .NET][1] offers. By default, the images inside the document are saved in SVG format when converting PDF files to HTML format. However, it is possible to save images in non-SVG format, as raster images. Please have a look at the following code snippet to see how this can be done.

```
// Source PDF file
Document doc = new Document("c:/pdftest/page_6.pdf");
// Create HtmlSaveOption with tested feature
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.FixedLayout = true;
saveOptions.SplitIntoPages = false;
saveOptions.RasterImagesSavingMode = HtmlSaveOptions.RasterImagesSavingModes.AsExternalPngFilesReferencedViaSvg;

string outFile = "c:/pdftest/Sample_ResultantFile.html";
// Save the output in HTML format
doc.Save(outFile, saveOptions); 
```

For further details, please visit PDF to HTML - Save Images in Raster Format.

## Get/Set PDF Information

This API provides the capability to get and set PDF file information. It also provides the feature to get and set custom properties associated with the PDF document. In this release, we have provided the feature to access custom property values, such as Trapped, from PDF files. Please note that the Trapped property is a part of the DocumentInfo structure, so in order to get or set its value, please try using the following code snippet.

```
using (Document pdfDocument = new Document(@"c:\test.pdf"))
{
    if (pfDocument.Info.Trapped == "True")
    {
        // Do something
    }
}
```

For more information, please visit Get PDF File Information.

This hotfix also contains fixes for some other high priority issues. Please visit the download section to get details on what's new and what's fixed in [Aspose.PDF for .NET 8.9.1][2].




[1]: https://products.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net




