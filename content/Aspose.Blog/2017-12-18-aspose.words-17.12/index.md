---
title: 'Use Aspose.Words in .NET Standard 2.0, Set Chart Axis Properties using C# .NET'
date: Mon, 18 Dec 2017 08:22:05 +0000
draft: false
url: /2017/12/18/aspose.words-17.12/
author: Tahir Manzoor
summary: ''
tags: ['.NET Word API for .NET Core', '.NET Word Library', 'Word API for .NET Core', 'Word API for .NET Standard']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 17.12][1]. This month’s release contains over 84 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Implemented Aspose.Words for .NET Standard 2.0.
*   Implemented API to set chart axis properties.
*   Added feature to get the docPartGallery value of StructuredDocumentTag of type SdtType.DocPartObj.
*   Horizontal and vertical flipping attributes are now taken into account when rendering DML textboxes.
*   Improved rendering of diacritics for "Courier New" font.
*   Multiline MathML expressions rendering fixed.
*   EMR\_ROUNDRECT records processing while rendering metafiles fixed.
*   PDF Rendering of indexed images while converting to CMYK color space fixed.
*   Fixed bug causing freezes when converting document with DML Charts to PDF in debug x86 mode.
*   OTF(CFF) fonts to PDF/A documents export fixed.
*   DML Charts with empty area do not throw exception on rendering now.
*   Fixed scaling problem with DML bubble charts on rendering.
*   LINQ Reporting Engine supports dynamic setting of chart axes’ titles.
*   Improved handling of decimal tab alignment in cells when paragraph has hanging indent.
*   Improved text wrapping when line contains single or no characters.
*   Improved handling of cell margins and table alignment.
*   Improved cell alignment when line has trailing spaces and custom tabs.
*   Improved handling of collapsed paragraphs.
*   Fixed exception in rare case when line break point cannot be found.
*   Fixed exception when document is saved with revision balloons inside of a cell.

## Included Aspose.Words for Android via Xamarin, Aspose.Words for iOS via Xamarin and Aspose.Words for Mac via Xamarin in Aspose.Words for .NET

Now, Aspose.Words for .NET includes Aspose.Words for Android via Xamarin, Aspose.Words for iOS via Xamarin and Aspose.Words for Mac via Xamarin. Following breaking changes have been made:

*   External reference to SkiaSharp has been added (in previous versions SkiaSharp was merged into Aspose.Words for Xamarin dlls)
*   Native graphics objects (Android.Graphics.Bitmap and Android.Graphics.Canvas in Aspose.Words for Android via Xamarin version and CoreGraphics.CGImage and CoreGraphics.CGContext in Aspose.Words for iOS via Xamarin and Aspose.Words for Mac via Xamarin) has been replaced in public API with SkiaSharp.SKBitmap and SkiaSharp.SKCanvas accordingly. This allowed us to fully unify public API of all Aspose.Words for Xamarin versions. Code written for one platform can be reused on another without any changes.

## Implemented Aspose.Words for .NET Standard 2.0

Starting from this release, Aspose.Words for .NET includes .NET Standard 2.0 version. It has full functionality of regular .NET version of Aspose.Words with few limitations and public API difference:

*   Saving to BMP is not yet supported.
*   Signing of PDF document is not yet supported.
*   Printing feature is not provided in .NET Standard
*   Saving to user browser is not provided, i.e. Document.Save(HttpResponse,string,ContentDescription,SaveOptions) overload is not available.
*   Public API differences are the same as in Xamarin versions, i.e. SkiaSharp.SKBitmap and SkiaSharp.SKCanvas are used as native graphics objects instead of System.Drawing.Bitmap and System.Drawing.Graphics.

## Implemented API to Set Chart Axis Properties

We have added public classes [ChartAxis][4], [AxisDisplayUnit][5], [AxisScaling][6] and following enumeration in this release to allow setting chart axis properties.

*   [ChartAxisType][7]
*   [AxisCategoryType][8]
*   [AxisCrosses][9]
*   [AxisTickLabelPosition][10]
*   [AxisTickMark][11]
*   [AxisTimeUnit][12]
*   [AxisBuiltInUnit][13]
*   [AxisScaleType][14]

Please check the examples from following documentation link.  
[How to Set Chart Axis Properties][15]

## Added Feature to Get the docPartGallery Value of StructuredDocumentTag of Type SdtType.DocPartObj

We have improve the behavior of following properties. Now, you can get the value of these properties for "Markup.SdtType.DocPartObj" SdtType.

```
public class StructuredDocumentTag
{
    .....
    public string BuildingBlockGallery{ get; set;}
    public string BuildingBlockCategory{get; set;}
    .....
}
```

## Changed Return Type for FieldMergingArgsBase.Field

We have provided typed access to a merge field's properties in this release of Aspose.Words. We have changed the return type of the FieldMergingArgsBase.Field property (and hence of the corresponding descendants' properties) from Field to FieldMergeField. Please refer to the following article for more detail.  
[How to Handle Text Before and After Switches During Mail Merge Operation][16]

```
/// <summary>
/// Gets the object that represents the current merge field.
/// </summary>
public FieldMergeField Field
{
    get { return mField; }
}
```

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][17].
2.  [Install using NuGet Package][18]
3.  [Documentation][19] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
4.  [API Reference Guide][20] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
5.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][21]
    *   [Paid Support Forum][22]
6.  [Enable Blog Subscription][23] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
7.  [Examples][24] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Words/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+17.12+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/chartaxis
[5]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/axisdisplayunit
[6]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/axisscaling
[7]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/chartaxistype
[8]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/axiscategorytype
[9]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/axiscrosses
[10]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/axisticklabelposition
[11]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/axistickmark
[12]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/axistimeunit
[13]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/axisbuiltinunit
[14]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/axisscaletype
[15]: https://docs.aspose.com/display/wordsnet/Working+with+Charts#WorkingwithCharts-HowtoSetChartAxisProperties
[16]: https://docs.aspose.com/display/wordsnet/How+to+Execute+Mail+Merge#HowtoExecuteMailMerge-HowtoHandleTextBeforeandAfterSwitchesDuringMailMergeOperation
[17]: https://products.aspose.com/words/net
[18]: https://www.nuget.org/packages/Aspose.Words/
[19]: https://docs.aspose.com/display/wordsnet
[20]: https://apireference.aspose.com/net/words
[21]: https://forum.aspose.com/c/words
[22]: https://helpdesk.aspose.com/
[23]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[24]: https://github.com/aspose-words/Aspose.Words-for-.NET




