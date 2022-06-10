---
title: 'Import ASE 3D Model and Create Rectangular Torus into the Scene using C#'
date: Wed, 17 Jan 2018 16:42:03 +0000
draft: false
url: /2018/01/17/import-ase-model-and-create-rectangular-torus-into-the-scene-with-aspose.3d-for-.net-18.1/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for .NET logo">}}


We are pleased to announce the availability of [new version 18.1.0 of Aspose.3D for .NET API][1]. The new version 18.1 of the API has been released with the support of importing 3D ASE models. Developers can create rectangular torus object in 3D scene as well as set the load option of RVM model to center the scene by moving the root node.

## Import ASE Models into Aspose.3D

With the help of Aspose.3D for .NET API, developers can import ASE 3D models, and then save to supported 3D formats. The multiple constructors and Open method of Diagram class allow importing 3D models. Please refer to this help topic: [Reading a 3D Scene][2]

## Create Rectangular Torus Object in 3D Scene

With the recent version 18.1 of Aspose.3D for .NET API, developers can create rectangular Torus object in 3D scene. In order to achieve this, we have added RectangularTorus class. Please refer to the code example as documented in this help topic: [Create rectangular Torus in 3D Scene][3]

Furthermore, the CenterScene member has been added to the A3DObject class. It helps to center the scene by moving the root node. This is the code example:

```
// initialize a 3D sceneScene scene = new Scene();scene.Open(@"c:\temp\test.rvm", new RvmLoadOptions() {CenterScene = true}); 
```

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][4]
*   [Aspose.3D product family forum][5] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][6] – help documentation and API reference documents.
*   Enable Blog Subscription – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [Install Aspose.3D NuGet package][8] - We publish each version of Aspose.3D for .NET API as a NuGet package on the NuGet gallery and recommend our clients upgrade old version to the latest one.
*   [Release Notes][9] - For details on API fixes, please check Release Notes having a complete list of the new features.

We hope you will enjoy this new release that save time and huge efforts for related files manipulation. The API is quite simple and can easily be used in any application.




[1]: https://www.nuget.org/packages/Aspose.3d/18.1.0
[2]: https://docs.aspose.com/display/3dnet/Create+and+Read+an+Existing+3D+Scene#CreateandReadanExisting3DScene-Readinga3DScene
[3]: https://docs.aspose.com/display/3dnet/Create+rectangular+Torus+in+3D+Scene
[4]: http://www.aspose.com/products/3d/net
[5]: https://forum.aspose.com/c/3d
[6]: https://docs.aspose.com/display/3dnet/Home
[7]: https://github.com/aspose3D/Aspose_3d_NET
[8]: https://www.nuget.org/packages/Aspose.3d
[9]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+18.1+-+January+2018




