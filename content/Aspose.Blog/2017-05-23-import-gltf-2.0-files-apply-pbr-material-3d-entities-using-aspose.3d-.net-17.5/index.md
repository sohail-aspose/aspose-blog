---
title: 'Import GLTF 2.0 Files using C# with Aspose.3D for .NET 17.5'
date: Tue, 23 May 2017 00:54:05 +0000
draft: false
url: /2017/05/23/import-gltf-2.0-files-apply-pbr-material-3d-entities-using-aspose.3d-.net-17.5/
author: Imran Rafique
summary: ''
tags: ['3D entities', 'Import GLTF 2.0', 'Physically based Rendering']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for NET APIs">}}


We are pleased to announce the availability of [new version 17.5 of Aspose.3D for .NET API][1]. The new version 17.5 of the API adds support of importing GLTF 2.0 (ASCII and Binary) files in the Aspose.3D API as well as allows developers to apply Physically Based Rendering (PBR) material to 3D entities. Developers may then save the final 3D scene to any supported file format. All 3D import formats are listed on this page: [Import an Existing 3D File][2]. 

All other internal improvements are also incorporated. Developers can install Aspose.3D Nuget package in their .NET applications because we publish each version as [a NuGet package on the NuGet gallery][3]. We recommend our clients upgrade old version of the Aspose.3D API to this latest one. For details on API fixes, please check [Release Notes][4] having a complete list of the new features.

## Import GLTF 2.0 ASCII and Binary Files into Aspose.3D API

GLTF 2.0 (GL Transmission Format) improves the way of storing, transferring and rendering 3D models. With the help of Aspose.3D for .NET API, developers can import existing GLTF 2.0 (ASCII and Binary) models, and then save in any other supported 3D format. The code example demonstrates how to open GLTF 2.0 files using Aspose.3D for .NET API: 

```
// Initialize a Scene class object
Scene scene = new Scene();
// Load an existing 3D document
scene.Open(MyDir + "document.gltf");
```

## Create a 3D Entity with Physically Based Rendering Material

Aspose.3D for .NET offers the capabilities to create an instance of any supported 3D entities, set position in a 3D scene, and then save in the supported file format. Developers would now be able to apply Physically Based Rendering material to that entity instance before saving. This help topic helps to know the way of applying Physically Based Rendering material to an instance of 3D entity: [Apply Physically Based Rendering (PBR) Material to a Box][5]MaterialtoaBox).

```
// initialize a scene
Scene scene = new Scene();
// initialize PBR material object
PbrMaterial mat = new PbrMaterial();
// an almost metal material
mat.MetallicFactor = 0.9;
// material surface is very rough
mat.RoughnessFactor = 0.9;
// create a box to which the material will be applied
var boxNode = scene.RootNode.CreateChildNode("box", new Box());
boxNode.Material = mat;
// save 3d scene into STL format
scene.Save(@"C:\3D\PBR_Material_Box_Out.stl", FileFormat.STLASCII);
```

## Public API Changes

The following API changes in the new version are also worth noticing:

*   Aspose.ThreeD.Shading.PbrMaterial class has been added. It helps in applying Physical Based Rendering (PBR) material to entities and render into 3D models.
*   GLTF2 and GLTF2\_Binary members are added to Aspose.ThreeD.FileFormat class. It helps in importing GLTF 2.0 (ASCII and Binary) files.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][6]
*   [Download Aspose.3D for .NET][7]
*   [Aspose.3D product family forum][8] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   Aspose.3D for .NET online documentation – help documentation and API reference documents.
*   [Enable Blog Subscription][9] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you will enjoy this new release that save time and huge efforts for related files manipulation. The API is quite simple and can easily be used in any application.




[1]: https://downloads.aspose.com/3d/net/new-releases/aspose.3d-for-.net-17.5/
[2]: https://docs.aspose.com/display/3dnet/Create+and+Read+an+Existing+3D+Scene
[3]: https://www.nuget.org/packages/Aspose.3d
[4]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+17.5+Release+Notes
[5]: https://docs.aspose.com/display/3dnet/Set+up+normals+or+UV+on+the+Cube+and+Add+Material+to+3D+Entities#SetupnormalsorUVontheCubeandAddMaterialto3DEntities-ApplyPhysicallyBasedRendering(PBR
[6]: http://www.aspose.com/products/3d/net
[7]: http://downloads.aspose.com/3d/net
[8]: http://www.aspose.com/community/forums/aspose.3d-product-family/535/showforum.aspx
[9]: https://blog.aspose.com/category/aspose-products/aspose-3d-product-family
[10]: https://github.com/aspose3D/Aspose_3d_NET




