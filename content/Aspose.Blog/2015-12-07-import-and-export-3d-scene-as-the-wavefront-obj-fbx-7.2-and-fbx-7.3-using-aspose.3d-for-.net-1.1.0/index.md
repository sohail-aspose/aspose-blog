---
title: 'Import and Export 3D Scene as Wavefront OBJ, FBX 7.2 and FBX 7.3 using Aspose.3D for .NET 1.1.0'
date: Mon, 07 Dec 2015 15:27:47 +0000
draft: false
url: /2015/12/07/import-and-export-3d-scene-as-the-wavefront-obj-fbx-7.2-and-fbx-7.3-using-aspose.3d-for-.net-1.1.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for NET APIs">}}


We are pleased to announce the version 1.1.0 of the Aspose.3D for .NET API. This second version of the Aspose.3D API covers more 3D formats, including import and export of the Wavefront's OBJ, FBX 7.2 (ASCII, Binary) and FBX 7.3 (ASCII, Binary) formats. The Wavefront's OBJ format supports multiple objects, index based polygon, vertex position, UV coordinates, normals, object smoothing and external materials. In general, it is also a universally accepted format. This release also includes the most recent bug fixes and enhancements.

## 3D Wavefront OBJ Support

Aspose.3D library provides an easy API to create Wavefront's OBJ files. Developers can now add vertices, polygons and external materials to define a 3D object. Following help topics show, how developers can read and save a scene in the supported formats: [Read an Existing 3D Scene][1], [Save 3D Scenes Overview][2]

## Extended FBX Support

In the previous version, we added support of the FBX 7.4 (ASCII, Binary) and FBX 7.5 (ASCII, Binary) formats. From this recent API version, developers would be able to save a 3D scene in the FBX 7.2 (ASCII, Binary) and FBX 7.3 (ASCII, Binary) formats too.

In the first version of Aspose.3D API, the Save method of the Scene class was also closing the resultant file stream. We have fixed this defect because the developers were not able to save the resultant file stream in the local space. We have left the resultant stream unclosed after Open/Save, developers are now responsible for closing the stream.

## Public API Changes

The following API changes in the new version are also worth noting:

*   The FBX7200ASCII format option has been added in the FileFormat enum. It represents ASCII FBX file format, with 7.2.0 version.
*   The FBX7200Binary format option has been added in the FileFormat enum. It represents Binary FBX file format, with 7.2.0 version.

The FBX7300ASCII format option has been added in the FileFormat enum. It represents ASCII FBX file format, with 7.3.0 version.

*   The FBX7300Binary format option has been added in the FileFormat enum. It represents Binary FBX file format, with 7.3.0 version.
*   The WavefrontOBJ format option has been added in the FileFormat enum. It represents Wavefront's Obj file format.
*   The WavefrontOBJ format option has been added in the FileFormatType enum. It represents Wavefront's Obj file format.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][3].
*   [Download Aspose.3D for .NET][4]
*   [Aspose.3D product family forum][5] - Post your technical questions and queries, or any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][6] – help documentation and API reference documents.
*   [Enable Blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.3D for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you’ll enjoy this new release that saves time and effort. The API is quite simple and developers can use it in application easily.




[1]: https://docs.aspose.com/display/3dnet/Create+and+Read+an+Existing+3D+Scene#CreateandReadanExisting3DScene-Readinga3DScene
[2]: https://docs.aspose.com/display/3dnet/Save+a+3D+Document
[3]: http://www.aspose.com/.net/3d-component.aspx
[4]: http://www.aspose.com/community/files/51/.net-components/aspose.3d-for-.net/default.aspx
[5]: http://forum.aspose.com
[6]: http://docs.aspose.com/display/3dnet/Home
[7]: https://blog.aspose.com/
[8]: https://github.com/aspose3D/Aspose_3d_NET




