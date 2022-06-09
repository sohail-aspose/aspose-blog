---
title: '.NET Graphics API - Create Images and Graphics from Scratch using C#'
seoTitle: ""
description: ""
date: Sat, 27 Jun 2020 16:25:57 +0000
draft: false
url: /2020/06/27/create-images-and-graphics-using-csharp-or-vb.net/
author: Usman Aziz
summary: ''
tags: ['.NET Graphics API', 'create images from scratch using csharp', 'draw graphics on image using csharp', 'draw graphics using csharp']
categories: ['Aspose.Drawing Product Family']
---



{{< figure align=center src="images/aspose_drawing-for-net.png" alt=".NET Graphics API">}}


You would have come across various drawing applications (i.e. MS Paint) that allow you to **draw graphics** and **generate images**. However, what if you want to create your own drawing utility or integrate drawing features within your web or desktop application? For such scenarios, Aspose offers its .NET Graphics API as [Aspose.Drawing for .NET][1] which is a lightweight solution for **creating images and graphics** identical to GDI+.

Without any dependencies of the native code and libraries, [Aspose.Drawing for .NET][2] lets you draw various graphical objects such as lines, arcs, rectangles, polygons, ellipses, etc. as well as use pens and brushes to create 2D graphics using C# or VB.NET. In this article, I'll demonstrate **how to create an image from scratch** or draw graphics on an existing image using C# with our drawing API.

*   [.NET Graphics API - Installation][3]
*   [Create an Image from Scratch using C#][4]
*   [Draw Graphics on Existing Images using C#][5]

## .NET Graphics API - Installation {#NET-Graphics-API-Installation}

Before we start, lets first have a look at the installation methods of Aspose.Drawing for .NET. You can either [download][6] the API's DLL or install it using the [NuGet][7] within the Visual Studio.

```
PM> Install-Package Aspose.Drawing
```

## Create an Image from Scratch using C# {#Create-an-Image-from-Scratch-using-CSharp}

In this section, I'll show you how to use the API for creating an image from scratch. For the demonstration, I'll add only a couple of graphical objects to the image, however, the same code can be extended for adding the other objects. The following are the steps to create an image using Aspose.Drawing for .NET.

*   Create an instance of the [Bitmap][8] class.
*   Create an instance of [Graphics][9] class and initialize it with Bitmap's instance.
*   Define a new [Pen][10] object and set its properties.
*   Use [Graphics.DrawArc(Pen, Single, Single, Single, Single, Single, Single)][11] method to draw an arc.
*   Use [Graphics.DrawEllipse(Pen, Single, Single, Single, Single)][12] method to draw an ellipse.
*   Save the drawing into your desired image format using [Bitmap.Save(string)][13] method.

The following code sample shows how to create an image from scratch using C#.

{{< gist aspose-com-gists 0c035ac54f3ae3fc794e8a7e10c5a85b "create-image.cs" >}}

### Output



{{< figure align=center src="images/Create-an-image-from-scratch.jpg" alt="create an image from scratch in C#">}}


You can visit the following documentation article for the code samples of drawing other graphical objects:

*   [Draw Bezier Spline][14]
*   [Create Cardinal Spline][15]
*   [Create Closed Curve][16]
*   [Draw Lines][17]
*   and [more][18].

## Draw Graphics on Existing Images using C# {#Draw-Graphics-on-Existing-Images-using-CSharp}

You may also load an existing image and draw the desired graphical objects on it. Loading and working with an existing image is as simple as creating a new one. The following are the steps to perform this operation.

*   Create an instance of [Bitmap][19] class and initialize it with the image's path.
*   Draw desired graphics such as line, polygon, etc. in the same way you have done in the previous example.
*   Save the updated image using [Bitmap.Save(string)][20] method.

The following code sample shows how to draw graphics on an existing image using C#.

{{< gist aspose-com-gists 0c035ac54f3ae3fc794e8a7e10c5a85b "draw-graphics-on-image.cs" >}}

### Output



{{< figure align=center src="images/draw-graphics-on-image.jpg" alt="draw graphics on image C#">}}


## Conclusion

In this article, I have shown you how to use the basic features of Aspose.Drawing for .NET and create images from scratch or add graphics on existing images using C#. In order to explore all the features of the API, you can consult the [documentation][21] and download the [code samples][22].

For the upcoming posts and tutorials on Aspose.Drawing for .NET, stay tuned and keep visiting [Aspose.Drawing Product Family][23] section.




[1]: https://docs.aspose.com/display/drawingnet/Product+Overview
[2]: https://products.aspose.com/drawing/net
[3]: #NET-Graphics-API-Installation
[4]: #Create-an-Image-from-Scratch-using-CSharp
[5]: #Draw-Graphics-on-Existing-Images-using-CSharp
[6]: https://downloads.aspose.com/drawing/net
[7]: https://www.nuget.org/packages/Aspose.drawing
[8]: https://apireference.aspose.com/drawing/net/system.drawing/bitmap
[9]: https://apireference.aspose.com/drawing/net/system.drawing/graphics
[10]: https://apireference.aspose.com/drawing/net/system.drawing/pen
[11]: https://apireference.aspose.com/drawing/net/system.drawing.graphics/drawarc/methods/1
[12]: https://apireference.aspose.com/drawing/net/system.drawing.graphics/drawellipse/methods/1
[13]: https://apireference.aspose.com/drawing/net/system.drawing.image/save/methods/2
[14]: https://docs.aspose.com/display/drawingnet/Working+with+Vector+Graphics#WorkingwithVectorGraphics-DrawBezierSpline
[15]: https://docs.aspose.com/display/drawingnet/Working+with+Vector+Graphics#WorkingwithVectorGraphics-DrawCardinalSpline
[16]: https://docs.aspose.com/display/drawingnet/Working+with+Vector+Graphics#WorkingwithVectorGraphics-DrawClosedCurve
[17]: https://docs.aspose.com/display/drawingnet/Working+with+Vector+Graphics#WorkingwithVectorGraphics-DrawLines
[18]: https://docs.aspose.com/display/drawingnet/Working+with+Vector+Graphics
[19]: https://apireference.aspose.com/drawing/net/system.drawing/bitmap
[20]: https://apireference.aspose.com/drawing/net/system.drawing.image/save/methods/2
[21]: https://docs.aspose.com/display/drawingnet/Product+Overview
[22]: https://github.com/aspose-drawing/Aspose.Drawing-for-.NET
[23]: https://blog.aspose.com/category/drawing/





