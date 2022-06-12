---
title: '.NET 3D Modeing and File Manipulation API - Aspose.3D for .NET 1.0.0'
seoTitle: ".NET 3D Modeing and File Manipulation API - Aspose.3D for .NET 1.0.0"
description: ""
date: Mon, 23 Nov 2015 16:07:55 +0000
draft: false
url: /2015/11/23/.net-3d-modeing-and-file-manipulation-api-read-write-convert-3d-files/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for NET APIs">}}


We are pleased to announce the first version 1.0.0 of the new [Aspose.3D for .NET][1] API. This addition, in the Aspose APIs, opens a new hole of automatic 3D modeling, brings agility, and enables developers to be innovative and figures out the new ways. As we have narrated in our earlier post that it is a class library and supports FBX and STL formats. For now, it supports FBX (ASCII, Binary) versions 7.5 and 7.4. We are pleased to let our community know that we have added support of FBX (ASCII, Binary) version 7.3 too. It is expected in the next release version.

## Why Use Aspose.3D for .NET API

3D computer graphics are generally used and they are almost too common to see anywhere, let it be movies, structural engineering, the automobile industry, product designs, advertisements and many more. Although they are commonly seen, that doesn’t mean they are easily created. In order to ideally control 3D objects, we offer Aspose.3D API because it covers advance functionalities that would be required a full complex project to create from scratch.

## Load and Convert a 3D File

The Aspose.3D API allows developers to save a 3D file to any supported file format. Below is the code for converting an FBX to STL file format:

```
// load an FBX file into Aspose.3D.
Aspose.ThreeD.Scene document = new Aspose.ThreeD.Scene();
document.Open(MyDir + "Document.fbx");
// Save it in the STL format.
document.Save(MyDir + "Output.stl", FileFormat.STLASCII);
```

## How to Create a Mesh

A Mesh is defined by a set of control points and the many n-sided polygons as needed. This sample code creates a mesh of the Cube shape:

```
// initialize control points
Vector4[] controlPoints = new Vector4[]{
    new Vector4( -5.0, 0.0, 5.0, 1.0),
    new Vector4( 5.0, 0.0, 5.0, 1.0),
    new Vector4( 5.0, 10.0, 5.0, 1.0),
    new Vector4( -5.0, 10.0, 5.0, 1.0),
    new Vector4( -5.0, 0.0, -5.0, 1.0),
    new Vector4( 5.0, 0.0, -5.0, 1.0),
    new Vector4( 5.0, 10.0, -5.0, 1.0),
    new Vector4( -5.0, 10.0, -5.0, 1.0)
};
// initialize mesh object
Mesh mesh = new Mesh();
// add control points to the mesh
mesh.ControlPoints.AddRange(controlPoints);

// create polygons to mesh
// front face (Z+)
mesh.CreatePolygon(new int[] { 0, 1, 2, 3 });
// right side (X+)
mesh.CreatePolygon(new int[] { 1, 5, 6, 2 });
// back face (Z-)
mesh.CreatePolygon(new int[] { 5, 4, 7, 6 });
// left side (X-)
mesh.CreatePolygon(new int[] { 4, 0, 3, 7 });
// bottom face (Y-)
mesh.CreatePolygon(new int[] { 0, 4, 5, 1 });
// top face (Y+)
mesh.CreatePolygon(new int[] { 3, 2, 6, 7 });
```

Please check this help topic to get inside other details: Create a 3D Cube Mesh.

## Place a Cube Shape and Save 3D Scene

Aspose.3D API allows developers to create the shape of the mesh geometry, place shapes in the scene and then save it in any supported file format:

```
// initialize scene object
Scene scene = new Scene();
// initialize Node class object for the shape cube
Node cubeNode = new Node("cube");
/*mesh is the same object as prepared under above sub heading "How to Create a Mesh"*/
// point cube node to the Mesh geometry
cubeNode.Entity = mesh;
// add cube node to a scene
scene.RootNode.ChildNodes.Add(cubeNode);

// this can also be done in a more elegant way:
// scene.RootNode.ChildNodes.Add(new Node("cube", mesh));

// save 3D scene in the supported file format
scene.Save(@"c:\temp\cube.fbx", FileFormat.FBX7500ASCII);
```

Please check this help topic to get inside other details: Create a Scene having 3D Cube Shape

## Implement 3D Mesh Instancing Technique

In the RTS (Real-time strategy) games like we can always see multiple NPCs (Non-Player Character) with the same 3D model, maybe in different colors, rendering engines usually share the same mesh geometry data across different NPCs, this technique is called Instancing. This technique is supported by Aspose.3D API as follows:

```
// initialize scene object
Scene scene = new Scene();

// define color vectors
Vector3[] colors = new Vector3[] {
    new Vector3(1, 0, 0),
    new Vector3(0, 1, 0),
    new Vector3(0, 0, 1)
};

int idx = 0;
foreach(Vector3 color in colors)
{
    // initialize cube node object
    Node cube = new Node("cube");
    /*mesh is the same object as prepared under 
     above sub heading "How to Create a Mesh"*/
    cube.Entity = mesh;
    LambertMaterial mat = new LambertMaterial();
    // set color
    mat.DiffuseColor = color;
    // set material
    cube.Material = mat;
    // set translation
    cube.Transform.Translation = new Vector3(idx++ * 20, 0, 0);
    // add cube node
    scene.RootNode.ChildNodes.Add(cube);
}

// save 3D scene in the supported file formats
scene.Save("cube.fbx", FileFormat.FBX7500ASCII);
```

Many other features are supported by Aspose.3D for .NET API:

1.  [Set up Normals or UV on Graphic Objects][2]
2.  [Add the Transformation to a Node][3]
3.  [Adding Material to the Shape Node][4]
4.  [Add an Asset Information to 3D Scene][5]
5.  [Add Animation to a Graphic Object][6]

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][7].
*   [Download Aspose.3D for .NET][8]
*   [Aspose.3D product family forum][9] - Post your technical questions and queries, or any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][10] – help documentation and API reference documents.
*   [Enable Blog Subscription][11] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes, and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.3D for .NET Examples][12] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you’ll enjoy this new release that saves time and effort. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/3d/net
[2]: https://docs.aspose.com/display/3dnet/Set+up+normals+or+UV+on+the+Cube+and+Add+Material+to+3D+Entities
[3]: https://docs.aspose.com/display/3dnet/Adding+Transformation+to+the+Node
[4]: https://docs.aspose.com/display/3dnet/Set+up+normals+or+UV+on+the+Cube+and+Add+Material+to+3D+Entities
[5]: http://docs.aspose.com/display/3dnet/Add+an+Asset+Information+and+Flip+Coordinate+System+in+3D+Formats#AddanAssetInformationandFlipCoordinateSystemin3DFormats-AddanAssetInformationto3DScene
[6]: https://docs.aspose.com/display/3dnet/Add+Animation+Property+and+Setup+Target+Camera+in+3D+document
[7]: https://products.aspose.com/3d/net
[8]: https://downloads.aspose.com/3d/net
[9]: http://forum.aspose.com
[10]: http://docs.aspose.com/display/3dnet/Home
[11]: https://blog.aspose.com/
[12]: https://github.com/aspose3D/Aspose_3d_NET




