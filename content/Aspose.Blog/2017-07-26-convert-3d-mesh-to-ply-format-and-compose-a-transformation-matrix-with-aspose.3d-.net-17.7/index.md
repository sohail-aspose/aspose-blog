---
title: 'Convert 3D Mesh to PLY Format and Compose a Transformation Matrix in C#'
date: Wed, 26 Jul 2017 04:52:31 +0000
draft: false
url: /2017/07/26/convert-3d-mesh-to-ply-format-and-compose-a-transformation-matrix-with-aspose.3d-.net-17.7/
author: Imran Rafique
summary: ''
tags: ['3D mesh to PLY', 'composing transformation matrix', 'transformation matrix']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for NET APIs">}}


We are pleased to announce the availability of [new version 17.7 of Aspose.3D for .NET API][1]. The new version 17.7 of the API has been released with the support of converting a mesh of any 3D object to PLY format, also developers can simplify the creation of the transform matrix by calling newly added methods in the Matrix4 class. We have enhanced the API usage by incorporating new features and regular bug fixes.

## Convert a Mesh of Any 3D Object to PLY Format

The PLY format describes an object as a collection of vertices, faces, and other elements, along with properties such as color and normal direction that can be attached to these elements. A PLY file contains a description of exactly one object. Aspose.3D for .NET API has the support of retrieving the mesh of any existing 3D object. With the help of this new API version 17.7, developers can convert that mesh to the PLY file. Please refer to this help topic: [Convert Mesh of a single 3D object in PLY file][2]

## Simplify the Composing of the Transformation Matrix

Typically, developers might need a sequence of transformations to position 3D objects in a scene. With the help of this new API version 17.7, they can compose a matrix in two transformation orders known as **Append** and **Prepend**. All transformation matrix steps are narrated in this help topic: [Simplify the creation of transformation matrix by the chain operations][3]

Besides this, the bug fixes have improved the rendering of FBX files and also preserves UVs in respective of the 3DS Max modeling tool.

## Public API Changes

The following API changes in the new version are also worth noticing:

*   Aspose.ThreeD.Utilities.ComposeOrder and Aspose.ThreeD.Utilities.TransformBuilder classes are added. These classes simplify the creation of the transformation matrix by the chain operations.
*   Aspose.ThreeD.Formats.PlySaveOptions class has been added. It allows defining details of the Ply format.
*   Aspose.ThreeD.Formats.PlyFormat class has been added. It allows encoding single mesh to PLY format.
*   PLY member is added in the Aspose.ThreeD.FileFormat class. It allows converting a 3D scene to PLY format.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][4]
*   [Download Aspose.3D for .NET][5]
*   [Aspose.3D product family forum][6] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][7] – help documentation and API reference documents.
*   [Enable Blog Subscription][8] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [Install Aspose.3D NuGet package][10] - We publish each version of Aspose.3D for .NET API as a NuGet package on the NuGet gallery and recommend our clients upgrade the old version to the latest one.
*   [Release Notes][11] - For details on API fixes, please check Release Notes having a complete list of the new features.

We hope you will enjoy this new release that saves time and huge efforts for related file manipulation. The API is quite simple and can easily be used in any application.




[1]: https://downloads.aspose.com/3d/net/new-releases/aspose.3d-for-.net-17.7/
[2]: https://docs.aspose.com/display/3dnet/Convert+Mesh+of+a+single+3D+object+in+PLY+file
[3]: https://docs.aspose.com/display/3dnet/Simplify+the+creation+of+transformation+matrix+by+the+chain+operations
[4]: https://products.aspose.com/3d/net
[5]: http://downloads.aspose.com/3d/net
[6]: https://forum.aspose.com/c/3d
[7]: http://docs.aspose.com/display/3dnet/Home
[8]: https://blog.aspose.com/category/aspose-products/aspose-3d-product-family
[9]: https://github.com/aspose3D/Aspose_3d_NET
[10]: https://www.nuget.org/packages/Aspose.3d
[11]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+17.7+Release+Notes




