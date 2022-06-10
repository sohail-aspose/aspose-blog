---
title: 'Improvements in Fields, Rendering, Layout Features and New Members Added in Aspose.Words 14.8.0'
date: Thu, 11 Sep 2014 10:48:37 +0000
draft: false
url: /2014/09/11/improvements-in-fields-rendering-layout-features-and-new-members-added-in-aspose.words-14.8.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 14.8.0 has been released. This month’s release contains over 79 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 14.8.0][1]
*   [Aspose.Words for Java 14.8.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Improved how TOC field culture and formatting is handled.
*   Timestamping of PDF digital signatures using external timestamp server implemented.
*   Improvements to advanced rendering features, for example pre-blending semi-transparent images.
*   Horizontal rotation of characters with HorizontalRotatedFarEast orientation supported.
*   Improved page layout for additional compatibility modes.
*   Improved floater positioning in complex cases.

## Time Stamping of PDF Digital Signature using External Timestamp Server

The new property TimestampSettings has been added to PdfDigitalSignatureDetails. It allows you to timestamp a digital signature in a PDF document using an external timestamp server.

```
/// <summary>
/// Gets or sets the digital signature timestamp settings.
/// </summary>
/// <remarks>
/// <para>The default value is null and the digital signature will not be time-stamped.
/// When this property is set to a valid <see cref="PdfDigitalSignatureTimestampSettings"/> object,
/// then the digital signature in the PDF document will be time-stamped.</para>
/// </remarks>
public PdfDigitalSignatureTimestampSettings TimestampSettings
{
        get { return mTimestampSettings; }
        set { mTimestampSettings = value; }
} 
```
```
// Usage:
saveOptions.DigitalSignatureDetails.TimestampSettings = new PdfDigitalSignatureTimestampSettings(timestampServerUrl, userName, password, timeout); 
```

## PreblendImages Property Added to PdfSaveOptions Class

The PreblendImages property has been added to the PdfSaveOptions class. It may improve a PDF document's visual appearance in Adobe Reader and remove anti-aliasing artefacts.

```
/// <summary>
/// Gets or sets a value determining whether or not to preblend transparent images with black background color.
/// </summary>
/// <remarks>
/// <para>Preblending images may improve PDF document visual appearance in Adobe Reader and remove anti-aliasing artifacts.</para>
/// 
/// <para>In order to properly display preblended images, PDF viewer application must support /Matte entry in soft-mask image dictionary. 
/// Also preblending images may decrease PDF rendering performance.</para>
/// 
/// <para>The default value is false.</para&gt
/// </remarks>
public bool PreblendImages
{
    get { return mPreblendImages; }
    set { mPreblendImages = value; }
} 
```

## LinkedStyleName Property Added to Style Class

The following new public member is added to the Style class:

```
/// <summary>
/// Gets the name of the Style linked to this one. Returns Empty string if no styles are linked.
/// </summary>
public string LinkedStyleName 
```




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx




