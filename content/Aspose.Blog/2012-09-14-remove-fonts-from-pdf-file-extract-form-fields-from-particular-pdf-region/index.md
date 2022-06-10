---
title: 'Remove Fonts from PDF and Extract Form Fields from Particular PDF Region in C#'
date: Fri, 14 Sep 2012 07:30:50 +0000
draft: false
url: /2012/09/14/remove-fonts-from-pdf-file-extract-form-fields-from-particular-pdf-region/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', '.NET', 'Acrobat', 'Center align image', 'Image stamping', 'Image to PDF', 'JavaScript', 'PDF', 'PNG to Image', 'Text stamping', 'XML to PDF', 'bindPCL', 'product release']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose.pdf-logo2.jpg" alt="Aspose.Pdf icon">}}


We are pleased to announce the release of [Aspose.PDF for .NET 7.3.0][1] which provides a new feature to remove duplicate/unused fonts from PDF documents. In order to replace fonts please use the following approaches:

  

*   Use TextFragmentAbsorber.
*   Use TextEditOptions.FontReplace.RemoveUnusedFonts parameter for TextFragmentAbsorber. (_The above parameter removes fonts that become unused during font replacement_).
*   Set font individually for each text fragment.

The following code snippet replaces font for all text fragments of all document pages and removes unused fonts.

```
Document doc = new Document(inFile); 
TextFragmentAbsorber absorber = new TextFragmentAbsorber(new TextEditOptions(TextEditOptions.FontReplace.RemoveUnusedFonts)); 
doc.Pages.Accept(absorber);
foreach (TextFragment textFragment in absorber.TextFragments) 
{ textFragment.TextState.Font = FontRepository.FindFont("Courier New"); 
}
doc.Save(outFile);
```

It also offers a new feature to extract form fields from a particular rectangular region of a PDF document. In order to fulfill this requirement, we have introduced the **GetFieldsInRect(Rectangle rect)** method to the Aspose.Pdf.Form class.

```
Document doc = new Document("d:/pdftest/FDA-3500_508+No+submit_Filled.pdf"); 
Aspose.Pdf.InteractiveFeatures.Forms.Field[] fields = doc.Form.GetFieldsInRect(new Aspose.Pdf.Rectangle(35, 703, 126, 753));
```

In this release version, we have also introduced the **Close(...)** method in all classes under the Aspose.Pdf.Facades namespace so that all resources occupied by these classes can be released.

Recently, a customer reported that when rotating the PDF page, the width and height information is not changed. To fulfill this requirement, we introduced the **Page.GetPageRect(bool considerRotation)** method to the Page class. So in order to get page rectangle with rotation, please call GetPageRect(true):

```
Document pdfDocument = new Document("d:/pdftest/HelloWorld.pdf");
//adds a blank page to pdf document Page page = pdfDocument.Pages.Count > 0 ? pdfDocument.Pages[1] : pdfDocument.Pages.Add(); 
Console.WriteLine(page.GetPageRect(true).Width.ToString() + ":" + page.GetPageRect(true).Height); page.Rotate = Rotation.on90; 
Console.WriteLine(page.GetPageRect(true).Width.ToString() + ":" + page.GetPageRect(true).Height);
```

Besides this, we have also resolved many issues related to PDF printing, conversion of HTML files into PDF format, form filling, text extraction and many more. Please visit the following link for further details on what's new & fixed in [Aspose.PDF for .NET 7.3.0][2].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net




