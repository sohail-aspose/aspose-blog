---
title: 'PDF to EPUB, XFA to PDF, Get Print Job Status and Specify PDF Open Page with Aspose.Pdf for .NET 8.5.0'
date: Tue, 08 Oct 2013 15:23:51 +0000
draft: false
url: /2013/10/08/pdf-to-epub-xfa-to-pdf-get-print-job-status-and-specify-pdf-open-page/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---

[](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png)[![Aspose.Pdf for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Pdf-for-net_100.png)We are excited to announce new features like PDF to EPUB conversion, dynamic XFA to PDF or image conversion, getting the status of a PDF printing job (finding out whether the process completed successfully or got stuck in the middle of execution) and specifying a particular page number to open when viewing the document. All these feature are introduced in latest release of [ Aspose.Pdf for .NET 8.5.0][2].

At Aspose, we love to keep things simple and effective. Keeping that tradition alive, PDF to EPUB conversion is as simple as [EPUB to PDF conversion][3]. Just specify the source PDF file and leave the rest of the conversion job to Aspose.Pdf for .NET. Please take a look at the following code snippet for an example of PDF to EPUB conversion.

```
 // Load source PDF file
Document pdfDocument = new Document("c:/input.pdf");
// Instantiate EpubSave Options object
EpubSaveOptions options = new EpubSaveOptions();
// Specify the layout for resultant file
options.ContentRecognitionMode = EpubSaveOptions.RecogntionMode.Flow;
// Save the EPUB file
pdfDocument.Save("c:/output.epub", options); 
```

The operation to convert a dynamic XFA form to image formats is also implemented in this release. Please take a look over following code snippet which shows the steps to convert an XFA form to JPEG format using the JpegDevice class.

```
 string inFile = "c:/input_XFA.pdf";
string outFile = "c:/output_Image.jpg";
Aspose.Pdf.Document pd = new Aspose.Pdf.Document(inFile);
pd.Form.Type = FormType.Standard;
JpegDevice jpegDevice = new JpegDevice(new Resolution(96));
using (FileStream stream = new FileStream(outFile, FileMode.Create, FileAccess.Write))
{ jpegDevice.Process(pd.Pages[1], stream); } 
```

This release also includes other fixes related to converting PDF to HTML, converting PDF to image, creating tables inside a PDF file, manipulating bookmarks and converting PDF to PDF/A. Please download and evaluate the latest release of [Aspose.Pdf for .NET 8.5.0][4].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Pdf-for-net_100.png "Aspose.Pdf for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry500601.aspx
[3]: https://docs.aspose.com/display/pdfnet/Home
[4]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry500601.aspx




