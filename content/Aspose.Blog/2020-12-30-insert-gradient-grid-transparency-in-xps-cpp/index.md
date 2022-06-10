---
title: 'Insert Gradient, Grid, or Transparent Objects in XPS File with C++'
seoTitle: "Insert Gradient, Grid, or Transparent Objects in XPS File with C++"
description: "You can insert or add gradient, grid, or transparent objects in XPS files programmatically using C++. Insert Linear, vertical, horizontal gradient."
date: Wed, 30 Dec 2020 21:48:00 +0000
draft: false
url: /2020/12/30/insert-gradient-grid-transparency-in-xps-cpp/
author: Farhan Raza
summary: 'XPS files can be used to display a lot of visual information. They support text, images, object transparency, grids, gradients, and many other features. You can **add gradients, grids, and transparent objects in XPS** files as per your requirements. In this article, we will be exploring these features in detail, along with different examples and use cases.'
tags: ['Edit XPS Document in CPP', 'Insert Gradient in XPS', 'Insert Grid in XPS', 'Insert Transparent object in XPS']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/Add-Gradient-Grid-Transparency-XPS.png" alt="Add Gradient Grid Transparency XPS">}}


XPS files can be used to display a lot of visual information. They support text, images, object transparency, grids, gradients, and many other features. You can insert gradient, grid, and transparent objects in XPS files as per your requirements. In this article, we will be exploring these features in detail, along with different examples and use cases. Let us walk through the following topics:

*   [Installing XPS API for C++][1]
*   [Adding Gradient in XPS file using C++][2]
    *   [Add Vertical Gradient in XPS file with C++][3]
    *   [Add Horizontal Gradient in XPS using C++][4]
*   [Insert Grid in XPS file with C++][5]
*   [Insert Transparent Object in XPS file using C++][6]

## Installing XPS API for C++ {#section1}

You can quickly and easily configure [Aspose.Page for C++][7] API in your programming applications for manipulating XPS, PS, EPS, and other supported file formats. Simply download the DLL file from official [Downloads][8], or install it from [NuGet][9] gallery with the command below:

```
PM> Install-Package Aspose.Page.Cpp 
```

## Adding Gradient in XPS file using C++ {#section2}

Sometimes you need to add gradient in XPS files. You can manipulate the XPS file as the API lets you add linear, horizontal as well as vertical gradient. Let us add the following gradients in a XPS file:

### Add Vertical Gradient in XPS file with C++ {#section3}

You can easily add vertical gradient in XPS files with a few simple API calls. Below are the steps for adding the vertical gradient:

1.  Create a new [XPS Document][10]
2.  Initialize List of [XpsGradientStop][11]
3.  Create a new path by defining the geometry
4.  Save resultant XPS document

The code below is based on these steps, which demonstrates how to add a vertical gradient in an XPS file using C++:

{{< gist aspose-com-gists fcfc294209efcb646f0a0de5ddfff050 "VerticalGradient.cpp" >}}

### Add Horizontal Gradient in XPS using C++ {#section4}

Another possible variation of gradient in XPS files is the horizontal gradient. The approach of adding horizontal gradient is bit related to the use case we have discussed above. The following are the steps that you need to follow for adding horizontal gradient:

1.  Create new XPS Document
2.  Specify gradient stops using [XpsGradientStop][12]
3.  Create path with geometry
4.  Save output XPS document

The following code snippet elaborates how to add horizontal gradient in XPS files using C++:

{{< gist aspose-com-gists fcfc294209efcb646f0a0de5ddfff050 "HorizontalGradient.cpp" >}}

## Insert Grid in XPS file with C++ {#section5}

Aspose.Page for C++ API lets you render grids in the XPS files with a lot of properties to control the rendering. Let us consider the example of inserting grid in XPS file in your C++ based applications. You can work with this feature by considering the steps below:

1.  Initialize XpsDocument class object
2.  Specify Geometry for the grid [VisualBrush][13]
3.  Create [Canvas][14] for magenta grid VisualBrush
4.  Create Visual brush and add grid
5.  Save output XPS file

The code below is based on these steps which explains how to insert grid in XPS files using C++:

{{< gist aspose-com-gists fcfc294209efcb646f0a0de5ddfff050 "Grid.cpp" >}}

## Insert Transparent Object in XPS file using C++ {#section6}

Another exciting feature for working with XPS files is the support for transparency and opacity. You might need to add transparent objects on the XPS file under different scenarios. This can be achieved with the help of the following steps:

1.  Create new [XPS Document][15]
2.  Create path with closed rectangle geometry
3.  Add geometry for different paths
4.  Save output XPS document

These steps are followed by the following code, that demonstrates how to add transparent object in XPS file with C++ programming language:

{{< gist aspose-com-gists fcfc294209efcb646f0a0de5ddfff050 "TransparentObject.cpp" >}}

## Conclusion

In a nutshell, we have explored a number of features to work with XPS files. You can add a gradient, linear, horizontal, or vertical, as well as grids or transparent objects in XPS files. Moreover, you can take a look at several other features by downloading the [Examples project][16]. In case of any ambiguity, please feel free to write to us at the [Free Support Forums][17]. We will be honored to guide you!

## See Also

[Insert Text or Image in XPS File Programmatically using C++][18]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: #section4
[5]: #section5
[6]: #section6
[7]: https://products.aspose.com/page/cpp
[8]: https://downloads.aspose.com/page/cpp
[9]: https://www.nuget.org/packages/Aspose.Page.Cpp/
[10]: https://apireference.aspose.com/page/cpp/class/aspose.page.x_p_s.xps_document/
[11]: https://apireference.aspose.com/page/cpp/class/aspose.page.x_p_s.xps_model.xps_gradient_stop
[12]: https://apireference.aspose.com/page/cpp/class/aspose.page.x_p_s.xps_model.xps_gradient_stop
[13]: https://apireference.aspose.com/page/cpp/class/aspose.page.x_p_s.xps_model.xps_visual_brush
[14]: https://apireference.aspose.com/page/cpp/class/aspose.page.x_p_s.xps_model.xps_canvas
[15]: https://apireference.aspose.com/page/cpp/class/aspose.page.x_p_s.xps_document/
[16]: https://github.com/aspose-page/Aspose.Page-for-C
[17]: https://forum.aspose.com/c/page
[18]: https://blog.aspose.com/2020/12/29/insert-image-text-xps-cpp/





