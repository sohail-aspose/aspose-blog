---
title: 'Track Word Wrapping and Line Breaking in Scenario of Editing PDF Documents'
date: Sun, 26 Aug 2018 21:04:06 +0000
draft: false
url: /2018/08/26/track-word-wrapping-and-line-breaking-in-scenario-of-editing-pdf-documents/
author: Asad Ali
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="">}}


It is our honor to announce the August Release of [Aspose.PDF for .NET 18.8][1] which is available for download over NuGet Gallery. The latest release of the API includes 20+ bug fixes reported in earlier versions of the API. Since the feature set of API has been being expanded with each new release, new features and enhancements are also part of this release. If you are planning to upgrade to the latest version of the API, we strongly recommend you please visit the [release notes page of Aspose.PDF for .NET 18.8][2] in the official documentation. All public API Changes, as well as improvements and enhancements, have been listed in the release notes. Following are some insights about what is new in the API:

## Track Word Wrapping and Line Breaking while Editing PDF Documents

In earlier version(s) of the API, support for identifying points/position was provided in which an “Enter” was added/pressed to create a line break. Logging and background processing of multi-line text fragments in text adding scenarios were implemented by introducing GetNotifications() method in Page Class. Also, it was promised that this feature would be improved in future releases of the API. Thus, tracking of word wrapping and line breaking is further improved and implemented in the latest release of the API.

Following code snippet shows a demonstration on how you can use this feature in your .NET Applications:

```
TextFragmentAbsorber textFragmentAbsorber = <br>new TextFragmentAbsorber("[Cname,companyname,Textbox,50]");
textFragmentAbsorber.TextReplaceOptions.ReplaceAdjustmentAction =
    TextReplaceOptions.ReplaceAdjustment.WholeWordsHyphenation;

Document doc = new Document("29224.pdf");
doc.Pages.Accept(textFragmentAbsorber);

foreach (TextFragment textFragment in textFragmentAbsorber.TextFragments)
{
    textFragment.Text = "This is a Lerger String to Testing of this issue";
}

string notifications1 = doc.Pages[1].GetNotifications();
File.WriteAllText("editing_notifications_sample_1.txt", notifications1);
```

## Support for Tagged PDF Documents

Since functionality to generate Tagged PDF documents has been under development, completed features have also been included in this release of the API. Following is the list of features related to Tagged (PDF/UA) PDF documents:

*   Headings validations have been implemented for PDF/UA
*   Implemented PDF/UA Tables Validations
*   Validations of Lists are included for PDF/UA
*   Writing correct file name attribute to validate log file has been added
*   Added warning and manual check levels to validation log
*   Validation of Notes and References has been implemented

## Miscellaneous Fixes

Along with the above-mentioned features, 26 fixes have also been incorporated in Aspose.PDF for .NET 18.8. Some important fixes and improvements include:

*   PDF to PPTX Conversion is improved
*   Text searching engine has been improved
*   Text replacement operation is further improved
*   PDF to Image Conversion is improved
*   Image to PDF Conversion issues are resolved
*   Sizing issues of SVG inside PDF document have been fixed
*   API is improved to generate PDF/A Compliant documents

## Aspose.PDF for .NET Resources

As it is always recommended to use latest releases of our API’s, so we suggest you to please download the latest release [Aspose.PDF for .NET 18.8][3] and check following resources which will help you working with API:

*   [Home page for Aspose.PDF for .NET][4]
*   [Download Aspose.PDF for .NET 18.8][5]
*   [Aspose.PDF product family forum][6]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for .NET online documentation][7]– help documentation and API reference documents.
*   [Enable Blog Subscription][8]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Pdf/18.8.0
[2]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+18.8+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Pdf/18.8.0
[4]: https://products.aspose.com/pdf/net
[5]: https://www.nuget.org/packages/Aspose.Pdf/18.8.0
[6]: https://forums.aspose.com/c/pdf
[7]: https://docs.aspose.com/display/pdfnet/Home
[8]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[9]: https://github.com/aspose-pdf/Aspose.PDF-for-.NET




