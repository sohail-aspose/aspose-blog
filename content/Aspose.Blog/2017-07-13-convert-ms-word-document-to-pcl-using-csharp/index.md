---
title: 'Convert MS Word Document to PCL using C#'
date: Thu, 13 Jul 2017 11:10:49 +0000
draft: false
url: /2017/07/13/convert-ms-word-document-to-pcl-using-csharp/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)We are pleased to announce our next version [Aspose.Words for .NET 17.7][1]. This month’s release contains over 82 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from an older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Rendering into PCL format (Printer Command Language) has implemented. New saving format introduced – “SaveFormat.Pcl”. Please note that custom fonts is not yet supported.
*   The proper algorithm for rendering of shapes with automatic size textboxes (i.e. closest to MS Word output) implemented.
*   The rendered PDF documents can now show the document title in the title bar of the viewer. This is controlled by “PdfSaveOptions.DisplayDocTitle” property.
*   Improved font rendering in PDF documents for Adobe Illustrator limitations.
*   Improved rendering of fonts with simulated bold style.
*   Vertical text rendering in DrawingML textboxes improved.
*   Problem with rendering of numbers on horizontal axis in DrawingML Charts fixed.
*   Implemented support for "Wrap trailing spaces to next line" option.
*   Implemented support for footnote continuation notices.
*   Improved text wrapping logic for "2013 and later" documents.
*   Improved non-breaking space width calculation.
*   Improved Asian text justification logic.

## Convert Word Document to PCL using C#

We have introduced new saving format - PCL (Printer Command Language) in Aspose.Words for .NET 17.7. Aspose.Words can save documents to PCL 6 (PCL 6 Enhanced or PCL XL) format. There is one major feature of PCL that is unsupported in current version of Aspose.Words i.e. custom fonts. It is rather big and complex problem, but we will implement this feature in future. We have added new value to enum SaveFormat:

```
SaveFormat.Pcl
```

Please check the code example from here:   
[Save Document to PCL][4]

PclSaveOptions has following public options and methods:

```
/// <summary>
/// Gets or sets a value determining whether or not complex transformed elements
/// should be rasterized before saving to PCL document.
/// Default is <c>true</c>.
/// </summary>
/// <remarks>
/// PCL doesn't support some kind of transformations that are used by Aspose Words.
/// E.g. rotated, skewed images and texture brushes. To properly render such elements
/// rasterization process is used, i.e. saving to image and clipping.
/// This process can take additional time and memory.
/// If flag is set to <c>false</c>, some content in output may be different
/// as compared with the source document.
/// </remarks>
public bool RasterizeTransformedElements
{  get; set; }
 
/// <summary>
/// Adds information about font that is uploaded to the printer by manufacturer.
/// </summary>
/// <param name="fontFullName">Full name of the font (e.g. "Times New Roman Bold Italic").</param>
/// <param name="fontPclName">Name of the font that is used in Pcl document.</param>
/// <remarks>
/// There are 52 fonts that are to be built in any printer according to Pcl specification.
/// However manufactures can add some other fonts to their devices.
/// </remarks>
public void AddPrinterFont(string fontFullName, string fontPclName);
 
/// <summary>
/// Name of the font that will be used
/// if no expected font is found in printer and built-in fonts collections.
/// </summary>
/// <remarks>
/// If no fallback is found, warning is generated and "Arial" font is used.
/// </remarks>
public string FalllbackFontName
{  get; set; }
```

## Added Public Property PdfSaveOptions.DisplayDocTitle

We have added new feature in Aspose.Words for .NET 17.7 to control behavior of how document's title is presented in output PDF document. The PdfSaveOptions.DisplayDocTitle property is added in this version. This property is used to specify whether the window’s title bar should display the document title taken from the Title entry of the document information dictionary. Please refer to the following article for more detail:  
[Display the Document's Title in Window's Title bar][5]

```
/// <summary>
/// A flag specifying whether the window’s title bar should display the document title taken from
/// the Title entry of the document information dictionary.
/// </summary>
/// <remarks>
/// If <c>false</c>, the title bar should instead display the name
/// of the PDF file containing the document.
///
/// <para>The default value is <c>false</c>.</para>
/// </remarks>
public bool DisplayDocTitle
{
    get { return mDisplayDocTitle; }
    set { mDisplayDocTitle = value; }
}
```

## Improved Removal of Unused Resources From Document

Document.RemoveUnusedResources method is now obsolete. We have added new method Document.Cleanup in Aspose.Words for .NET 17.7 to remove unused styles and lists from the document. Now you can remove only lists or styles or both from document. Please refer to the following article for more detail.  
[Remove Unused Styles and Lists from Document][6]

## Changed Importing Behavior of Lists

Previously, list definitions were copied with a new identifier while importing. Now Aspose.Words reuses identical list definitions in the destination. Equality of list definitions in the source and destination is determined by their identifiers. Also Aspose.Words preserves list definition identifiers from the source when equal list definition cannot be found in the destination. This is how MS Word behaves.

## Shape.AspectRatioLocked Default Value was Changed for Shapes Inserted through the DocumentBuilder.InsertImage Method

Shape.AspectRatioLocked default value was changed for shapes inserted through the DocumentBuilder.InsertImage method. Now, to mimic MS Word behavior this value is "true" for ShapeType.Image upon inserting image through the DocumentBuilder or through the Model. Please check the code example from here:

[Lock Aspect Ratio of Image  
](https://docs.aspose.com/words/net/working-with-images/#lock-aspect-ratio-of-image)

```
/// Specifies whether the shape's aspect ratio is locked.
/// </summary>
/// <remarks>
/// The default value depends on the <see cref="ShapeType"/>, for the ShapeType.Image it is <b>true</b>
/// but for the other shape types it is <b>false</b>.
/// Has effect for top level shapes only.
/// </remarks>
public bool AspectRatioLocked
{
  get { return GraphicData.AspectRatioLocked; }
  set { GraphicData.AspectRatioLocked = value; }
} 
```

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

*   [Home of Aspose.Words for .NET API][7].
*   [Aspose.Words for .NET Download Section][8].
*   [Install Aspose.Words for .NET NuGet Package][9]
*   [Aspose.Words for .NET Documentation][10] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [Aspose.Words for .NET API Reference Guide][11] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][12]
    *   [Paid Support Forum][13]
*   [Enable Blog Subscription][14] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for .NET Examples][15] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/net/new-releases/aspose.words-for-.net-17.7/
[2]: https://docs.aspose.com/words/net/aspose-words-for-net-17-7-release-notes/
[3]: https://docs.aspose.com/words/net/aspose-words-for-net/
[4]: https://docs.aspose.com/words/net/saving-a-document/#SavingaDocument-SaveDocumenttoPCL
[5]: https://docs.aspose.com/words/net/working-with-document/#WorkingwithDocument-DisplaytheDocument'sTitleinWindow'sTitlebar
[6]: https://docs.aspose.com/words/net/working-with-document/#WorkingwithDocument-RemoveUnusedStylesandListsfromDocument
[7]: https://products.aspose.com/words/net
[8]: https://downloads.aspose.com/words/net
[9]: https://www.nuget.org/packages/Aspose.Words/
[10]: https://docs.aspose.com/words/net
[11]: https://apireference.aspose.com/net/words
[12]: https://forum.aspose.com/c/words
[13]: https://helpdesk.aspose.com/
[14]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[15]: https://github.com/aspose-words/Aspose.Words-for-.NET




