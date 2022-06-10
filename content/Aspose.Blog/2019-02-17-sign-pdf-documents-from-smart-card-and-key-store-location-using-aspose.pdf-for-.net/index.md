---
title: 'Add Digital Signature to PDF from Smart Card and Key Store Location in C# .NET'
date: Sun, 17 Feb 2019 01:22:36 +0000
draft: false
url: /2019/02/17/sign-pdf-documents-from-smart-card-and-key-store-location-using-aspose.pdf-for-.net/
author: Asad Ali
summary: ''
tags: ['Asad Ali']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="">}}


February release of Aspose.PDF for .NET has been rolled out and is thriving with exciting features and enhancements. Our efforts to implement the most requested functionalities have brought up the API this far that its feature set has become such enriched and appealing. Being a specialized API in order to process PDF documents, [Aspose.PDF for .NET 19.2][1] brings more interesting features in this revision. In this post, we will be going to explore what is new in this release and having insights into further improvements. Without waiting so much, let’s learn what this update of the API offers and how it can be consumed to perform newly introduced functionalities.

## Add Digital Signature to PDF from a Smart Card

Signing PDF documents with digital signatures is a common exercise when you intend to secure them. This functionality can be achieved using Adobe Reader by following “[Adding Signatures and Security][2]” guide. In the referred guide, you can notice that all steps are performed manually by using Adobe Reader. But, automating this entire process and getting this done programmatically sounds more efficient and time-saving. Isn’t it? At this point, Aspose.PDF can definitely save you big time from efforts. Those who are already users of the API may know that it offers functionality to [digitally sign PDF documents][3] as well as certify them using the PFX file.

Well, extending its feature set in the region of signing and security, Aspose.PDF for .NET now offers the functionality to add digital signatures from a key store location. This means you will be able to apply the signature by accepting the certificate provided by the certificate store, smart card or [PIV card][4] connected to the system at run-time. All of the mentioned functionality can be achieved by just using following simple code snippet(s):

### Using Signature Field{{< gist aspose-com-gists 63473b1ba28e09e229cfbf4430eabd8a "Examples-CSharp-AsposePDF-aa-SignWithSmartCardUsingSignatureField-1.cs" >}}

### Using PdfFileSignaure{{< gist aspose-com-gists 63473b1ba28e09e229cfbf4430eabd8a "Examples-CSharp-AsposePDF-aa-SignWithSmartCardUsingPdfFileSignature-1.cs" >}}

## Major Enhancements for Creating Tagged PDFs

We are not yet done with the updates this release of the API has brought. There have been many requests for the feature to create Tagged PDFs (PDF/UA) which is finally offered by the API. With every release of the API, this feature is being richer with useful enhancements. You can now achieve the following by using this release of the API:

*   [Styling Text Structure][5]: Support of setting text style for structure elements was implemented to TaggedPdf. Access to necessary property performs through **StructureTextState** property of **StructureElement**. (Only for Structure Element which implements the **ITextElement** interface). All properties can be null. Use null to inherit necessary property from parent Structure Element. (Default value is null).
*   [Access Structure Elements Attributes][6]: Access to structure elements attributes was implemented to **TaggedPdf**. **StructureAttributeCollection**, **StructureAttributes,** and **StructureAttributes** classes are intended for work with attributes. **AttributeOwnerStandard**, **AttributeKey** and **AttributeName** classes contain valid values for corresponding entities.
*   [Illustrate Structure Elements][7]

## Useful Improvements and Fixes

As per the history of monthly API revisions, this release of the API has also been improved for performance and usability. Following is the list of useful improvement and fixes in Aspose.PDF for .NET 19.2:

*   HTML to PDF Conversion Engine has been further improved
*   Text Extraction scenarios have been taken care of to return precise coordinates
*   Memory consumption in processing text paragraphs has been optimized
*   API is further improved to work in non-windows platforms
*   Inter-File format conversion is further improved
*   Text replacement and searching scenarios have been improved

It would surely be exciting to use API with such above mentioned improvements, enhancements and of course new features. Now you must have a pretty good idea of what’s new in the API and how it can improve your experience to automate PDF documents processing.

Well, the story does not end here as you can also check the [release notes page][8] of this release of the API for every minor detail of the updates. In case you still have inquiries in this regard, you are most welcome to post them in our [forums][9]. For more exciting features and news, [stay tuned with us][10].




[1]: https://www.nuget.org/packages/Aspose.PDF/19.2.0
[2]: http://www.adobepress.com/articles/article.asp?p=1272495&seqNum=6 "Adding Signatures and Security"
[3]: https://docs.aspose.com/display/pdfnet/Digitally+sign+PDF+file "Digitally Sign PDF"
[4]: https://whatis.techtarget.com/definition/personal-identity-verification-PIV-card "PIV Cards"
[5]: https://docs.aspose.com/display/pdfnet/Create+Tagged+PDF+Documents#CreateTaggedPDFDocuments-StylingTextStructure "Styling Text Structure"
[6]: https://docs.aspose.com/display/pdfnet/Create+Tagged+PDF+Documents#CreateTaggedPDFDocuments-CreatingStructureElements "Access Structure Elements"
[7]: https://docs.aspose.com/display/pdfnet/Create+Tagged+PDF+Documents#CreateTaggedPDFDocuments-IllustratingStructureElements "Illustrate Structure Elements"
[8]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+19.2+Release+Notes "Aspose.PDF for .NET 19.2 Release Notes"
[9]: https://forum.aspose.com/c/pdf "Aspose.PDF Forums"
[10]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/ "Aspose Blog Subscription"




