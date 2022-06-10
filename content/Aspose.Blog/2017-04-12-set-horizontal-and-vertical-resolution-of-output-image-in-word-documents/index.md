---
title: 'Set Horizontal and Vertical Resolution of Output Image in Word Documents'
date: Wed, 12 Apr 2017 10:20:51 +0000
draft: false
url: /2017/04/12/set-horizontal-and-vertical-resolution-of-output-image-in-word-documents/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We are pleased to announce our next version of Aspose.Words 17.4. This month’s release contains over 80 useful new features, enhancements and bug fixes. You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 17.4][1]
*   [Aspose.Words for Java 17.4][2]

Please see the [release notes][3] for more detail. If you are planning to upgrade from an older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][4] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   CompareOptions class introduced to allow customer specify comparison settings.
*   Custom Xml Data Properties is now supported for RTF format.
*   Implemented support for baseline alignment in Asian text.
*   Improved table split for vertically merged cells in combination with at-least height.
*   Improved table grid calculation for horizontally merged cells.
*   Improved BalanceSingleByteDoubleByteWidth handling.
*   The horizontal and vertical resolution of output images can now be specified separately (through ImageSaveOptions.VerticalResolution and ImageSaveOptions.HorizontalResolution).
*   Underline, strikethrough, text borders and effects are now taken into account wile rendering OfficeMath equation text.
*   A substitution of fonts with the same name but with different suffixes now generates a proper warning.
*   Textboxes with automatic fit is now rendered correctly inside the group shapes.
*   Corrupted texture images do not stop the rendering procedure with an exception, a warning is sent instead now.
*   DrawingML Charts rendering improved (rotated and scaled horizontal axis labels).

## Added an Interface to Flexibly Format Field Result

We have implemented a more generic and flexible solution to format field result. We have added an interface IFieldResultFormatter in Aspose.Words 17.4 allowing to implement custom formatting of field's result. Now, you can apply formatting to numeric and date/time field result. Please read the following article for more detail:  
[How to Apply Custom Formatting to Field Result][5]

## Added Feature to Set Horizontal and Vertical Resolution of Output Image

Previously it was one property ImageSaveOptions.Resolution that set both vertical and horizontal resolution to the same values. We have added new public properties HorizontalResolution and VerticalResolution in ImageSaveOptions class to set horizontal and vertical resolution of output image. Please refer to the following article:  
[How to Save Document's Page to Image with Horizontal and Vertical Resolution][6]

```
/// <summary>
/// Gets or sets the horizontal resolution for the generated images, in dots per inch.
/// </summary>
/// <remarks>
/// <para>This property has effect only when saving to raster image formats.</para>
/// The default value is 96.
/// </remarks>
public float HorizontalResolution {get;set;}
 
 
/// <summary>
/// Gets or sets the vertical resolution for the generated images, in dots per inch.
/// </summary>
/// <remarks>
/// <para>This property has effect only when saving to raster image formats.</para>
/// The default value is 96.
/// </remarks>
public float VerticalResolution {get;set;}
```

Please note that ImageSaveOptions.Resolution property became write-only.

```
/// <summary>
/// Sets both horizontal and vertical resolution for the generated images, in dots per inch.
/// </summary>
/// <remarks>
/// <para>This property has effect only when saving to raster image formats.</para>
/// </remarks>
public float Resolution {set;}
```

## Added Feature to Ignore Document formatting and Header Footer Content during Document Comparison

We have introduced new class CompareOptions in Aspose.Words 17.4 to compare two documents with advanced options. Now, you can ignore document formatting and header footer content during document comparison. Please check following article for more detail:  
[Compare Word Documents and Ignore Document Formatting][7]  

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

*   [Home of Aspose.Words for .NET API][8].
*   [Aspose.Words for .NET Download Section][9].
*   [Aspose.Words for .NET Documentation][10] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [Aspose.Words for .NET API Reference Guide][11] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Words Product Family Forum][12] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
*   [Enable Blog Subscription][13] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for .NET Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+17.4+Release+Notes
[4]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+17.4+Release+Notes
[5]: https://docs.aspose.com/display/wordsnet/Updating+and+Removing+a+Field#UpdatingandRemovingaField-HowtoApplyCustomFormattingtoFieldResult
[6]: https://docs.aspose.com/display/wordsnet/Rendering#Rendering-HowtoSaveDocument'sPagetoImagewithHorizontalandVerticalResolution
[7]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-CompareWordDocumentsandIgnoreDocumentFormatting
[8]: https://www.aspose.com/products/words/net
[9]: http://downloads.aspose.com/words/net
[10]: https://docs.aspose.com/display/wordsnet
[11]: https://apireference.aspose.com/net/words
[12]: https://www.aspose.com/community/forums/aspose.words-product-family/75/showforum.aspx
[13]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[14]: https://github.com/aspose-words/Aspose.Words-for-.NET




