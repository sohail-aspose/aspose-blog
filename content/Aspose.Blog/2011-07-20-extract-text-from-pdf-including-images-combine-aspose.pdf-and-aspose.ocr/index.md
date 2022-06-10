---
title: 'Extract Text from PDF Including Images in C# using Aspose.PDF and Aspose.OCR'
date: Wed, 20 Jul 2011 12:11:05 +0000
draft: false
url: /2011/07/20/extract-text-from-pdf-including-images-combine-aspose.pdf-and-aspose.ocr/
author: Shahzad Latif
summary: ''
tags: ['Aspose.OCR', 'Aspose.Pdf', 'C# OCR Library', 'C# ocr', 'Extract Image', 'Extract Text', 'Extract Text from Image', 'Extract Text from PDF', 'Read PDF Images and Text in C#', 'detect text in images', 'extract text and images from pdf', 'product release', 'read text from images']
categories: ['Aspose.PDF Product Family', 'Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose.pdf-logo2.jpg" alt="Extract text and images from PDF using C# .NET">}}


Extracting text from a PDF file is a common requirement of the developers working with PDF files. [Aspose.PDF for .NET][1] already allows you to extract text from the PDF file using C# in your .NET applications. The only limitation was that the text couldn't be extracted from the images contained by the PDF file.

Well, with the introduction of [Aspose.OCR for .NET][2] in our .NET product suite, we have moved towards removing this limitation. In this post, I'm going to share some details along with the code snippets to elaborate that how both of these components can be used together to extract all the text from the PDF file using C#.

Currently, Aspose.OCR for .NET allows you to extract text from TIFF and BMP images. It supports Arial and Times New Roman fonts, and 16pt/32pt font sizes. However, we're adding support for new fonts and other attributes that will be available gradually in our upcoming versions.

Now, in order to extract text completely from the PDF file, including the images, you'll have to go through the following three steps:

*   Extract Text from the PDF File
*   Extract Images from the PDF File
*   Extract Text from the Images

## Extract Text from PDF using C#

Text can be extracted from the PDF file using either PdfExtractor in Facades or DOM API. Please see the C# code samples in the following topics to get an idea about extracting text from PDF:

*   [Extract Text from PDF using DOM API][3]
*   [Extract Text from PDF using Facades][4]

## Extract Images from PDF using C#

For extracting images, there are again two approaches: Facades or DOM API. Please see the following topics for further details:

*   [Extract Images from PDF using DOM API][5]
*   [Extract Images from PDF using Facades][6]

## Extract Text from Images using C#

As we have already extracted the images using one of the two approaches mentioned above, it's time to move forward to extract the text from these images. The following C# code snippet can help you with how to extract text from images:

```
//initialize OcrEngine
OcrEngine ocrEngine = new OcrEngine();
 //set the image
ocrEngine.Image = ImageStream.FromFile("image.bmp");

 //add language and other attributes
ocrEngine.Languages.AddLanguage(Language.Load("english"));
ocrEngine.Config.NeedRotationCorrection = false;
ocrEngine.Config.UseDefaultDictionaries = true;

//load the resource file
ocrEngine.Resource = new FileStream("2011.07.02 v1.0 Aspose.OCR.Resouces.zip", FileMode.Open);

//process the whole image
if (ocrEngine.Process()) 
{
Console.WriteLine("Text :{0}",ocrEngine.Text);
}
```

For more details on extracting text from the images using C# and getting the resource file we used in the above sample, please see the following topic: [Perform OCR on Image][7].




[1]: http://www.aspose.com/categories/.net-components/aspose.pdf-for-.net/default.aspx
[2]: http://www.aspose.com/categories/.net-components/aspose.ocr-for-.net/default.aspx
[3]: https://docs.aspose.com/display/pdfnet/Extract+Text+from+PDF
[4]: https://docs.aspose.com/pdf/net/
[5]: https://docs.aspose.com/display/pdfnet/Manipulate+Images#ManipulateImages-ExtractImagesfromthePDFFile
[6]: https://docs.aspose.com/pdf/net/
[7]: https://docs.aspose.com/display/ocrnet/Performing+OCR+on+an+Image




