---
title: 'Apply 3D Mesh Morphing and Evaluate Nurbs Curve in C# .NET'
date: Mon, 05 Mar 2018 17:17:17 +0000
draft: false
url: /2018/03/05/apply-3d-mesh-morphing-and-evaluate-nurbs-curve-with-aspose.3d-for-.net-18.2-api/
author: Imran Rafique
summary: ''
tags: ['3D Mesh', '3D Model', 'Morphing Channel', 'Nurbs curve', 'neighbor knots']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for .NET logo">}}


We are pleased to announce the availability of [new version 18.2.0 of Aspose.3D for .NET API][1]. The new version 18.2 of the API has been released with the support of adding targets to Morph channel in 3D models. Developers can evaluate frequency between two neighbor knots of the Nurbs curve. The recent version 18.2 also covers enhancements and regular bug fixes. We recommend our clients to incorporate the latest upgrade of Aspose.3D for .NET API to take benefit of improved functionality and bug fixes.

## Add Targets to Morph Channel in 3D Mesh

With the help of Aspose.3D for .NET API, developers can modify a Mesh from one shape to another by adding targets to the Morph Channel. Please refer to the following C# code example:

```
// initialize a 3D scene
Scene scene = new Scene();
// initialize Deformer
MorphTargetDeformer blendShape = new MorphTargetDeformer("BlendShape"); 
// initialize Chanel
MorphTargetChannel channel = new MorphTargetChannel("BlendShapeChannel"); 
// add Chanel
blendShape.Channels.Add(channel); 
// initialize shape
Shape shape = new Shape("Shape"); 
// set weight range between 0-1 
channel[shape] = 0.99; 
// initialize Mesh
Mesh mesh = new Mesh("mesh"); 
mesh.Deformers.Add(blendShape);
```

## Evaluate Nurbs Curve in C#

With the recent version 18.2 of Aspose.3D for .NET API, developers can evaluate the frequency between two neighbor knots and the default value is 20. Developers can retrieve an array of Points in the curve. In order to achieve this, we have added Evaluate and EvaluateAt members to NurbsCurve class. Please refer to the following C# code example:

```
NurbsCurve curve = new NurbsCurve();
    curve.ControlPoints.AddRange(new Vector4[]{
        new Vector4(-28.0118217468262, 53.0359077453613, 0, 1),
        new Vector4(8.95330429077148, 64.7735290527344, 0, 1),
        new Vector4(35.7778739929199, 42.424259185791, 0, 1),
        new Vector4(24.8725852966309, -4.86993026733398, 0, 1),
        new Vector4(-35.7778739929199, -34.192684173584, 0, 1),
        new Vector4(-18.6066780090332, -57.1458396911621, 0, 1),
        new Vector4(17.733715057373, -64.7735290527344, 0, 1)
    });
    curve.KnotVectors.AddRange(new double[]{0, 0, 0, 0, 0.25, 0.5, 0.75, 1, 1, 1, 1});
    foreach (var pt in curve.Evaluate())
    {
        Console.WriteLine(pt);
    }
```

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][2]
*   [Aspose.3D product family forum][3] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][4] – help documentation and API reference documents.
*   Enable Blog Subscription – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][5] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [Install Aspose.3D NuGet package][6] - We publish each version of Aspose.3D for .NET API as a NuGet package on the NuGet gallery and recommend our clients upgrade old version to the latest one.
*   [Release Notes][7] - For details on API fixes, please check Release Notes having a complete list of the new features.

We hope you will enjoy this new release that save time and huge efforts for related files manipulation. The API is quite simple and can easily be used in any application.




[1]: https://www.nuget.org/packages/Aspose.3d/18.2.0
[2]: http://www.aspose.com/products/3d/net
[3]: https://forum.aspose.com/c/3d
[4]: https://docs.aspose.com/display/3dnet/Home
[5]: https://github.com/aspose3D/Aspose_3d_NET
[6]: https://www.nuget.org/packages/Aspose.3d
[7]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+18.2+-+February+2018




