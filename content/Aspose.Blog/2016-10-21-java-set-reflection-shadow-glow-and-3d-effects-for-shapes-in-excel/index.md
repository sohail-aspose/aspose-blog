---
title: 'Set Reflection, Shadow, Glow and 3D Effects for Shapes in Excel using Java'
date: Fri, 21 Oct 2016 09:36:41 +0000
draft: false
url: /2016/10/21/java-set-reflection-shadow-glow-and-3d-effects-for-shapes-in-excel/
author: Babar Raza
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 16.10.0][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the API. Please check the detailed [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the [Public API Changes][3] section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Reflection Effects in Excel Shapes

Aspose.Cells for Java 16.10.0 has added the support for reflection effects for a Shape object as Excel provides it via Effects tab under Format Shape dialog as shown below.



{{< figure align=center src="images/reflection-effect-of-shape1.png" alt="">}}


In order to provide the said feature, Aspose.Cells for Java 16.10.0 has exposed the ReflectionEffect class along with Shape.Reflection property which together controls the reflection effects of a Shape object.

Here is a simple usage scenario of newly exposed APIs to apply reflection on an existing shape, whereas a detailed article can be viewed on [Working with Reflection Effects for Shapes][4].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-WorkingWithReflectionEffect-WorkingWithReflectionEffect.java" >}}

## Support for Shadow Effects

Aspose.Cells for Java 16.10.0 has added the support for Shadow Effects for a Shape object as Excel provides it via Effects tab under Format Shape dialog as shown below.



{{< figure align=center src="images/shadow-effect-of-shape.png" alt="">}}


Aspose.Cells for Java 16.10.0 has exposed the Shape.ShadowEffect property along with ShadowEffect class which together allows to set the shadow effect on a Shape object.

Here is a simple usage scenario of newly exposed APIs to apply shadow on an existing shape, whereas a detailed article can be viewed on [Working with Shadow Effects for Shapes][5].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-WorkingWithShadowEffect-WorkingWithShadowEffect.java" >}}

## Support for Glow Effects

Aspose.Cells for Java now supports the Glow Effects for a Shape object as Excel provides it via Effects tab under Format Shape dialog as shown below.



{{< figure align=center src="images/glow-effect-of-shape.png" alt="">}}


Aspose.Cells for Java 16.10.0 has exposed the Shape.Glow property along with GlowEffect class which together allows to set the glow effect on a Shape object.

Here is a simple usage scenario of newly exposed APIs to apply glow effect on an existing shape, whereas a detailed article can be viewed on [Working with Glow Effects for Shapes][6].

{{< gist aspose-cells 87c05ec07dd1a65ac6fcdf2fa896b01e "Examples-src-main-java-com-aspose-cells-examples-articles-WorkingWithGlowEffect-WorkingWithGlowEffect.java" >}}

## Support for 3-D Formats

Aspose.Cells for Java supports the 3-D Formats for Shape objects as Excel provides it via Effects tab under Format Shape dialog as shown below.



{{< figure align=center src="images/ThreeDformat-of-shape.png" alt="">}}


Aspose.Cells for Java 16.10.0 has exposed the Shape.ThreeDFormat property along with ThreeDFormat class which together allows to set the 3D formatting for a Shape object.

Here is a simple usage scenario of newly exposed APIs to apply 3D formatting on an existing shape, whereas a detailed article can be viewed on [Working with 3-D Formats for Shapes][7].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-WorkingWithThreeDFormat-WorkingWithThreeDFormat.java" >}}

## Support for WordArt Built-in Styles

Aspose.Cells for Java APIs now support to add WordArt objects with built-in styles. In order to provide this feature, the Aspose.Cells for Java APIs have exposed the ShapeCollection.AddWordArt method along with PresetWordArtStyle enumeration which together allows to add preset WordArt objects since Excel 2007.

Here is a simple usage scenario of newly exposed APIs to add WordArt with build-in styles, whereas a detailed article can be viewed on [Working with Built-in Styles for WordArt][8].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-AddWordArtText-AddWordArtText.java" >}}

## Automatic Propagation of Formula in ListObject

Microsoft Excel application allows the automatic proprgation of formulas when new rows are inserted to a ListObject/Table. Aspose.Cells now provides the same feature by exposing the ListColumn.Formula property with this release

Here is a simple usage scenario of ListColumn.Formula property, whereas a detailed article can be viewed on [Automatically Propagate Formula in ListObject][9].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-PropagateFormulaInTableorListObject-PropagateFormulaInTableorListObject.java" >}}

## Other Enhancements & Fixes

Aspose.Cells for Java 16.10.0 has fixed a few critical bugs as well as enhanced its core for more stability. A few of the worth mentioning enhancements are as follow.

*   Ability to [detect if spreadsheet contains hidden external links][10].
*   Ability to [add XML map to spreadsheet][11] and [link cell to XML map elements][12].
*   Ability to [set preset WordArt styles to shape's text][13].
*   Handled a few exceptions such as NullPointerException, IndexOutOfBoundsException & ClassCastException for certain scenarios.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][14].
*   [Aspose.Cells for Java Download Section][15].
*   [Aspose.Cells for Java Documentation][16] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][17] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][18] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][19] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][20] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://www.aspose.com/downloads/cells/java/new-releases/-aspose.cells-for-java-16.10.0/
[2]: http://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+16.10.0+Release+Notes
[3]: http://docs.aspose.com/display/cellsjava/Migrating+from+Earlier+Versions+of+Aspose.Cells
[4]: http://docs.aspose.com/display/cellsjava/Working+with+the+Reflection+Effect+of+Shape+or+Chart
[5]: http://docs.aspose.com/display/cellsjava/Working+with+the+Shadow+Effect+of+Shape+or+Chart
[6]: http://docs.aspose.com/display/cellsjava/Working+with+the+Glow+Effect+of+Shape+or+Chart
[7]: http://docs.aspose.com/display/cellsjava/Working+with+the+ThreeDFormat+of+Shape+or+Chart
[8]: http://docs.aspose.com/display/cellsjava/Add+Word+Art+Text+with+Built-in+Styles
[9]: http://docs.aspose.com/display/cellsjava/Propagate+Formula+in+Table+or+List+Object+automatically+while+entering+data+in+new+rows
[10]: http://docs.aspose.com/display/cellsjava/Check+if+Workbook+contains+hidden+External+Links
[11]: http://docs.aspose.com/display/cellsjava/Add+XML+Map+inside+the+Workbook+using+XmlMapCollection.Add+method
[12]: http://docs.aspose.com/display/cellsjava/Link+Cells+to+Xml+Map+Elements
[13]: http://docs.aspose.com/display/cellsjava/Set+preset+WordArt+style+to+the+text+of+the+shape
[14]: http://www.aspose.com/java/excel-component.aspx
[15]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/default.aspx
[16]: http://docs.aspose.com/display/cellsjava/home
[17]: http://www.aspose.com/api/java/cells/com.aspose.cells/index
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[20]: https://github.com/asposecells/Aspose_Cells_Java




