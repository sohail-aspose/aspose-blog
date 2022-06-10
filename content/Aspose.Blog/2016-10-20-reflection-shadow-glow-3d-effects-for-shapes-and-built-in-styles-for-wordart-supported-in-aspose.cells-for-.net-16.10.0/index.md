---
title: 'Reflection, Shadow, Glow &amp; 3D Effects for Shapes and Built-in Styles for WordArt Supported in Aspose.Cells for .NET 16.10.0'
date: Thu, 20 Oct 2016 19:11:48 +0000
draft: false
url: /2016/10/20/reflection-shadow-glow-3d-effects-for-shapes-and-built-in-styles-for-wordart-supported-in-aspose.cells-for-.net-16.10.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce our next version of [Aspose.Cells for .NET v16.10.0][1]. This release includes many new features and other enhancements with some critical bug fixes. Please see the [release notes][2] in order to know what is new and what has been changed/fixed with this version of Aspose.Cells for .NET. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete [Public API Changes][3] section to know what APIs are changed so far. We have highlighted some important features and other enhancements here.

## Support for Reflection Effects

Aspose.Cells for .NET 16.10.0 has added the support for reflection effects for a Shape object as Excel provides it via Effects tab under Format Shape dialog as shown below.



{{< figure align=center src="images/reflection-effect-of-shape1.png" alt="">}}


In order to provide the said feature, Aspose.Cells for .NET 16.10.0 has exposed the ReflectionEffect class along with Shape.Reflection property which together controls the reflection effects of a Shape object.

Here is a simple usage scenario of newly exposed APIs to apply reflection on an existing shape, whereas a detailed article can be viewed on [Working with Reflection Effects for Shapes][4].

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ReflectionEffectOfShape-ReflactionEffectOfShape.cs" >}}

## Support for Shadow Effects

Aspose.Cells for .NET 16.10.0 has added the support for Shadow Effects for a Shape object as Excel provides it via Effects tab under Format Shape dialog as shown below.



{{< figure align=center src="images/shadow-effect-of-shape.png" alt="">}}


Aspose.Cells for .NET 16.10.0 has exposed the Shape.ShadowEffect property along with ShadowEffect class which together allows setting the shadow effect on a Shape object.

Here is a simple usage scenario of newly exposed APIs to apply shadow on an existing shape, whereas a detailed article can be viewed on [Working with Shadow Effects for Shapes][5].

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ShadowEffectOfShape-ShadowEffectOfShape.cs" >}}

## Support for Glow Effects

Aspose.Cells for .NET now supports the Glow Effects for a Shape object as Excel provides it via Effects tab under Format Shape dialog as shown below.



{{< figure align=center src="images/glow-effect-of-shape.png" alt="">}}


Aspose.Cells for .NET 16.10.0 has exposed the Shape.Glow property along with GlowEffect class which together allows setting the glow effect on a Shape object.

Here is a simple usage scenario of newly exposed APIs to apply glow effect on an existing shape, whereas a detailed article can be viewed on [Working with Glow Effects for Shapes][6].

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-GlowEffectOfShape-GlowEffectOfShape.cs" >}}

## Support for 3-D Formats

Aspose.Cells for .NET supports the 3D Formats for Shape objects as MS Excel provides it via Effects tab under Format Shape dialog as shown below.



{{< figure align=center src="images/ThreeDformat-of-shape.png" alt="">}}


Aspose.Cells for .NET 16.10.0 has exposed the Shape.ThreeDFormat property along with ThreeDFormat class which together allows to set the 3D formatting for a Shape object.

Here is a simple usage scenario of newly exposed APIs to apply 3D formatting on an existing shape, whereas a detailed article can be viewed on [Working with 3-D Formats for Shapes][7].

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-Shape3DEffect-Shape3DEffect.cs" >}}

## Support for WordArt Built-in Styles

Aspose.Cells for .NET APIs now support to add WordArt objects with built-in styles. In order to provide this feature, the Aspose.Cells for .NET APIs have exposed the ShapeCollection.AddWordArt method along with PresetWordArtStyle enumeration which together allows adding preset WordArt objects since MS Excel 2007.

Here is a simple usage scenario of newly exposed APIs to add WordArt with build-in styles, whereas a detailed article can be viewed on [Working with Built-in Styles for WordArt][8].

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-AddWordArtTextWithBuiltinStyle-1.cs" >}}

## Automatic Propagation of Formula in ListObject

Microsoft Excel application allows the automatic propagation of formulas when new rows are inserted into a ListObject/Table. Aspose.Cells now provides the same feature by exposing the ListColumn.Formula property with this release

Here is a simple usage scenario of ListColumn.Formula property, whereas a detailed article can be viewed on [Automatically Propagate Formula in ListObject][9].

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-PropagateFormulaInTable-1.cs" >}}

## Other Enhancements and Fixes

Aspose.Cells for .NET 16.10.0 has fixed a few critical bugs as well as enhanced its core for more stability. A few of the worth mentioning enhancements are as follows.

*   Ability to [detect if spreadsheet contains hidden external links][10].
*   Ability to [add XML map to spreadsheet][11] and [link cell to XML map elements][12].
*   Ability to [set preset WordArt styles to shape's text][13].
*   Ability to [read values of the GridWeb cells on client side][14].
*   Ability to [calculate custom functions in GridWeb][15].
*   Aspose.Cells for .NET formula calculation engine is enhanced.
*   Handled a few exceptions, such as, NullPointerException, IndexOutOfRangeException, System.ArgumentOutOfRangeException and System.FormatException for certain scenarios.

In this release, several important issues have been addressed. For example, issues around reading and rendering to Excel and HTML file formats, adding List Objects/ Tables, conditional formatting, manipulating shapes, manipulating internal and external links, manipulating PivotTables, [rendering images from Excel worksheets][16], [rendering images files from charts][17] and [exporting Excel workbooks to PDF format][18] have been resolved.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][19].
*   [Aspose.Cells for .NET Download Section][20].
*   [Aspose.Cells for .NET Documentation][21] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][22] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][23] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][24] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/net
[2]: http://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+16.10.0+Release+Notes
[3]: http://docs.aspose.com/display/cellsnet/Migrating+from+Earlier+Versions+of+Aspose.Cells
[4]: http://docs.aspose.com/display/cellsnet/Working+with+the+Reflection+Effect+of+Shape+or+Chart
[5]: http://docs.aspose.com/display/cellsnet/Working+with+the+Shadow+Effect+of+Shape+or+Chart
[6]: http://docs.aspose.com/display/cellsnet/Working+with+the+Glow+Effect+of+Shape+or+Chart
[7]: http://docs.aspose.com/display/cellsnet/Working+with+the+ThreeDFormat+of+Shape+or+Chart
[8]: http://docs.aspose.com/display/cellsnet/Add+Word+Art+Text+with+Built-in+Styles
[9]: http://docs.aspose.com/display/cellsnet/Propagate+Formula+in+Table+or+List+Object+automatically+while+entering+data+in+new+rows
[10]: http://docs.aspose.com/display/cellsnet/Check+if+Workbook+contains+hidden+External+Links
[11]: http://docs.aspose.com/display/cellsnet/Add+XML+Map+inside+the+Workbook+using+XmlMapCollection.Add+method
[12]: http://docs.aspose.com/display/cellsnet/Link+Cells+to+Xml+Map+Elements
[13]: http://docs.aspose.com/display/cellsnet/Set+preset+WordArt+style+to+the+text+of+the+shape
[14]: http://docs.aspose.com/display/cellsnet/Read+the+values+of+the+GridWeb+cells+on+Client+Side
[15]: http://docs.aspose.com/display/cellsnet/Calculate+Custom+Functions+in+GridWeb
[16]: http://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Image
[17]: https://docs.aspose.com/display/cellsnet/Home
[18]: http://docs.aspose.com/display/cellsnet/Converting+Excel+to+PDF+Files
[19]: https://products.aspose.com/cells/net
[20]: http://www.aspose.com/downloads/cells/net
[21]: http://docs.aspose.com/display/cellsnet/home
[22]: https://apireference.aspose.com/net/cells
[23]: http://forum.aspose.com
[24]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




