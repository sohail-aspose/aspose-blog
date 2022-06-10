---
title: 'Extract Text from Page Region, Manipulate Files up to 1.5GB with Aspose.PDF for .NET 8.2.0'
date: Mon, 08 Jul 2013 21:06:56 +0000
draft: false
url: /2013/07/08/extract-text-from-particular-page-region-manipulate-files-up-to-1.5-gb/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Calculate Bbox for Character in PDF', 'Extract Text from Page Region in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


We are proud to announce the release of [Aspose.PDF for .NET 8.2.0][1] which provides some great new features including text extraction from a particular page region, calculating the Bbox for a character, defining an outer color of the text when using RenderingMode.FillStrokeText and much more.

## Extracting Text from Page Region

Since the first release of Aspose.PDF for .NET, the component has provided the capability to extract text and images from PDF files. Recently, we have received requests to implement a feature for extracting text from a particular page region. In order to accomplish this task, please try using the following code snippet:

```
// Open document
Document doc = new Document("input.pdf");

// Create TextAbsorber object to extract text
TextAbsorber absorber = new TextAbsorber();
absorber.TextSearchOptions.LimitToPageBounds = true;
absorber.TextSearchOptions.Rectangle = new Aspose.Pdf.Rectangle(200, 200, 450, 350);

// Accept the absorber for first page
doc.Pages[1].Accept(absorber);

// Get the extracted text
string extractedText = absorber.Text;
```

## Calculating Bbox for Characters

Another feature we have been asked for is calculating a character's bounding box. To fulfill this requirement, we've implemented the **CharInfo** class and **TextSegment.Characters** collection. The following code snippet shows how to iterate through all characters in a PDF file and draw a rectangle around them:

```
// Open document
Document pdfDocument = new Document("input.pdf");
 TextFragmentAbsorber textFragmentAbsorber = new TextFragmentAbsorber();

// Accept the absorber for all the pages
pdfDocument.Pages[1].Accept(textFragmentAbsorber);

// Get the extracted text fragments
TextFragmentCollection textFragmentCollection = textFragmentAbsorber.TextFragments;

// Suppress page contents updates until all operations are done
pdfDocument.Pages[1].Contents.SuppressUpdate();
try
{
    // Loop through the fragments
    foreach (TextFragment textFragment in textFragmentCollection)
    {
        for (int i = 0; i < 100; i++)
        {
            foreach (TextSegment textSegment in textFragment.Segments)
            {
                foreach (CharInfo charInfo in textSegment.Characters)
               {
                   pdfDocument.Pages[1].Contents.Add(new Operator.GSave());
                   pdfDocument.Pages[1].Contents.Add(new Operator.ConcatenateMatrix(1, 0, 0, 1, 0, 0));
                   pdfDocument.Pages[1].Contents.Add(new Operator.SetRGBColorStroke(0.7, 0, 0));
                   pdfDocument.Pages[1].Contents.Add(new Operator.Re(charInfo.Position.XIndent,
                   charInfo.Position.YIndent,
                   charInfo.Rectangle.Width,
                   charInfo.Rectangle.Height));
                   pdfDocument.Pages[1].Contents.Add(new Operator.ClosePathStroke());
                   pdfDocument.Pages[1].Contents.Add(new Operator.GRestore());
                }
            }
        }
    }
}
finally
{
    // Resume page contents updates
    pdfDocument.Pages[1].Contents.ResumeUpdate();
}
pdfDocument.Save("output_Bbox.pdf");
```

From this release, we have also included product binaries specific for .NET Framework 3.5\_ClientProfile. Among other great enhancements, the product has been tested when manipulating large PDF files up to 1.5GB and it worked like a charm. Text/image stamping, text/image extraction, support for placing large data set, PDF to PDF/A conversion, PDF to DOC/DOCX, TIFF to PDF, PDF to TIFF and other functionalities are other areas in which we have made improvements.

Please download and evaluate the latest release. For further details on what's new and fixed in [Aspose.PDF for .NET 8.2.0][2].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net




