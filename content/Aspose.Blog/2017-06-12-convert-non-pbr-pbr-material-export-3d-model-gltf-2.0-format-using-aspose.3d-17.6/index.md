---
title: 'Export 3D Scene to GLTF 2.0 in C# using Aspose.3D for .NET'
date: Mon, 12 Jun 2017 10:57:27 +0000
draft: false
url: /2017/06/12/convert-non-pbr-pbr-material-export-3d-model-gltf-2.0-format-using-aspose.3d-17.6/
author: Imran Rafique
summary: ''
tags: ['Convert 3D scene to GLTF', 'Convert Non-PBR to PBR Material', 'Export 3D Model to GLTF 2.0']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for NET APIs">}}


We are pleased to announce the availability of [new version 17.6 of Aspose.3D for .NET API][1]. The new version 17.6 of the API adds support of exporting 3D scenes to GLTF 2.0 (ASCII or Binary) format. GLTF 2.0 only supports PBR materials and Aspose.3D for .NET API internally converts Non-PBR materials to PBR materials as well as allows developers to customize the convert procedure. The recent version 17.6 also incorporates various bug fixes and internal improvements.

## Export 3D Scene to GLTF 2.0 using C#

With the help of Aspose.3D for .NET API, developers can start the transition of 3D models to GLTF 2.0 to reap performance, portability and to gain quality benefits. GLTF 2.0 only supports PBR materials and PBR materials are a flexible way for 3D content creators to specify the rendering characteristics of their surfaces. During the export of a 3D model, Aspose.3D API internally converts non-PBR materials to PBR materials.

The materials in the scene will remain unchanged, and the developers can customize the conversion behavior. The code example demonstrates the customized export of 3D models to GLTF 2.0 format with Aspose.3D for .NET API: 

```
// initialize a new 3D scene
var s = new Scene();
var box = new Box();
s.RootNode.CreateChildNode("box1", box).Material = new PhongMaterial() {DiffuseColor = new Vector3(1, 0, 1)};
GLTFSaveOptions opt = new GLTFSaveOptions(FileFormat.GLTF2);
//Custom material converter to convert PhongMaterial to PbrMaterial
opt.MaterialConverter = delegate(Material material)
{
    PhongMaterial m = (PhongMaterial) material;
    return new PbrMaterial() {Albedo = new Vector3(m.DiffuseColor.x, m.DiffuseColor.y, m.DiffuseColor.z)};
};
// save in GLTF 2.0 format
s.Save("test.gltf", opt);
```

Please check this help topic to get inside other details: [Customize Non-PBR to PBR Materials Conversion before saving 3D Scenes to GLTF 2.0 Format][2]

## Public API Changes

The following API changes in the new version are also worth noticing:

*   MaterialConverter member is added to Aspose.ThreeD.Formats.GLTFSaveOptions class. It helps in customizing non-PBR to PBR materials conversion.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][3]
*   [Download Aspose.3D for .NET][4]
*   [Aspose.3D product family forum][5] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][6] – help documentation and API reference documents.
*   [Enable Blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [Install Aspose.3D NuGet package][9] - We publish each version of Aspose.3D for .NET API as a NuGet package on the NuGet gallery and recommend our clients upgrade old version to the latest one.
*   [Release Notes][10] - For details on API fixes, please check Release Notes having a complete list of the new features.

We hope you will enjoy this new release that save time and huge efforts for related files manipulation. The API is quite simple and can easily be used in any application.




[1]: https://downloads.aspose.com/3d/net/new-releases/aspose.3d-for-.net-17.6/
[2]: https://docs.aspose.com/display/3dnet/Customize+Non-PBR+to+PBR+Materials+Conversion+before+Saving+3D+Scenes+to+GLTF+2.0+Format
[3]: http://products.aspose.com/3d/net
[4]: http://downloads.aspose.com/3d/net
[5]: http://forum.aspose.com
[6]: http://docs.aspose.com/display/3dnet/Home
[7]: https://blog.aspose.com/category/aspose-products/aspose-3d-product-family
[8]: https://github.com/aspose3D/Aspose_3d_NET
[9]: https://www.nuget.org/packages/Aspose.3d
[10]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+17.6+Release+Notes




