---
title: 'Enhanced PowerPoint Shapes Capabilities using Aspose.Slides for .NET, Java and C++'
date: Fri, 20 Sep 2019 14:11:26 +0000
draft: false
url: /2019/09/20/enhanced-powerpoint-shapes-capabilities-using-aspose-slides/
author: Adnan Ahmad
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png) Here comes new release of Aspose.Slides 19.8 for .NET, Java and C++, which contains a lot of new features. In this blog, we will explore different enhanced features improving PowerPoint shapes capabilities. The shapes in a presentation could be distinguished by the Alternative Text or Shape Name property. The Alternative Text property can be read or set by using Aspose.Slides as well as Microsoft PowerPoint. By using this property, one can tag a shape and can perform different operations; such as removing a shape, hiding a shape or reordering shapes on a slide.

In following sections, I will give you walk through of new features included in API.

## Hiding Shapes

In this new release, we have provided feature to hide any shape. First, one need to identify the desired shape using Alternative Text property. Then using following example code hiding of shapes is achieved in API.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Shapes-Hidingshapes-Hidingshapes.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Slides-Shapes-HidingTheShapesFromSlide-HidingTheShapesFromSlide.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-Hidingshapes-Hidingshapes.cpp" >}}

## Get Effective Properties of Camera

Aspose.Slides provide feature to get effective properties of the camera. For this purpose, the** Camera Effective Data **class has been added in Aspose.Slides. Camera Effective Data class represents an immutable object which contains effective camera properties. The purpose of this property is to get camera properties from presentation file.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Shapes-GetCameraEffectiveData-GetCameraEffectiveData.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Slides-Shapes-GetCameraEffectiveData-GetCameraEffectiveData.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-GetCameraEffectiveData-GetCameraEffectiveData.cpp" >}}

## Get Effective Font Height Value {#mce_24}

In this new release, the support for getting effective font height value has also been made available. The following example demonstrates the portion's effective font height value changing after setting local font height values on different presentation structure levels. 

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Text-SetLocalFontHeightValues-SetLocalFontHeightValues.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Text-SetLocalFontHeightValues-SetLocalFontHeightValues.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-SetLocalFontHeightValues-SetLocalFontHeightValues.cpp" >}}

## Setting Layout Mode of Chart Plot Area

Setting layout mode for chart plot area is one of frequently used feature and has now been introduced in API as well. For this purpose, a property **LayoutTargetType** has been added to **ChartPlotArea** class  and **IChartPlotArea** interface. If the layout of the plot area is defined manually then this property specifies whether to layout the plot area by its inside (not including axis and axis labels) or outside (including axis and axis labels). There are two possible values which are defined in **LayoutTargetType **enum.

The following examples demonstrate how to Set Layout Mode of chart using API.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Charts-SetLayoutMode-SetLayoutMode.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Slides-Charts-SetLayoutMode-SetLayoutMode.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-SetLayoutMode-SetLayoutMode.cpp" >}}

## Get Effective Fill Format for Table

Aspose.Slides provides feature to get effective fill formatting for different table logic parts. For this purpose, the** IFillFormatEffectiveData** interface has been added in Aspose.Slides, which contains effective fill formatting properties. One thing to note is that cell formatting always has higher priority than row formatting, a row has higher priority than column and column higher that whole table. The **CellFormatEffectiveData** properties are always used to draw the table.

The following code sample shows how to get effective fill formatting for different table logic parts.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Tables-GetEffectiveValuesOfTable-GetEffectiveValuesOfTable.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Slides-Table-GetEffectiveValuesOfTable-GetEffectiveValuesOfTable.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-GetEffectiveValuesOfTable-GetEffectiveValuesOfTable.cpp" >}}

## Set File Type for an Embedding Object

Now, API also provides feature to set file type of an embedded object. These feature allow to get OLE object as a parameter. So now OLE object contains its type and PowerPoint can open created OLE objects.

The following example shows how to set file type for an embedding object:

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Tables-GetEffectiveValuesOfTable-GetEffectiveValuesOfTable.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Slides-Shapes-SetFileTypeForAnEmbeddingObject-SetFileTypeForAnEmbeddingObject.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-SetFileTypeForAnEmbeddingObject-SetFileTypeForAnEmbeddingObject.cpp" >}}

Wait, there's many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][2]

When time allows you can check out API [examples at Github][3], talk about this release and other API related issues in our [forum][4].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png "Aspose.Slides or .NET logo"
[2]: https://docs.aspose.com/display/slidesnet/Aspose.Slides+for+.NET+19.8+Release+Notes
[3]: https://github.com/aspose-slides/
[4]: https://forum.aspose.com/c/slides




