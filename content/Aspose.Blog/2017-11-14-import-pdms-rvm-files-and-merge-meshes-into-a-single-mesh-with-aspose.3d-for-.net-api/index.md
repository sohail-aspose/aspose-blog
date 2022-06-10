---
title: 'Import PDMS and RVM Files and Merge Meshes into a Single Mesh with Aspose.3D for .NET'
date: Tue, 14 Nov 2017 04:12:12 +0000
draft: false
url: /2017/11/14/import-pdms-rvm-files-and-merge-meshes-into-a-single-mesh-with-aspose.3d-for-.net-api/
author: Imran Rafique
summary: ''
tags: ['C# .NET 3D API', 'Import PDMS Files', 'Import RVM Files', 'Merge Meshes into a Single Mesh']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for .NET logo">}}


We are pleased to announce the availability of [new version 17.11 of Aspose.3D for .NET API][1]. The new version 17.11 of the API has been released with the support of importing PDMS RVM files and developers can export these RVM files to [the supported file formats][2]. Developers can merge all Meshes of the Scene, a Node and a set of nodes as well as get or set the transparency of the PBR material (only supported for GLTF). We have fixed a defect of exporting incorrect material opacity in GLTF.

## Import RVM file into Aspose.3D API

With the help of Aspose.3D for .NET API, developers can convert RVM file to all supported formats. The RVM file stores 3D power plant project. Developers can import RVM models into the Aspose.3D for .NET API with the constructor or Open member of the Scene class as narrated in this help topic: [Import a 3D model][3] and [Use RVM load options][4]

## Merge all Meshes into a Single Mesh

With the recent version 17.11 of Aspose.3D for .NET API, developers can merge Meshes to a single transformed Mesh. In order to achieve this, three MergeMesh members are added to the PolygonModifier class. Please refer to the code example as documented in this help topic: [Merge Meshes in 3D file][5]

Developers can also control the transparency of PBR material. Aspose.3D for .NET API supports PBR material for only GLTF 2.0, so this improvement will affect the GLTF 2.0 export. This is the code example:

```
// initialize a 3D scene
Scene scene = new Scene();
// add PBR material with transparency factor
scene.RootNode.CreateChildNode("box", new Box()).Material = new PbrMaterial()
                  {Transparency = 0.5, Albedo = new Vector3(Color.AliceBlue)};
// save 3D scene
scene.Save("box.gltf", FileFormat.GLTF2);
```

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][6]
*   [Aspose.3D product family forum][7] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][8] – help documentation and API reference documents.
*   Enable Blog Subscription – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [Install Aspose.3D NuGet package][10] - We publish each version of Aspose.3D for .NET API as a NuGet package on the NuGet gallery and recommend our clients upgrade old version to the latest one.
*   [Release Notes][11] - For details on API fixes, please check Release Notes having a complete list of the new features.

We hope you will enjoy this new release that save time and huge efforts for related files manipulation. The API is quite simple and can easily be used in any application.




[1]: https://www.nuget.org/packages/Aspose.3d
[2]: https://docs.aspose.com/display/3dnet/Save+a+3D+Document
[3]: https://docs.aspose.com/display/3dnet/Create+and+Read+an+Existing+3D+Scene#CreateandReadanExisting3DScene-Readinga3DScene
[4]: https://docs.aspose.com/display/3dnet/Specify+3D+File+Load+Options#Specify3DFileLoadOptions-UseRVMloadoptions
[5]: https://docs.aspose.com/display/3dnet/Merge+Meshes+in+3D+file
[6]: https://products.aspose.com/3d/net
[7]: https://forum.aspose.com/c/3d
[8]: https://docs.aspose.com/display/3dnet/Home
[9]: https://github.com/aspose3D/Aspose_3d_NET
[10]: https://www.nuget.org/packages/Aspose.3d
[11]: https://docs.aspose.com/display/3dnet/Home




