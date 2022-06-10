---
title: 'Convert Tagged PDF to XML and Create Searchable PDF File with Aspose.Pdf for .NET 8.1.0'
date: Sat, 08 Jun 2013 17:43:17 +0000
draft: false
url: /2013/06/08/convert-tagged-pdf-to-xml-and-create-searchable-pdf-file/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'PDF to DOCX in CSharp', 'PDF to Searchable PDF', 'PDF to XML']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="PDF to XML in C# .NET">}}


We are pleased to announce the release of [Aspose.PDF for .NET 8.1.0][1] which includes some great features like converting normal PDF document to searchable PDF, [converting tagged PDF to XML][2] and the capability to get the dimensions of a source SVG file before its converted to PDF.

In order to convert a normal image PDF to a searchable PDF file, we need to perform OCR on the image inside the PDF file. The following logic recognizes text from PDF images. For recognition, you may use outer OCR supports HOCR standard ([http://en.wikipedia.org/wiki/HOCR][3].

You may use the free Google tesseract OCR ([http://en.wikipedia.org/wiki/Tesseract\_%28software%29][4]. Please install it on your computer from [http://code.google.com/p/tesseract-ocr/downloads/list][5] and after that you will have tesseract.exe console application.

```
private string CallBackGetHocr(System.Drawing.Image img)
{
      string dir = @"c:\PdfTest\";
      img.Save(dir + "test.jpg");
      ProcessStartInfo info = new ProcessStartInfo(@"tesseract");
      info.WindowStyle= ProcessWindowStyle.Hidden;
      info.Arguments = @"c:\pdftest\test.jpg c:\pdftest\out hocr";
      Process p = new Process();
      p.StartInfo = info;
      p.Start();
      p.WaitForExit();
      StreamReader streamReader = new StreamReader(@"c:\pdftest\out.html");
      string text = streamReader.ReadToEnd();
      streamReader.Close();
      return text;
}
public void Main
{
     Document doc = new Document("Input.pdf");
     doc.Convert(CallBackGetHocr);
     doc.Save("output.pdf");
}
```

## PDF to DOCX Conversion

One of the features introduced in this release is PDF to DOCX conversion. The PDF to DOC conversion has been supported for quite some time and now we are very much excited to announce support for PDF to DOCX conversion. A new property named Format has been added in the DocSaveOptions class. This property is used to specify the format of the output document: DOC or DOCX. In order to convert the PDF file to DOCX format, please pass Docx as the value from the DocSaveOptions.DocFormat enumeration. Please take a look at the following code snippet which converts a PDF file to DOCX.

```
// Open PDF document
Document pdfDocument = new Document("source.pdf");
// Instantiate DocSaveOptions object
DocSaveOptions saveOptions = new DocSaveOptions();
// Specify the output format as DOCX
saveOptions.Format = DocSaveOptions.DocFormat.DocX;
// Save document to DOCX format
pdfDocument.Save("output.docx", saveOptions);
```

Among these great features, we also have made some improvements to the PDF to HTML, PDF to XPS, PDF to TIFF and PDF to DOC conversion features. Printing PDF documents has also been improved. Please visit the following link for further details on what's new and fixed in [Aspose.PDF for .NET 8.1.0][6].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Convert+PDF+file+to+other+Formats#ConvertPDFfiletootherFormats-ConvertPDFtoXML
[3]: http://en.wikipedia.org/wiki/HOCR)
[4]: http://en.wikipedia.org/wiki/Tesseract_%28software%29)
[5]: http://code.google.com/p/tesseract-ocr/downloads/list
[6]: https://downloads.aspose.com/pdf/net




