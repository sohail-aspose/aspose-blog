---
title: 'Update Digital Signature Information in PDF using C#'
date: Sat, 27 Apr 2019 22:39:49 +0000
draft: false
url: /2019/04/27/change-signature-text-while-signing-pdf-digitally-using-aspose.pdf/
author: Asad Ali
summary: ''
tags: ['Asad Ali']
categories: ['Aspose.PDF Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2016/06/aspose-Pdf-for-net.png)Process of signing PDF documents has been commonly known and being practiced in many systems. Signatures are meant to secure documents and authenticate them. We can simple take example of a piece of paper where some information is written on. Now, if you do not find any reference of that information or any attestation mark over that paper, it would be hard to believe if information is correct. But, if any stamp or signature is present on the paper then you will definitely find that information as approved or from some authentic source. Similarly, signing a PDF document digitally approves that it is from a reliable source and content present in it is authenticated.

Signing PDF documents is one of the most used features offered by Aspose.PDF and because of many requests from its users, these features have been being enhanced and improved with each new revision of the API. In earlier versions of the API, signature text over the signature could not be changed and used to remain constant. The following image is showing how signature text displays in PDF viewer once the document is signed.

* * *



{{< figure align=center src="images/SignatureText-300x99.png" alt="">}}


* * *

[Aspose.PDF for .NET 19.4][1] enables you to change text and information of the digital signature which is visible in the PDF document. The signature text contains the following information:

*   Date Signed
*   Date Digitally Signed
*   Reason Label
*   Location Label

Along with changing or specifying the information mentioned above, you will also be able to specify the format of the Date as per your needs. The following code snippet shows the complete implementation of the functionality introduced in the latest version of the API.

{{< gist aspose-com-gists 63473b1ba28e09e229cfbf4430eabd8a "Examples-CSharp-AsposePdfFacades-Security-Signatures-ChangeLanguageInDigitalSignText-ChangeLanguageInDigitalSignText.cs" >}}

Furthermore, API has been revised with other new features and enhancements along with major fixes and improvements. Following list contains areas where the latest version of the API has been improved for performance and usability:

*   Support of Latex Script for mathematical expressions is added
*   You can now tag existing images in PDF for Accessibility feature
*   Structure element into text element can now be added
*   Concatenation scenarios have been improved
*   Rendering of HTML content inside PDF document has been further enhanced
*   Table manipulation and rendering have been further improved
*   PDF to PDF/A conversion engine has been improvised
*   Text replacement scenarios have been taken care of for better performance
*   Working with Annotation area is now better
*   PDF to XPS conversion engine has further been improved

Detailed information about all fixes and enhancements has been given in the [release notes][2] page of the API. In order to stay updated with every news about releases of the API, subscribe to our [blog][3]. Do not forget to post your inquiry in our [forum][4] in case you have some. We will be back soon with updates of future version(s) of the API.




[1]: http://nuget.org/packages/Aspose.PDF/19.4.0
[2]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+19.4+Release+Notes
[3]: https://blog.aspose.com/category/aspose-products/aspose-omr-product-family/
[4]: https://forum.aspose.com/c/pdf




