---
title: 'Split Mesh of Scene by Material and Build Primitive 3D Models in C#'
date: Mon, 09 May 2016 03:06:28 +0000
draft: false
url: /2016/05/09/split-mesh-of-scene-by-material-and-build-primitive-3d-models-in-csharp/
author: Imran Rafique
summary: ''
tags: ['3D Models', 'Memory Layout of the Vertex', 'Primitives', 'Split Mesh', 'Split Mesh by Material', 'Vertex', 'Vertex Structure']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for NET APIs">}}


[](https://blog.aspose.com/wp-content/uploads/sites/2/2015/10/Aspose.3d-for-net-100x100.png)We’re pleased to announce the availability of new version 1.5.0 of the [Aspose.3D for .NET][1] API. This new version gives the comprehensive features. Developers would be able to, split the mesh of scene by material, get mesh of the primitives, create a scene from the primitive 3D models and convert a mesh to triangle mesh with custom memory layout of the vertex. Besides all the new features, we have enhanced the support of flipping coordinate system in Universal 3D files. Aspose.3D for .NET is now more robust, feature-rich, and easier to use. All these factors make it a great choice for developers.

## Create a Box, Sphere, Plane, Cylinder and Torus Object in the Scene

**Getting the Mesh of Primitive:** Primitives include many of the most basic and most used objects like box, sphere, plane, cylinder, and torus. Developers may include predefined primitives in the scene. They can also get the mesh of any primitive to modify it later as needed. This article explains how to convert the primitive to a mesh: Convert the Primitive to a Mesh

**Build a Scene from Primitive 3D Models:** 3D Modeling is the process of pure creation. For model objects, developers may use several different ways of including the primitive objects. Using Aspose.3D API, developers can now easily create a scene from primitive 3D models. This article explains how to do so: Create a Scene from Primitive 3D Models

## Split the Mesh by Material

Developers may require to automatically split a mesh by material, so that each mesh is only using one material or split mesh by specifying the material. These scenarios could be achieved by using Aspose.3D API. Please check these help topics to go more in the points of interest: Split All Meshes of a Scene Per Material and Split a Mesh by Specifying the Material

## Convert a Mesh to Triangle Mesh with Custom Memory Layout of the Vertex

Developers may convert a mesh to the triangle mesh because any complex structure can be represented as a bunch of triangles. Many graphics software packages and hardware devices operate more efficiently on triangles. The memory layout of Vertex is also important to feed the GPU (Graphics Processing Unit) because the GPU must also know about the vertex layout in order to extract correct attributes from the buffer. This help topic shows how to convert a mesh to the triangle mesh with user defined memory layout of the vertex: Convert a Mesh to Triangle Mesh with Custom Memory Layout of the Vertex

## Public API Changes

The following API changes in the new version are also worth noting:

*   The new interface Aspose.ThreeD.Entities.IMeshConvertible is added - Any class that implements this interface can be converted to mesh.
*   Distreet3DS format is marked as obsolete and the new Discreet3DS format has been introduced.
*   The class Aspose.ThreeD.Entities.Primitive is added - It is derived from the Entity class and also the base class of all primitive classes.
*   The classes Aspose.ThreeD.Entities.Box/Cylinder/Plane/Sphere/Torus are added - These can be used to define scene with simple primitives. Developers can also convert them to mesh automatically.
*   The class Aspose.ThreeD.Entities.TriMesh is added - TriMesh class contains the definition for triangle-based meshes with custom memory layout, which is useful when developer requires to convert the scene to their own proprietary file formats or in rendering.
*   The new classes Aspose.ThreeD.Utilities.FVector2/FVector3/FVector4 are added - These classes present vector components in the float. Only a few modern GPU supports double-precision vector, single-precision float types are more welcomed in real-time rendering world. These replacements will co-exist with the original Vector2/Vector3/Vector4 since they play different roles in Aspose.3D. Double-precision is mainly used to store model's data because it has less accumulated error. Single-precision is mainly used in rendering or user's own proprietary file formats conversion because it has better acceptance and performance. We introduced this set of vectors in Aspose.3D 1.5 because we added support for custom vertex layout, where the float vectors will be frequently used.
*   The new attribute class Aspose.ThreeD.Utilities.SemanticAttribute is added - Developer can define the custom structure for vertex, and use this attribute to mark the semantic of the fields.
*   The new class Aspose.ThreeD.Utilities.VertexDeclaration is added - It describes the memory layout of the vertex.
*   The new enums Aspose.ThreeD.Utilities.VertexFieldDataType/VertexFieldSemantic are added - These enum types annotate the vertex's field's data type and semantic respectively.
*   The new class Aspose.ThreeD.Utilities.VertexField is added - It describes each field in the custom memory layout of Vertex.
*   The new class Aspose.ThreeD.Utilities.Vertex is added - It can be used to access the raw vertex in TriMesh.
*   The new enum Aspose.ThreeD.Entities.SplitMeshPolicy is added - It specifies the data policy used in the mesh splitting algorithm, we support two policies, share data between sub-meshes or each sub-mesh has its own data (Only used data).
*   Three new SplitMesh methods are added to class Aspose.ThreeD.Entities.PolygonModifier:
    *   Split meshes on a specified node to sub-meshes by material definition.
    *   Split all meshes in the given scene to sub-meshes by material definition.
    *   Split the given mesh to sub-meshes by material definition.
*   The new property FlipCoordinateSystem is added in the class Aspose.ThreeD.Formats.Universal3DConfig - It allows users to flip the coordinate system of U3D during import or export.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][2].
*   [Download Aspose.3D for .NET][3]
*   [Aspose.3D product family forum][4] - Post your technical questions and queries, or any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][5] – help documentation and API reference documents.
*   [Enable Blog Subscription][6] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/3d/net
[2]: https://products.aspose.com/3d/net
[3]: https://downloads.aspose.com/3d/net
[4]: http://forum.aspose.com
[5]: https://docs.aspose.com/3d/net
[6]: https://blog.aspose.com/ "Aspose.3D for .NET Blog Subscription"
[7]: https://github.com/aspose3D/Aspose_3d_NET




