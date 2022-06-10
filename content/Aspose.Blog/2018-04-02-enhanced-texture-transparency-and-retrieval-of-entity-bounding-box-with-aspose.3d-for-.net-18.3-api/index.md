---
title: 'Enhanced Texture-Transparency and Retrieval of Entity Bounding Box using C#'
date: Mon, 02 Apr 2018 01:18:33 +0000
draft: false
url: /2018/04/02/enhanced-texture-transparency-and-retrieval-of-entity-bounding-box-with-aspose.3d-for-.net-18.3-api/
author: Imran Rafique
summary: ''
tags: ['3D Model', 'bounding box', 'entities', 'materials', 'texture-transparency']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for .NET logo">}}


We are pleased to announce the availability of [new version 18.3.0 of Aspose.3D for .NET API][1]. The new version 18.3 of the API has been released with the support of retrieving the bounding box of entities in 3D model. Developers can find improvement on applying transparency to the materials as well as the compatibility support among 3D formats with new APIs. The recent version 18.3 also covers enhancements and regular bug fixes. We recommend our clients to incorporate the latest upgrade of Aspose.3D for .NET API to take benefit of improved functionality and bug fixes.

## Apply Texture-Transparency with Per-Pixel Alpha Channel

With the help of Aspose.3D for .NET API, developers can apply a material using per-pixel alpha channel defined in the diffuse/albedo texture. In order to achieve this, we have added Alpha and AlphaSource members. These members make it compatible with texture-transparency in 3D formats like U3D/FBX and these are also supported in Aspose.3D API renderer, since LambertMaterial, PhongMaterial, and PbrMaterial classes have transparency factors.

```
// define a box node with alpha channel defined in albedo texture:
var node = new Node()
{
    Material = new PbrMaterial()
    {
        AlbedoTexture = new Texture()
        {
            AlphaSource = AlphaSource.PixelAlpha,
            Alpha = 1,
            FileName = "window.tga"
        }
     },
     Entity = new Box()
};
```

## Retrieve Bounding Box of 3D Entities using C#

With the recent version 18.3 of Aspose.3D for .NET API, developers can retrieve a bounding box of 3D entities. The GetBoundingBox method has been added to the base Entity class:

```
var box = new Box();
BoundingBox bbox = box.GetBoundingBox(); 
Console.WriteLine(bbox);
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




[1]: https://www.nuget.org/packages/Aspose.3d/18.3.0
[2]: http://www.aspose.com/products/3d/net
[3]: https://forum.aspose.com/c/3d
[4]: https://docs.aspose.com/display/3dnet/Home
[5]: https://github.com/aspose3D/Aspose_3d_NET
[6]: https://www.nuget.org/packages/Aspose.3d
[7]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+18.3+-+March+2018




