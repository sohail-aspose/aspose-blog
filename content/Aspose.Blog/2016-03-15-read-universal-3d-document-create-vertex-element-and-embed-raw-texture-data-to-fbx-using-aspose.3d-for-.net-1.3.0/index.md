---
title: 'Read Universal 3D Document and Create Vertex Element using Aspose.3D for .NET 1.3.0'
date: Tue, 15 Mar 2016 12:35:34 +0000
draft: false
url: /2016/03/15/read-universal-3d-document-create-vertex-element-and-embed-raw-texture-data-to-fbx-using-aspose.3d-for-.net-1.3.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for NET APIs">}}


We’re pleased to announce the availability of new version 1.3.0 of the Aspose.3D for .NET API and let our community know about the progress. This new version has better performance than previous. It allows developers to load a Universal 3D document and get the internal elements programmatically. Probably, we’ll add support of exporting a Universal 3D document to other supported formats in the next version. Our product team is working hard to cover all aspects of the Universal 3D format. It also allows developers, to embed the raw content to the texture of FBX, create a vertex element by passing reference and mapping modes, and initialize Vector4 object by passing Vector3 class object. Besides this, we have changed certain namespaces and classes’ names following the coding guidelines widely accepted by Microsoft .NET developers because it improves readability and makes sense in the context in which it is used.

## Load a Universal 3D File and Get Internal Elements

In the Aspose.3D API, we have implemented a Universal 3D file reader, which allows developers to load and get the internal elements of the U3D (Universal 3D) file in the same way as with other supported formats. This article explains how to load all supported 3D files: [Read an Existing 3D Scene][1]

## Create Vertex Element by Assigning Reference and Mapping Modes

Previously, the CreateElement and CreateElementUV methods of the Mesh class were creating the vertex element without assigning the reference and mapping modes. Developers were setting MappingMode and ReferenceMode properties of the VertexElementNode class object using separate lines of code. Using the version 1.3.0 and later, developers would be able to set these properties at once while calling the CreateElement and CreateElementUV methods of the Mesh class which makes code shorter.

**Sample code \[.NET, C#\]**

```
// call CreateElement method of the Mesh object
VertexElementNormal elementNormal = mesh.CreateElement(VertexElementType.Normal) as VertexElementNormal;
// Specify normal per control point.
elementNormal.MappingMode = MappingMode.ControlPoint;
// The data is directly referenced.
elementNormal.ReferenceMode = ReferenceMode.Direct;
```

**The new alternative approach:**

```
// call overloaded CreateElement method of the Mesh object
VertexElementNormal elementNormal = mesh.CreateElement(VertexElementType.Normal, MappingMode.ControlPoint, ReferenceMode.Direct) as VertexElementNormal;
```

This help topic shows how developers set up surface normal or UV on the cube: [Set Up Normals or UV on the Cube][2]

## Embed Raw Content Data inside the Texture for FBX

The Content property has added to the Texture class to embed the raw content data inside the texture for FBX document. It allows developers to get or set the binary content of the texture by loading texture from the external file. It is optional and specific to the FBX format.

**Sample code \[.NET, C#\]**

```
// initialize Texture class object
Texture texture = new Texture();
// set file name
texture.FileName = "embedded-texture.png";
// set binary content
texture.Content = File.ReadAllBytes("c:\\test.png");
```

This help topic shows how developers embed texture in the material of a 3D object: [Add Material to the Cube][3]

## Public API Changes

The following API changes in the new version are also worth noting:

*   Namespace Aspose.ThreeD.Animations has been changed to Aspose.ThreeD.Animation
*   Class Aspose.ThreeD.Animations.Animation has been changed to Aspose.ThreeD.Animation.AnimationNode
*   Namespace Aspose.ThreeD.IO has been changed to Aspose.ThreeD.Formats
*   Namespace Aspose.ThreeD.Utils has changed to Aspose.ThreeD.Utilities
*   Added a Decompose method in Matrix4 class - It is a mathematical utility function used to decompose an affine transformation matrix.
*   Added a new constructor in Vector4 class to receive a Vector3 object parameter - It makes easier to construct a Vector4 based on the Vector3. The fourth value of the Vector4 presents plane w and its default value is 1.
*   Added a Content property in Texture class - It allows to embed raw texture data inside the Texture instance for FBX documents.
*   The Universal3D option is added in the FileFormat enum.
*   The new overloads for Geometry.CreateElement and Geometry.CreateElementUV are added - It allows developers to create a new vertex element and assign reference and mapping modes at once, to make code shorter.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][4].
*   [Download Aspose.3D for .NET][5]
*   [Aspose.3D product family forum][6] - Post your technical questions and queries, or any other problem you faced while running Aspose.3D APIs.
*   Aspose.3D for .NET online documentation – help documentation and API reference documents.
*   [Enable Blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   How to Migrate from Earlier Versions of Aspose.3D API – We keep track of Aspose.3D API change version by version. So we recommend to get help from this section while upgrading to the latest API version or if Aspose.3D API code is broken at some stage.

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://docs.aspose.com/display/3dnet/Create+and+Read+an+Existing+3D+Scene#CreateandReadanExisting3DScene-Readinga3DScene
[2]: https://docs.aspose.com/display/3dnet/Set+up+normals+or+UV+on+the+Cube+and+Add+Material+to+3D+Entities
[3]: https://docs.aspose.com/display/3dnet/Set+up+normals+or+UV+on+the+Cube+and+Add+Material+to+3D+Entities#SetupnormalsorUVontheCubeandAddmaterialtothecube-Addmaterialtothecube
[4]: http://www.aspose.com/.net/3d-component.aspx
[5]: http://www.aspose.com/community/files/51/.net-components/aspose.3d-for-.net/default.aspx
[6]: http://www.aspose.com/community/forums/aspose.3d-product-family/535/showforum.aspx
[7]: https://blog.aspose.com/
[8]: https://github.com/aspose3D/Aspose_3d_NET




