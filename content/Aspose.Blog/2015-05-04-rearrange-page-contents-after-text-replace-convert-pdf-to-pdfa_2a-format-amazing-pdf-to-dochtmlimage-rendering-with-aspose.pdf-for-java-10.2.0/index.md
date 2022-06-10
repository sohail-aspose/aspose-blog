---
title: 'Rearrange Page Contents after Text Replace, Convert PDF to PDF/A_2a Format, PDF to DOC/HTML/Image with Aspose.PDF for Java 10.2.0'
date: Mon, 04 May 2015 09:15:19 +0000
draft: false
url: /2015/05/04/rearrange-page-contents-after-text-replace-convert-pdf-to-pdfa_2a-format-amazing-pdf-to-dochtmlimage-rendering-with-aspose.pdf-for-java-10.2.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for Java logo">}}


A new release of [Aspose.PDF for Java 10.2.0][1] is published which brings some new features for PDF manipulation. Among these new features, we always strive to make this API robust enough that it can fulfill most of our customers' requirements and works without any problem on various configurations. We are pretty much aware that the transformation of one file format to another is not an easy task because each format has particular specifications and the rendering mechanism should preserve data, as well formatting when saving the resultant files. Keeping all these perspectives in mind, we have made our API capable enough to convert various file formats (including SVG, HTML, Image, etc) to PDF format as well as render PDF files to DOC, HTML, Image, XPS, etc with great fidelity. These transformation features are one of the salient features being offered by our API and they are endorsed by many clients.

## PDF to PDF/A\_2a Conversion

Conversion of PDF to PDF/A compliant documents has been supported by our API for quite some time and in this new release, we have introduced the support for PDF files to PDF/A\_2a compliant format. In order to accomplish this requirement, a new value **PDF\_A\_2A** is added in **PdfFormat** enumeration. For further details, please visit [Convert PDF to PDF/A format][2].  
Please take a look over the following code snippet to convert PDF files to PDF/A\_2a compliant format.

```
//Open document
Document doc = new Document("d:\\input.pdf");
//Convert to PDF/A2_a compliant document
doc.convert("log.log", PdfFormat.PDF_A_2A, com.aspose.pdf.ConvertErrorAction.Delete);
//Save resultant document
doc.save("d:\\output.pdf");
```

## Auto Arrange Page Contents after Text Replace

Portable Document Format is one of the complex file formats when it comes to file manipulation as some of the contents placed inside file have relative and others may have obsolete positioning. So during PDF file manipulation, the contents of a file might be updated, which may result in extra space besides various elements or the objects may overlap each other due to space limitations. Keeping these issues in mind, we have optimized the text replacement mechanism of our API so that if the text inside PDF file is being replaced with small string or if file contents are being replaced with large string(TextFragment), the existing elements over a page will automatically adjust them, so that formatting of the document is preserved. For more information, we recommend you to visit [Text Replacement should automatically re-arrange Page contents][3].

```
//Load source PDF file
Document doc = new Document(myDir+"input.pdf");
//Create TextFragment Absorber object with regular expression
TextFragmentAbsorber textFragmentAbsorber = new TextFragmentAbsorber("[Cname,companyname,Textbox,50]");
doc.getPages().accept(textFragmentAbsorber);
//Replace each TextFragment
for (TextFragment textFragment : (Iterable)textFragmentAbsorber.getTextFragments())
{
    // Set font of text fragment being replaced
    textFragment.getTextState().setFont (FontRepository.findFont("Arial"));
    // Set font size
    textFragment.getTextState().setFontSize (12);
    textFragment.getTextState().setForegroundColor (com.aspose.pdf.Color.getNavy());
    // Replace the text with larger string than placeholder
    textFragment.setText ("This is a Lerger String to Testing of this issue");
}
//Save resultant PDF
doc.save(myDir+"29860_out_large_NoHyphenation_1020.pdf");
```

## Miscellaneous fixes

As well as the enhancements and features discussed above, there have been numerous fixes related to recently introduced PDF to TIFF and TIFF to PDF conversion, adding watermark/stamp objects, better support for UniCode characters, working with Annotations, printing PDF documents, SVG to PDF conversion and much more. Please download and try the latest [Aspose.PDF for Java 10.2.0][4] release.




[1]: https://downloads.aspose.com/pdf/java
[2]: http://docs.aspose.com/display/pdfjava/Convert+PDF+to+PDF-A+format
[3]: https://docs.aspose.com/display/pdfjava/Replace+Text+in+a+PDF+Document
[4]: https://downloads.aspose.com/pdf/java




