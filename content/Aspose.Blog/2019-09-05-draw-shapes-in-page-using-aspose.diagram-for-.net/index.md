---
title: 'Draw Shapes in Visio Page using C# with Aspose.Diagram for .NET'
date: Thu, 05 Sep 2019 16:22:53 +0000
draft: false
url: /2019/09/05/draw-shapes-in-page-using-aspose.diagram-for-.net/
author: Aliahmad
summary: ''
tags: ['.NET API', 'Aspose.Diagram', 'Drawing Shapes', 'Visio', 'Visio Shapes']
categories: ['Aspose.Diagram Product Family']
---

Microsoft office is one of the most powerful drawing tools in the market. If you want to work with it programmatically and develop Add-Ons, it becomes a hassle. Often times it becomes even hard to perform a basic task - like drawing a shape inside a page. Well, you don't need to worry much! It's as easy as pie when you draw shapes using **[Aspose.Diagram for .NET][1]**.

Using Aspose.Diagram for .NET, you can not only draw basic but complex shapes like **Bezier**, **Spline, Polyline,** and using just a couple of lines of code.

Let's draw some shapes in a page using Aspose.Diagram for .NET

## Draw Bezier

Drawing Bezier is pretty simple, you can draw it using the **DrawBezier** method.

```
`// Load diagram
Diagram diagram = new Diagram();
// Initiazlie a new PointF
PointF[] ps = new PointF[] { new PointF(1, 1), new PointF(2, 2), 
                             new PointF(3.79949292203676f, 0) };
// Draw brezier in diagram
diagram.Pages[0].DrawBezier(1, 1, 2, 2, ps);
// Save diagram
diagram.Save("DrawBezierInPage.vsdx", SaveFileFormat.VSDX);` 

```

The following is the resultant bezier shape.



{{< figure align=center src="images/Screenshot_12.png" alt="">}}


## Draw Polyline

Similarly, drawing polyline is even simpler, you can draw it using the **DrawPolyline** method.

```
`// Load diagram
Diagram diagram = new Diagram();
// Initiazlie a new PointF[]
PointF[] ps = new PointF[] { new PointF(1, 1), 
                             new PointF(2, 2), 
                             new PointF(3.79949292203676f, 0) };
// Draw polyline in page
diagram.Pages[0].DrawPolyline(1, 1, 2, 2, ps);
// Save diagram
diagram.Save(dataDir + "DrawPolylineInPage_out.vsdx", SaveFileFormat.VSDX);` 

```

The following is the resultant polyline shape.



{{< figure align=center src="images/Screenshot_13.png" alt="">}}


## Draw Spline

As explained earlier drawing shapes using Aspose.Diagram for .NET is a piece of cake, you can draw spline in a page using the **DrawSpline** method.

```
`// Load diagram
Diagram diagram = new Diagram();
// Initiazlie a new PointF[]
PointF[] ps = new PointF[] { new PointF(1, 1.3270758925347308f),
                 new PointF(2.2926845121364643f, 4.3581517392187368f),
                 new PointF(4.6526026522346893f, 5.4640748257705201f),
                 new PointF(6f, 7.327075892534732f) };
// Draw Spline in diagram
diagram.Pages[0].DrawSpline(1, 1, 2, 2, ps);
// Save diagram
diagram.Save(dataDir + "DrawSplineInPage.vsdx", SaveFileFormat.VSDX);` 

```

The following is the resultant spline shape.



{{< figure align=center src="images/Screenshot_11.png" alt="">}}


For more details, please feel free to visit documentation[.][2] To explore more examples you can access our open source [examples][3] and in case you would have any query, please feel to contact us using our [forum][4].




[1]: https://products.aspose.com/diagram
[2]: https://docs.aspose.com/display/pageproductfamily/Home
[3]: https://github.com/aspose-diagram/Aspose.Diagram-for-.NET
[4]: https://forum.aspose.com/c/diagram




