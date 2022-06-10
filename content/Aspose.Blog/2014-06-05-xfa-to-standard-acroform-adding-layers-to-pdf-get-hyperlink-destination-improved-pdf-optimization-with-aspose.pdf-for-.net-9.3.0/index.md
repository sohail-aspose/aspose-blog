---
title: 'Add Layers to PDF and Get Hyperlink Destination in C# - Aspose.PDF for .NET 9.3.0'
date: Thu, 05 Jun 2014 18:54:33 +0000
draft: false
url: /2014/06/05/xfa-to-standard-acroform-adding-layers-to-pdf-get-hyperlink-destination-improved-pdf-optimization-with-aspose.pdf-for-.net-9.3.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Add layers to PDF in Csharp', 'Convert dynamic XFA to Standard AcroForm', 'Csharp PDF API']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


The Aspose team is always happy to introduce new and exciting features to its APIs, where the main intent is to provide out of the box APIs that make the lives of developers worldwide easier. We create tools that means our customers don't have to do much of the tedious work required during document manipulation. We always thrive to present products that are simple and easy to use, so that our customers can focus on their business logic and forget about inner details and implementations. All our products are quality orientated, up to industry standards and undergo thorough testing before they are released.

Aspose.PDF for .NET is an award-winning API. Over the years it helped developers with PDF document creation as well as manipulation. In every new release, the development team works really hard to introduce new features and fix issues to deliver a better version of the API. Keeping this tradition alive, we have introduced some new features in [Aspose.PDF for .NET 9.3.0][1].

## Adding Layer to an Existing PDF

Adding layers to a PDF is a unique concept. It can be very useful for cases where you want to distribute multi-lingual file and want text in each language to appear on different layers, with the background design appearing on a separate layer. Aspose.Pdf for .NET 9.3.0 supports adding layers to PDF documents. For further information, please read the article [Add Layers to PDF File][2].

## Getting Hyperlink Destination

Hyperlinks are added as LinkAnnotation in PDF files. Aspose.Pdf for .NET supports the feature to [add a hyperlink to a PDF file][3], update links, and extract links. It can also get the destination URL of a LinkAnnotation (hyperlink) in PDF documents. To get a link's destination URL, get the LinkAnnotation Action as GoToURIAction. For further details, see [Get PDF Hyperlink Destination (URL)][4].

## Dynamic XFA to Standard AcroForm Conversion

Dynamic forms are based on an XML specification known as XFA, the “XML Forms Architecture”. The information about the form (as far as PDF is concerned) is very vague – it specifies that fields exist, with properties, and JavaScript events, but does not specify any rendering. The contents of such forms are rendered during the PDF display process by respective viewer application. Due to this nature and structure of the forms, if we directly try to convert it to image format, nothing is rendered. Therefore, the forms have to be converted to Standard AcroForms first and then to image. Aspose.Pdf for .NET supports the feature to convert XFA forms to standard forms. In order to cater for this requirement, the values from an enumeration named FormType can be passed to the Document.Form.Type property. For further details, please follow the instructions in the article [Convert Dynamic XFA form to Standard AcroForm][5].

## Set Document Access Privileges using Aspose.Pdf DOM

The Aspose.Pdf.Generator namespace makes it possible to create PDF files from scratch. During PDF creation, you might want to [set document access privileges (restrictions)][6]. Similarly, Aspose.Pdf.Facades namespace has offered the feature to set document access privileges to existing PDF documents for quite some time. Recently, we were asked to support a similar feature in the new Document Object Model of the Aspose.Pdf namespace, so that a single approach can be used to set access privileges when creating new documents or manipulating existing files. For further details, please visit the article Set Privileges on an Existing PDF File.

## Remove Signature and Keep Signature Field

The RemoveSignature() method in the PdfFileSignature class provides the capability to remove the signature field from PDF files. When using this method with versions prior to 9.3.0, it removes both the signature and signature fields. We received a requirement for removing only the signature and keeping the signature field so that the same field can be used to sign the document again. To keep the signature field and only remove the signature, please use the following code snippet.

```
private static void Run_34561_tests()
{
    new License().SetLicense(@"E:\Aspose.Pdf.lic");
    string inSingleSignedFile = @"C:\pdftest\PDFNEWNET_34561_SingleSigned.pdf";
    string outSingleUnsignedFile = @"C:\pdftest\PDFNEWNET_34561_SingleUnSigned.pdf";
    string inOutSingleResignedFile = @"C:\pdftest\PDFNEWNET_34561_SingleReSigned.pdf";

    PdfFileSignature pdfSignSingle = new PdfFileSignature();
    pdfSignSingle.BindPdf(inSingleSignedFile);
    IList names = pdfSignSingle.GetSignNames();
    Stream pfx = new FileStream(@"C:\pdftest\test1.pfx", FileMode.Open);
    PKCS7 pcks = new PKCS7(pfx, "test1");
    string sigNameSingle = names[0] as string;
    if (sigNameSingle != null && sigNameSingle != string.Empty)
    {
        pdfSignSingle.RemoveSignature(sigNameSingle, false);
        pdfSignSingle.Save(outSingleUnsignedFile);

        PdfFileSignature pdfSignSingle2 = new PdfFileSignature();
        pdfSignSingle2.BindPdf(outSingleUnsignedFile);
        pdfSignSingle2.SignatureAppearance = @"C:\pdftest\butterfly.jpg";
        pdfSignSingle2.Sign("Signature1", pcks);
        pdfSignSingle2.Save(inOutSingleResignedFile);
        pdfSignSingle2.BindPdf(inOutSingleResignedFile);
        // Assert.True(pdfSignSingle2.VerifySignature("Signature1"));
        Console.Write("Signature 1 check result : " + pdfSignSingle2.VerifySignature("Signature1").ToString() + " \n");
    }

    // Test file with multiple signatures
    string inManySignedFile = @"C:\pdftest\PDFNEWNET_34561_ManySigned.pdf";
    string outManyUnsignedFile = @"C:\pdftest\PDFNEWNET_34561_ManyUnSigned.pdf";
    string inOutManyResignedFile = @"C:\pdftest\PDFNEWNET_34561_ManyReSigned.pdf";
    PdfFileSignature pdfSignMany = new Aspose.Pdf.Facades.PdfFileSignature(inManySignedFile);

    IList sigNames = pdfSignMany.GetSignNames();
    foreach (string sigName in sigNames)
    {
        pdfSignMany.RemoveSignature(sigName, false);
    }

    pdfSignMany.Save(outManyUnsignedFile);

    PdfFileSignature pdfSignMany2 = new PdfFileSignature();
    pdfSignMany2.BindPdf(outManyUnsignedFile);
    pdfSignMany2.Sign("Signature1", pcks);
    pdfSignMany2.Save(inOutManyResignedFile);
    pdfSignMany2.BindPdf(inOutSingleResignedFile);
    //Assert.IsTrue(pdfSignMany2.VerifySignature("Signature1"));
    Console.Write("Signature 2 check result : " + pdfSignMany2.VerifySignature("Signature1").ToString() + " ");
}
```

More details can be found in the article [Remove Digital Signature from the PDF File (Facades)][7]

## Generate 3 Sets of Fonts to Ensure Maximum Browser Compatibility

Prior to the release of Aspose.Pdf for .NET 9.3.0, the API supported the feature to either save fonts as WOFF or TTF. Unfortunately, this meant that fonts could not be loaded in Internet Explorer 6 through 8, so documents didn't look right when viewed in these browsers. Also for mobile browsers, TTF fonts are required for maximum compatibility. So the solution was to generate 3 sets of fonts, to ensure maximum browser compatibility, and then reference all fonts in the CSS like as shown below. The following format is similar somewhat to that described in [this link][8].

```
@font-face {
	font-family:"WBULFR+Arial-BoldMT";
	src:url("fa507958-0001-0000-0000-000000000000.eot");
	src:url("fa507958-0001-0000-0000-000000000000.eot?#iefix") format("embedded-opentype"),
	url("fa507958-0001-0000-0000-000000000000.woff") format("woff"),
	url("fa507958-0001-0000-0000-000000000000.ttf") format("truetype");
}
```

To accomplish this requirement, the SaveInAllFormats font saving mode is introduced to the HtmlSaveOptions.FontSavingModes enumeration. The following code snippet demonstrates how to generate 3 sets of fonts:

```
string inPdf = @"F:\ExternalTestsData\36192.pdf";
string outHtml = @"F:\ExternalTestsData\36873.html";

Document doc = new Document(inPdf);
HtmlSaveOptions htmlOptions = new HtmlSaveOptions();
htmlOptions.FixedLayout = true;
htmlOptions.RasterImagesSavingMode = HtmlSaveOptions.RasterImagesSavingModes.AsExternalPngFilesReferencedViaSvg;
htmlOptions.FontSavingMode = HtmlSaveOptions.FontSavingModes.SaveInAllFormats;

doc.Save(outHtml, htmlOptions);
```

Further details regarding this feature can be found in the article [PDF to HTML –][9] [Save Fonts as WOFF or TTF][10].

As well as the new features above, this new version includes fixes related to PDF to image conversion, saving PDF files in a particular PDF version, deleting images from PDF files, performance improvements when generating PDF files and much more. Go ahead, download and start exploring the new release of [Aspose.PDF for .NET 9.3.0.][11]




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Manipulate+PDF+Document
[3]: https://docs.aspose.com/display/pdfnet/Add+and+Get+Hyperlink
[4]: https://docs.aspose.com/display/pdfnet/Add+and+Get+Hyperlink#AddandGetHyperlink-GetPDFHyperlinkDestination(URL)
[5]: https://docs.aspose.com/display/pdfnet/Working+with+XFA+Forms
[6]: http://docs.aspose.com/display/pdfnet/Allow+or+Disallow+Privileges+on+PDF+Document
[7]: https://docs.aspose.com/display/pdfnet/Working+with+Signature+in+a+PDF+File
[8]: http://css-tricks.com/snippets/css/using-font-face/
[9]: https://docs.aspose.com/display/pageproductfamily/Home
[10]: https://docs.aspose.com/display/pdfnet/Convert+PDF+File+into+HTML+Format#ConvertPDFFileintoHTMLFormat-PDFtoHTML-SaveFontsasWOFForTTF
[11]: https://downloads.aspose.com/pdf/net




