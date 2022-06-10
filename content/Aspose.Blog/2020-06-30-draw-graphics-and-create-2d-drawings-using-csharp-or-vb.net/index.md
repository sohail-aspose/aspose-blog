---
title: 'Draw Graphics and Create 2D Drawings using C# or VB.NET'
seoTitle: ".NET Graphics API | C# Draw Graphics and Create 2D Drawing Shapes"
description: "Learn how to create drawings and draw various graphics in C# using .NET Graphics API. Draw line, rectangle, polygon, arc, curve, ellipse graphics using C#."
date: Tue, 30 Jun 2020 00:37:15 +0000
draft: false
url: /2020/06/30/draw-graphics-and-create-2d-drawings-using-csharp-or-vb.net/
author: Usman Aziz
summary: ''
tags: ['create 2d drawing using csharp', 'create 2d graphics using csharp', 'create drawings using csharp', 'draw graphics using csharp']
categories: ['Aspose.Drawing Product Family']
---



{{< figure align=center src="images/aspose_drawing-for-net.png" alt="Draw Graphics using C#">}}


In my previous [article][1], I have given you an overview of our .NET Graphics API - [Aspose.Drawing for .NET][2]. Along with that, we have seen how to create images from scratch or draw graphics on existing images using C#. In this article, we'll go one step ahead and learn how to create 2D drawings by drawing various graphical objects within the .NET applications such as ASP.NET web application, Windows application, and etc.

The following are the vector graphics that we are going to draw within our drawings using .NET Graphics API.

*   [Create a Drawing using C#][3]
*   [Draw an Arc in the Drawing][4]
*   [Draw a Bezier Spline in a Drawing][5]
*   [Draw a Cardinal Spline in a Drawing][6]
*   [Draw a Closed Curve in a Drawing][7]
*   [Draw an Ellipse in a Drawing][8]
*   [Draw Lines in a Drawing][9]
*   [Draw a Path in a Drawing][10]
*   [Draw a Polygon in a Drawing][11]
*   [Draw Rectangle in a Drawing][12]

Before we start, make sure you have installed Aspose.Drawing for .NET within your .NET application. You can read about the installation methods in [this post][13].

## Create a Drawing from Scratch using C# {#Create-a-Drawing-using-CSharp}

First of all, let's have a look at how to create an empty drawing and save it as a PNG image. The steps are as simple as pie.

*   Create a new [Bitmap][14] object.
*   Save the drawing in PNG format using [Bitmap.Save(string)][15] method.

You can save the drawing in [other image formats][16] as well. The following code sample shows how to create a drawing from scratch using C#.

{{< gist aspose-com-gists b8960f80422422251405395636eab772 "create-drawing.cs" >}}

## Draw an Arc in Drawing using C# {#Draw-an-Arc-within-the-Drawing}

Let's check out how to draw an arc within the drawing. The following are the steps to perform this operation.

*   Define an instance of the [Bitmap][17] class.
*   Initialize an object of [Graphics][18] class from the Bitmap object.
*   Create a [Pen][19] object to draw the arc with.
*   Use [Graphics.DrawArc(Pen, Single, Single, Single, Single, Single, Single)][20] method to draw an arc.
*   Save the drawing as an image using [Bitmap.Save(string)][21] method.

The following code sample shows how to draw an arc in the drawing using C#.

{{< gist aspose-com-gists b8960f80422422251405395636eab772 "Examples-CSharp-LinesCurvesShapes-DrawArc-DrawArc.cs" >}}



{{< figure align=center src="images/Draw-an-Arc.jpg" alt="Draw an Arc">}}


## Draw a Bezier Spline in Drawing using C# {#Draw-a-Bezier-Spline-in-a-Drawing}

The following are the steps to draw a bezier spline within a drawing.

*   Create an object of the [Bitmap][22] class.
*   Initialize an object of [Graphics][23] class from the Bitmap object.
*   Create a [Pen][24] object to draw the graphics.
*   Use [Graphics.DrawBezier(Pen, PointF, PointF, PointF, PointF)][25] method to draw Bezier Spline.
*   Save the drawing using [Bitmap.Save(string)][26] method.

The following code sample creates a Bezier Spline using C#.

{{< gist aspose-com-gists b8960f80422422251405395636eab772 "Examples-CSharp-LinesCurvesShapes-DrawBezierSpline-DrawBezierSpline.cs" >}}



{{< figure align=center src="images/Draw-Bezier-Spline.jpg" alt="Draw Bezier Spline">}}


## Add a Cardinal Spline in Drawing using C# {#Draw-a-Cardinal-Spline-in-a-Drawing}

Use the following steps to draw a cardinal spline using our .NET Graphics API.

*   Instantiate an object of the [Bitmap][27] class.
*   Create an object of [Graphics][28] class from the Bitmap object.
*   Create a [Pen][29] object for drawing.
*   Draw cardinal spline using [Graphics.DrawCurve(Pen,Point\[\])][30] method.
*   Save the drawing as an image using [Bitmap.Save(string)][31] method.

The following C# code sample draws a cardinal spline using Aspose.Drawing for .NET.

{{< gist aspose-com-gists b8960f80422422251405395636eab772 "Examples-CSharp-LinesCurvesShapes-DrawCardinalSpline-DrawCardinalSpline.cs" >}}



{{< figure align=center src="images/Draw-Cardinal-Spline.png.jpg" alt="Draw Cardinal Spline">}}


## Add a Closed Curve in Drawing using C# {#Draw-a-Closed-Curve-in-a-Drawing}

You can also draw a closed curve in the same way you have drawn the other graphical objects. The following are the steps for this.

*   Instantiate a [Bitmap][32] object.
*   Create an object of [Graphics][33] class and initialize it from the Bitmap object.
*   Create a [Pen][34] object for drawing the closed curve.
*   Draw a closed curve using [Graphics.DrawClosedCurve(Pen,Point\[\])][35] method.
*   Save the drawing using [Bitmap.Save(string)][36] method.

You can draw a closed curve using the following C# code sample.

{{< gist aspose-com-gists b8960f80422422251405395636eab772 "Examples-CSharp-LinesCurvesShapes-DrawClosedCurve-DrawClosedCurve.cs" >}}



{{< figure align=center src="images/Draw-Closed-Curve.jpg" alt="Draw Closed Curve">}}


## Draw an Ellipse in a Drawing using C# {#Draw-an-Ellipse-in-a-Drawing}

The following are the steps to draw an ellipse in a drawing using Aspose.Drawing for .NET.

*   Create an instance of the [Bitmap][37] class.
*   Define an instance of the [Graphics][38] class and initialize it from the Bitmap object.
*   Use a [Pen][39] object to draw the ellipse.
*   Draw an ellipse using [Graphics.DrawEllipse(Pen, Single, Single, Single, Single)][40] method.
*   Save the drawing as an image using [Bitmap.Save(string)][41] method.

The following code sample shows how to draw an ellipse using C#.

{{< gist aspose-com-gists b8960f80422422251405395636eab772 "Examples-CSharp-LinesCurvesShapes-DrawEllipse-DrawEllipse.cs" >}}



{{< figure align=center src="images/Draw-Ellipse.jpg" alt="Draw Ellipse">}}


## Draw Lines in a Drawing using C# {#Draw-Lines-in-a-Drawing}

Lines are one of the basic objects for creating the drawings. The following are the steps to draw the lines in a drawing using Aspose' Graphics API.

*   Instantiate the [Bitmap][42] object.
*   Create a new [Graphics][43] object and initialize it from the Bitmap object.
*   Define a [Pen][44] object to draw the line.
*   Draw a line using [Graphics.DrawLine(Pen, Int32, Int32, Int32, Int32)][45] method.
*   Save the drawing using [Bitmap.Save(string)][46] method.

The following code sample shows how to draw lines within a drawing using C#.

{{< gist aspose-com-gists b8960f80422422251405395636eab772 "Examples-CSharp-LinesCurvesShapes-DrawLines-DrawLines.cs" >}}



{{< figure align=center src="images/Draw-Lines.jpg" alt="Draw Lines">}}


## Draw a Path in the Drawing using C# {#Draw-a-Path-in-a-Drawing}

The following are the steps to draw a path within a drawing using C#.

*   Instantiate the [Bitmap][47] object.
*   Create an object of [Graphics][48] class and initialize it from the Bitmap object.
*   Define a [Pen][49] object to draw the path.
*   Create an instance of [GraphicsPath][50] class.
*   Add graphics to the path collection.
*   Draw the path using [Graphics.DrawPath(Pen, GraphicsPath)][51] method.
*   Save the drawing using [Bitmap.Save(string)][52] method.

The following code sample shows how to draw a path within a drawing using C#.

{{< gist aspose-com-gists b8960f80422422251405395636eab772 "Examples-CSharp-LinesCurvesShapes-DrawPath-DrawPath.cs" >}}



{{< figure align=center src="images/Draw-Path.jpg" alt="Draw Path">}}


## Draw a Polygon in a Drawing using C# {#Draw-a-Polygon-in-a-Drawing}

The following are the steps to draw a polygon within a drawing using Aspose.Drawing for .NET.

*   Instantiate the [Bitmap][53] object.
*   Define a [Graphics][54] object and initialize it from the Bitmap object.
*   Define a [Pen][55] object to draw the polygon.
*   Draw a polygon using [Graphics.DrawPolygon(Pen,Point\[\])][56] method.
*   Save the drawing using [Bitmap.Save(string)][57] method.

This is how you can draw a polygon within a drawing using C#.

{{< gist aspose-com-gists b8960f80422422251405395636eab772 "Examples-CSharp-LinesCurvesShapes-DrawPolygon-DrawPolygon.cs" >}}



{{< figure align=center src="images/Draw-Polygon.jpg" alt="Draw Polygon">}}


## Draw a Rectangle within the Drawing using C# {#Draw-Rectangle-in-a-Drawing}

Last but not the least, drawing a rectangle. The following are the steps to draw a rectangle.

*   Create a [Bitmap][58] object.
*   Create a [Graphics][59] object and initialize it from the Bitmap object.
*   Define a [Pen][60] object to draw the rectangle.
*   Draw a rectangle using [Graphics.DrawRectangle(Pen, Int32, Int32, Int32, Int32)][61] method.
*   Save the drawing using [Bitmap.Save(string)][62] method.

The following C# code sample draws a rectangle within a drawing.

{{< gist aspose-com-gists b8960f80422422251405395636eab772 "Examples-CSharp-LinesCurvesShapes-DrawRectangle-DrawRectangle.cs" >}}



{{< figure align=center src="images/Draw-Rectangle.jpg" alt="Draw Rectangle">}}


## Conclusion

In this article, we have seen how various graphical objects can be drawn within a drawing programmatically using C#. The step by step guide and code samples demonstrated how to draw lines, rectangles, polygons, arcs, bezier spline, cardinal spline, curves and ellipses within the drawings. You can learn more about our .NET Graphics API using the [documentation][63].

## See Also

*   [Create Images and Graphics from Scratch using C#][64]




[1]: https://blog.aspose.com/2020/06/27/create-images-and-graphics-using-csharp-or-vb.net/
[2]: https://products.aspose.com/drawing/net
[3]: #Create-a-Drawing-using-CSharp
[4]: #Draw-an-Arc-within-the-Drawing
[5]: #Draw-a-Bezier-Spline-in-a-Drawing
[6]: #Draw-a-Cardinal-Spline-in-a-Drawing
[7]: #Draw-a-Closed-Curve-in-a-Drawing
[8]: #Draw-an-Ellipse-in-a-Drawing
[9]: #Draw-Lines-in-a-Drawing
[10]: #Draw-a-Path-in-a-Drawing
[11]: #Draw-a-Polygon-in-a-Drawing
[12]: #Draw-Rectangle-in-a-Drawing
[13]: https://blog.aspose.com/2020/06/27/create-images-and-graphics-using-csharp-or-vb.net/#.NET-Graphics-API-Installation
[14]: https://apireference.aspose.com/drawing/net/system.drawing/bitmap
[15]: https://apireference.aspose.com/drawing/net/system.drawing.image/save/methods/2
[16]: https://docs.aspose.com/display/drawingnet/Supported+File+Formats
[17]: https://apireference.aspose.com/drawing/net/system.drawing/bitmap
[18]: https://apireference.aspose.com/drawing/net/system.drawing/graphics
[19]: https://apireference.aspose.com/drawing/net/system.drawing/pen
[20]: https://apireference.aspose.com/drawing/net/system.drawing.graphics/drawarc/methods/1
[21]: https://apireference.aspose.com/drawing/net/system.drawing.image/save/methods/2
[22]: https://apireference.aspose.com/drawing/net/system.drawing/bitmap
[23]: https://apireference.aspose.com/drawing/net/system.drawing/graphics
[24]: https://apireference.aspose.com/drawing/net/system.drawing/pen
[25]: https://apireference.aspose.com/drawing/net/system.drawing/graphics/methods/drawbezier
[26]: https://apireference.aspose.com/drawing/net/system.drawing.image/save/methods/2
[27]: https://apireference.aspose.com/drawing/net/system.drawing/bitmap
[28]: https://apireference.aspose.com/drawing/net/system.drawing/graphics
[29]: https://apireference.aspose.com/drawing/net/system.drawing/pen
[30]: https://apireference.aspose.com/drawing/net/system.drawing/graphics/methods/drawcurve
[31]: https://apireference.aspose.com/drawing/net/system.drawing.image/save/methods/2
[32]: https://apireference.aspose.com/drawing/net/system.drawing/bitmap
[33]: https://apireference.aspose.com/drawing/net/system.drawing/graphics
[34]: https://apireference.aspose.com/drawing/net/system.drawing/pen
[35]: https://apireference.aspose.com/drawing/net/system.drawing/graphics/methods/drawclosedcurve
[36]: https://apireference.aspose.com/drawing/net/system.drawing.image/save/methods/2
[37]: https://apireference.aspose.com/drawing/net/system.drawing/bitmap
[38]: https://apireference.aspose.com/drawing/net/system.drawing/graphics
[39]: https://apireference.aspose.com/drawing/net/system.drawing/pen
[40]: https://apireference.aspose.com/drawing/net/system.drawing.graphics/drawellipse/methods/1
[41]: https://apireference.aspose.com/drawing/net/system.drawing.image/save/methods/2
[42]: https://apireference.aspose.com/drawing/net/system.drawing/bitmap
[43]: https://apireference.aspose.com/drawing/net/system.drawing/graphics
[44]: https://apireference.aspose.com/drawing/net/system.drawing/pen
[45]: https://apireference.aspose.com/drawing/net/system.drawing.graphics/drawline/methods/2
[46]: https://apireference.aspose.com/drawing/net/system.drawing.image/save/methods/2
[47]: https://apireference.aspose.com/drawing/net/system.drawing/bitmap
[48]: https://apireference.aspose.com/drawing/net/system.drawing/graphics
[49]: https://apireference.aspose.com/drawing/net/system.drawing/pen
[50]: https://apireference.aspose.com/drawing/net/system.drawing.drawing2d/graphicspath
[51]: https://apireference.aspose.com/drawing/net/system.drawing/graphics/methods/drawpath
[52]: https://apireference.aspose.com/drawing/net/system.drawing.image/save/methods/2
[53]: https://apireference.aspose.com/drawing/net/system.drawing/bitmap
[54]: https://apireference.aspose.com/drawing/net/system.drawing/graphics
[55]: https://apireference.aspose.com/drawing/net/system.drawing/pen
[56]: https://apireference.aspose.com/drawing/net/system.drawing/graphics/methods/drawpolygon
[57]: https://apireference.aspose.com/drawing/net/system.drawing.image/save/methods/2
[58]: https://apireference.aspose.com/drawing/net/system.drawing/bitmap
[59]: https://apireference.aspose.com/drawing/net/system.drawing/graphics
[60]: https://apireference.aspose.com/drawing/net/system.drawing/pen
[61]: https://apireference.aspose.com/drawing/net/system.drawing.graphics/drawrectangle/methods/1
[62]: https://apireference.aspose.com/drawing/net/system.drawing.image/save/methods/2
[63]: https://docs.aspose.com/display/drawingnet/Product+Overview
[64]: https://blog.aspose.com/2020/06/27/create-images-and-graphics-using-csharp-or-vb.net/





