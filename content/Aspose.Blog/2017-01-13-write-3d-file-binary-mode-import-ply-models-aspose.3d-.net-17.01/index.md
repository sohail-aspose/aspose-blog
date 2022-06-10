---
title: 'Save 3D Meshes in Custom Binary Format and Import PLY Models using C#'
date: Fri, 13 Jan 2017 21:11:05 +0000
draft: false
url: /2017/01/13/write-3d-file-binary-mode-import-ply-models-aspose.3d-.net-17.01/
author: Imran Rafique
summary: ''
tags: ['3D Meshes', 'Convert 3D Mesh to Binary Format', 'Import 3D PLY Models', 'Import PLY', 'Load Options of 3D PLY']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for NET APIs">}}


We are pleased to announce the availability of [new version 17.01 of Aspose.3D for .NET API][1]. The new version adds support for importing PLY models. Developers can import PLY (ASCII and Binary) models into the Aspose.3D API, and then export them in any supported 3D format. The new version also integrates the feature of writing a 3D file in the custom binary mode. All the regular bug fixes and enhancements have also been included. Developers can install Aspose.3D Nuget package in their .NET applications because we publish each version as a NuGet package on the NuGet gallery. We recommend our clients upgrade an old version of the Aspose.3D API to this latest one. For details on API fixes, please check [Release Notes][2] having a complete list of the features, enhancements, and bug fixes.

## Load 3D File and Save Meshes in Custom Binary Format

Using Aspose.3D for .NET API, developers can already load all supported 3D files. Developers can also retrieve meshes and the new public API changes allow to save the meshes in custom binary format. The binary file size remains the same as the data we store like the minimum workable size. This feature would also help our clients manipulate bigger 3D models more effectively. Please check this help topic to save meshes in custom binary format: [Save 3D Meshes in Custom Binary Format][3]

## Import an Existing PLY File into the Aspose.3D API

PLY is a computer file format known as the Polygon File Format or the Stanford Triangle Format. It is one of the simplest formats to read and write a 3D mesh. Using Aspose.3D API, developers can now import any existing PLY (ASCII or Binary) model. Developers would also be able to load a PLY file and then save in any supported 3D file format. Please check these help topics to know how to import an existing PLY file: [Reading a 3D Scene][4] and [Specify Load Options of 3D PLY][5].

## Public API Changes

The following API changes in the new version are also worth noting:

*   A PLY format entry is added in the Aspose.ThreeD.FileFormat class. It helps in loading 3D PLY models.
*   Aspose.ThreeD.Formats.PLY.PlyLoadOptions class has been added. It specifies load settings to load a PLY model into the Aspose.3D API.
*   Aspose.ThreeD.GlobalTransform class has been added. The GlobalTransform class provides exactly the same interface like Transform but all its properties are read-only. It is useful for global transform purposes.
*   The GlobalTransform member is added to Aspose.ThreeD.Node class. It allows accessing the node's global transform.
*   The Polygons member is added to Aspose.ThreeD.Entities.Mesh class. It allows to get all polygons inside the mesh, each polygon is an array of polygon vertex index.
*   The CreateStream member from Aspose.ThreeD.Formats.IOConfig class has been removed. This was marked as obsolete in version 16.11.0, the new interface FileSystem was introduced in version 16.11.0 which provides more extensibility.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][6]
*   [Download Aspose.3D for .NET][7]
*   [Aspose.3D product family forum][8] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][9] – help documentation and API reference documents.
*   [Enable Blog Subscription][10] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Migrate from Earlier Versions of Aspose.3D API – We keep track of Aspose.3D API change version by version. So we recommend getting help from this section while upgrading to the latest API version or if Aspose.3D API code is broken at some stage.

We hope you’ll enjoy this new release that saves time and effort. The API is quite simple and developers can use it in application easily.




[1]: http://downloads.aspose.com/3d/net/new-releases/aspose.3d-for-.net-17.01/
[2]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+17.01+Release+Notes
[3]: https://docs.aspose.com/display/3dnet/Save+3D+Meshes+in+Custom+Binary+Format
[4]: https://docs.aspose.com/display/3dnet/Create+and+Read+an+Existing+3D+Scene#CreateandReadanExisting3DScene-Readinga3DScene
[5]: https://docs.aspose.com/display/3dnet/Specify+3D+File+Load+Options#Specify3DFileLoadOptions-UseofthePlyLoadOptions
[6]: http://products.aspose.com/3d/net
[7]: http://downloads.aspose.com/3d/net
[8]: http://forum.aspose.com
[9]: http://docs.aspose.com/display/3dnet/Home
[10]: https://blog.aspose.com/category/aspose-products/aspose-3d-product-family
[11]: https://github.com/aspose3D/Aspose_3d_NET




