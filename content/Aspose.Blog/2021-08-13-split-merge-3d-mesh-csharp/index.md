---
title: 'Split or Merge 3D Mesh in 3D File Programmatically in C#'
seoTitle: "Split or Merge 3D Mesh in 3D File Programmatically in C#"
description: "You can split or merge mesh in a 3D scene programmatically using C#. Mesh splitter or merger API with different planes and materials."
date: Fri, 13 Aug 2021 20:56:00 +0000
draft: false
url: /2021/08/13/split-merge-3d-mesh-csharp/
author: Farhan Raza
summary: 'You can split all meshes of a 3D scene into several sub-meshes. Likewise, you can merge multiple meshes into a single mesh programmatically using C#. This article covers the splitting and merging of 3D meshes in different scenarios.'
tags: ['merge mesh in 3D', 'merge meshes in 3D', 'split mesh in 3D']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/split-merge-mesh.png" alt="split merge mesh">}}


You can split all meshes of a 3D scene into several sub-meshes. Likewise, you can merge multiple meshes into a single mesh programmatically using C#. This article covers the splitting and merging of 3D meshes in different scenarios:

*   [3D Scene Meshes Splitter or Merger – C# API Installation][1]
*   [Split Meshes of a Scene Per Material Programmatically using C#][2]
*   [Split a Mesh by a Specific Material Programmatically using C#][3]
*   [Merge Meshes in a 3D file into a Single Mesh Programmatically in C#][4]

## 3D Scene Meshes Splitter or Merger – C# API Installation {#section1}

[Aspose.3D for .NET][5] API can be used to split or merge 3D meshes programmatically using C#. You can configure the API by installing it from the [Downloads][6] section, or with the below [NuGet][7] installation command:

```
PM> Install-Package Aspose.3D
```

## Split Meshes of a Scene Per Material Programmatically using C# {#section2}

A 3D file like the FBX format can contain several meshes of a scene. You can split all meshes into several sub meshes per material if the mesh has not been assigned a single material. Please follow the steps below for splitting meshes of a scene per material:

1.  Load input 3D file.
2.  Split all meshes with the [SplitMesh][8] method.
3.  Save output file with the splitted meshes.

The following code shows how to split meshes of a scene per material programmatically using C#:

{{< gist aspose-com-gists 634dbc04f47028fe3df49ec2d51cf625 "Split-Mesh.cs" >}}

## Split a Mesh by a Specific Material Programmatically using C# {#section3}

You can split a mesh by manually specifying the material. In this way, you can create several objects containing only one material. For demonstration purposes, the below code creates a mesh of a box with 6 planes. Then you will split a primitive mesh by manually specifying the material using the following steps:

1.  Create a mesh of a box with six planes.
2.  Secondly, create a material element and specify indexes for each plane.
3.  Split the Mesh using [SplitMeshPolicy][9] enumeration.

The code below explains how to split a mesh by specific material programmatically using C#:

{{< gist aspose-com-gists 634dbc04f47028fe3df49ec2d51cf625 "Split-Mesh-Box.cs" >}}

## Merge Meshes in a 3D file into a Single Mesh Programmatically in C# {#section4}

You can merge different meshes into a single valid mesh with the below steps:

1.  Load input 3D scene file.
2.  Merge all meshes.
3.  Finally, encode the merged mesh.

The following code elaborates how to merge meshes into a single mesh programmatically using C#:

{{< gist aspose-com-gists 634dbc04f47028fe3df49ec2d51cf625 "Merge-Mesh.cs" >}}

## Get Free Temporary License

You can get a [Free Evaluation License][10] for testing the API without any limitations.

## Conclusion

In conclusion, you have learned how to merge or split a mesh of a 3D scene. The API exposes different methods for splitting or merging one or multiple meshes, which you can utilize as per your requirements. Moreover, please feel free to visit the [Documentation][11] where several other features are also explained. Please contact us at the [Free Support Forum][12] in case of any queries.

## See Also

[Convert DXF to FBX or glTF GLB file Programmatically in C#][13]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: #section4
[5]: https://products.aspose.com/3d/net/
[6]: https://releases.aspose.com/
[7]: https://www.nuget.org/packages/Aspose.3D
[8]: https://apireference.aspose.com/3d/net/aspose.threed.entities/polygonmodifier/methods/splitmesh/index
[9]: https://apireference.aspose.com/3d/net/aspose.threed.entities/splitmeshpolicy
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/3d/net/
[12]: https://forum.aspose.com/c/3d
[13]: https://blog.aspose.com/2021/07/28/convert-dxf-to-fbx-or-gltf-glb-file-programmatically-in-csharp/





