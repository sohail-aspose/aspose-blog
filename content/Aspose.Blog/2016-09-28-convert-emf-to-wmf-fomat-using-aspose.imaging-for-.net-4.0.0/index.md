---
title: 'Convert EMF to WMF Fomat using C# or VB.NET'
date: Wed, 28 Sep 2016 19:44:44 +0000
draft: false
url: /2016/09/28/convert-emf-to-wmf-fomat-using-aspose.imaging-for-.net-4.0.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Imaging for .NET][1] 4.0.0. The major development in this release is support for converting EMF to WMF metafile image.

## Convert EMF to WMF Metafile Image using C#

Aspose.Imaging for .Net now supports converting EMF metafile image to WMF format. Below provided sample code demonstrates how simple it is to convert EMF metafile to WMF format.

```
string inputFileName = @"TestEmfPlusFigures.emf";
string outputFileName = inputFileName + ".wmf";

// Load an existing EMF file as Image.
using (Image image = Image.Load(inputFileName))
{
      // Call the Save method of Image class.
     //  Pass instance of WmfOptions class to Save method.
     image.Save(outputFileName,new WmfOptions());
}
```

## Enhancements

The following enhancements have been introduced in this release.

*   Process to get Height & Width of WMF image has been improved.
*   Process to extract file format using GetFileFormat property of Image class has been improved.
*   Process of extracting layer/nested layers name in PSD file has been improved.
*   Process of manipulating large TIFF files (e.g. size 500MB) has been improved.

Please refer to the release notes of [Aspose.Imaging for .NET 4.0.0][2] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the Public API Change section to know what has been changed in the public API since your current version.

## Aspose.Imaging for .Net Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for .Net API][3].
*   [Download Aspose.Imaging for .NET][4].
*   [Aspose.Imaging for .NET online documentation][5] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][9] for a chat.




[1]: https://products.aspose.com/imaging/net
[2]: https://downloads.aspose.com/imaging/net
[3]: https://products.aspose.com/imaging/net
[4]: https://downloads.aspose.com/imaging/net
[5]: https://docs.aspose.com/imaging/net
[6]: http://forum.aspose.com
[7]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[8]: https://github.com/aspose-imaging/Aspose.Imaging-for-.NET
[9]: http://forum.aspose.com




