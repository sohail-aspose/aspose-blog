---
title: 'Export 3D Models to RVM Format and Scale Geometries of 3D Scenes in C#'
date: Wed, 27 Dec 2017 12:05:22 +0000
draft: false
url: /2017/12/27/export-3d-models-to-rvm-and-scale-geometries-of-3d-scenes-in-csharp-asp.net/
author: Imran Rafique
summary: ''
tags: ['Export 3D Models to RVM in Csharp', 'Scale Geometries of 3D Scenes in Csharp']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for .NET logo">}}


We are pleased to announce the availability of [new version 17.12 of Aspose.3D for .NET API][1]. The new version 17.12 of the API has been released with the support of scaling geometries in the 3D model as well as manipulating the custom properties of 3D objects. Developers can sort out a child node using FindNode member of the Node instance. In the previous version 17.11, we have added support of importing RVM files and now with the recent version 17.12, developers can export RVM files.

## Export 3D Models to RVM in C#

With the help of Aspose.3D for .NET API, developers can export all supported 3D models to RVM format. The Save method of the Scene class allows to export 3D models as narrated in this help topic: [Save a 3D Document][2]

## Scale Geometries of 3D Scenes

With the recent version 17.12 of Aspose.3D for .NET API, developers can scale a single 3D object or all objects in a 3D scene. In order to achieve this, multiple Scale members are added to the PolygonModifier class. 

```
// scale the model in huge-scene.obj by 0.01 and save it to another file:
Scene scene = new Scene("huge-scene.obj");
// create a Box instance
var box = scene.RootNode.CreateChildNode("box", new Box());
// scale geometries of a single node
PolygonModifier.Scale(box, new Vector3(0.01));
// scale geometries of all nodes
PolygonModifier.Scale(scene, new Vector3(0.01));
scene.Save("scaled-scene.obj", FileFormat.WavefrontOBJ);
```

Please refer to the code example as documented in this help topic: [Scale geometries of a 3D Scene][3]

## Manipulate Custom Properties of 3D Objects

With the help of Aspose.3D for .NET API, developers can add, retrieve, and remove custom properties of 3D objects. In order to achieve this, RemoveProperty, GetProperty, SetProperty members are added in the Node class.

```
// initialize a scene 
Scene scene = new Scene();
// create a Box instance
var box = scene.RootNode.CreateChildNode("box", new Box());
// add custom property
box.SetProperty("property-name", "property-value");
box.SetProperty("property-name2", "property-value2");
// get a custom property by name
Property property = (Property)box.GetProperty("property-name");
// remove the custom property by name or property instance
box.RemoveProperty("property-name");
box.RemoveProperty(property);
// save 3D scene
scene.Save("test.fbx", FileFormat.FBX7400ASCII);
scene.Save("test.gltf", new GLTFSaveOptions(FileFormat.GLTF){SaveExtras = true});
scene.Save("test-2.gltf", new GLTFSaveOptions(FileFormat.GLTF2){SaveExtras = true});
```

Please refer to this help topic: [Manipulate custom properties of a 3D Scene][4]

Furthermore, the FindNode method has been added in the Node class. It helps in retrieving a child node by name. This is the code example:

```
// initialize a 3D scene
Scene scene = new Scene();// create a Box objectscene.RootNode.CreateChildNode("child", new Box());// find a child nodeNode child = scene.RootNode.FindNode("child");
```

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][5]
*   [Aspose.3D product family forum][6] - Post your technical questions, queries, and any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][7] – help documentation and API reference documents.
*   Enable Blog Subscription – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes, and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [Install Aspose.3D NuGet package][9] - We publish each version of Aspose.3D for .NET API as a NuGet package on the NuGet gallery and recommend our clients upgrade the old version to the latest one.
*   [Release Notes][10] - For details on API fixes, please check Release Notes having a complete list of the new features.

We hope you will enjoy this new release that save time and huge efforts for related files manipulation. The API is quite simple and can easily be used in any application.




[1]: https://www.nuget.org/packages/Aspose.3d/17.12.0
[2]: https://docs.aspose.com/display/3dnet/Save+a+3D+Document
[3]: https://docs.aspose.com/display/3dnet/Scale+geometries+of+a+3D+Scene
[4]: https://docs.aspose.com/display/3dnet/Manipulate+custom+properties+of+a+3D+Scene
[5]: http://www.aspose.com/products/3d/net
[6]: https://forum.aspose.com/c/3d
[7]: https://docs.aspose.com/display/3dnet/Home
[8]: https://github.com/aspose3D/Aspose_3d_NET
[9]: https://www.nuget.org/packages/Aspose.3d
[10]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+17.12+-+December+2017




