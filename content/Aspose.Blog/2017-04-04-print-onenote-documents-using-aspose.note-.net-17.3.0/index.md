---
title: 'Print OneNote Documents using Aspose.Note for .NET 17.3.0'
date: Tue, 04 Apr 2017 14:06:56 +0000
draft: false
url: /2017/04/04/print-onenote-documents-using-aspose.note-.net-17.3.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---

[![][1]](https://www.aspose.com/products/note/net)

We are pleased to announce the release of [Aspose.Note for .NET 17.3.0][2]. This month’s release introduces a new feature of printing OneNote documents to printer. It also provides support for linking images in a document to a URL. For a detailed note on what is new and fixed, please visit the [release notes][3] section of Aspose.Note for .NET documentation.

# New Features and Enhancements

**Printing OneNote Document:** As mentioned earlier, this month’s release introduces a new feature of [printing OneNote][4] documents. The Document.Print method allows sending the loaded document to default printer. You can also specify printer settings for printing the document using the PrintOptions class. These settings include page layout, margins information, and page splitting algorithm. The following code sample shows the usage of this new API feature.

```
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
{
    PrinterSettings = printerSettings,
    Resolution = 1200,
    PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
    DocumentName = "Test.one"
}); 
```

**Support for Hyperlinks in Images:** We have also enhanced the API with capability of  linking document images to hyperlinks. The HyperlinkUrl property exposed by the Image class can be specified to [link the image][5] to a URL, as shown in the following code sample.

```
string dataDir = RunExamples.GetDataDir_Images(); 
            
var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg");
            
image.HyperlinkUrl = "http://image.com";
            
page.AppendChild(image);
            
document.AppendChild(page);
            
document.Save(dataDir + "Image with Hyperlink_out.one"); 
```

**Optimization of File Size and Saving Time:** This month’s release also optimizes the output file size and time required to save OneNote documents that have many page revisions. This further improves the performance of API while working with such documents.

# Other Improvements

This month's release also fixes a number of bugs that further adds to the stability of the API functionality. At Aspose, we are committed to improve the API functionality with every new release and fixing issues contributes to our this cause.

# API Resources

You can get started with Aspose.Note for .NET by making use of information available in the following.

**[API Documentation][6]** – Helps getting started with the API using code samples and examples

**[Forum Support][7]** – Post your inquiries to get help from our technical support team

**[Examples][8]** – Try the ready-to-use examples of the API by downloading from our GitHub repository

**[API Reference Guide][9]** – Provides information about all the namespaces, classes and properties of the API




[1]: http://blog.aspose.com/wp-content/uploads/sites/2/2016/11/Aspose.Note-for-.NET_.png
[2]: https://downloads.aspose.com/note/net
[3]: https://docs.aspose.com/display/notenet/Aspose.Note+for+.NET+17.3.0+Release+Notes
[4]: https://docs.aspose.com/display/notenet/Printing+Documents
[5]: https://docs.aspose.com/display/notenet/Working+with+Images#WorkingwithImages-LinkanImagetoHyperlink
[6]: https://docs.aspose.com/display/notenet/Home
[7]: https://forum.aspose.com/c/note
[8]: https://github.com/asposenote/Aspose_Note_NET
[9]: http://www.aspose.com/api/net/note




