---
title: 'Save 3D Scene to Collada Format, Detect the Type of 3D File, Triangulate a Polygon and Hardware Based Rendering of 3D Geometry using Aspose.3D for .NET 2.1.0'
date: Thu, 08 Sep 2016 00:29:39 +0000
draft: false
url: /2016/09/08/save-3d-scene-to-collada-format-detect-the-type-of-3d-file-triangulate-a-polygon-and-hardware-based-rendering-of-3d-geometry-using-aspose.3d-for-.net-2.1.0/
author: Imran Rafique
summary: ''
tags: ['Convert 3D Scene to Collada', 'Detect 3D File Type', 'Hardware Based Rendering of 3D Geometry', 'Triangulate a Polygon']
categories: ['Aspose.3D Product Family']
---

[![Aspose.3D for NET APIs][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2015/10/Aspose.3d-for-net-100x100.png)

[](https://blog.aspose.com/wp-content/uploads/sites/2/2015/10/Aspose.3d-for-net-100x100.png)We are pleased to announce the availability of [new version 2.1.0 of Aspose.3D for .NET API][2]. The new version allows developers to export 3D files to Collada format, detect the format of any supported 3D file, pick vertices on a polygon, and then form triangles. Developers can also program the GPU (Graphics Processing Unit) to set up the graphics hardware for rendering 3D geometry. Developers can install an Aspose.3D Nuget package in their .NET applications because we publish each version as [a NuGet package on the NuGet gallery][3]. We recommend our clients upgrade old version of the Aspose.3D API to this latest one. For details on API fixes, please check Release Notes having a complete list of the features, enhancements and bug fixes.

## Convert a 3D Scene to Collada Format

Aspose.3D API has added support of converting all 3D files (Discreet 3DS, FBX, STL, Universal 3D and WavefrontOBJ) to Collada format. The Collada is an open XML file format for 3D assets, supported by various 3D software packages. Using the recent version 2.1.0 or higher, developers may import any supported 3D scene, and then export to a Collada 3D format.

## Detect the Type of 3D File

The file format identification is the process of figuring out the format of a sequence of bytes. Aspose.3D API allows developers to detect the type of all supported 3D files before loading them for any manipulation purpose. This help topic shows how developers detect the type of a 3D file: Detect the Type of a 3D File

## Create Hardware and Render 3D Geometry

Using Aspose.3D API, developers can program the GPU (Graphics Processing Unit) and set up the graphics hardware for rendering 3D geometry instead of the fixed function pipeline. There are several approaches to program GPUs. Aspose.3D API uses graphics APIs such as OpenGL 4.0, DirectX 11, DirectX 9 and Vulkan to program the GPU. This help topic explains how to create a hardware and render a 3D geometry: Hardware Based Rendering of 3D Geometry

## Triangulation of a Polygon

A polygonal curve is a finite chain of line segments. Line segments called edges, their endpoints called vertices. A simple polygon is a closed polygonal curve without self-intersection. Using Aspose.3D for .NET API, developers can triangulate the polygons. In short, any polygon can be divided into triangles. Developers might pick vertices from a polygon area, and then form triangles by calling algorithm of triangulation. This help topic explains how to triangulate a polygon: Triangulation of a Simple Polygon

## Public API Changes

The following API changes in the new version are also worth noting:

*   ColladaSaveOptions, Discreet3DSSaveOptions, ObjSaveOptions, STLSaveOptions and FBXSaveOptions classes have been added.
    
*   Discreet3DSLoadOptions, ObjLoadOptions, STLLoadOptions and U3DLoadOptions classes have been added.
    
*   The overloads of the Open and Save methods have been added to Scene class.
    
*   The FillDummyIndexArray property of FBXConfig Class has been added.
    
*   The Detect, CreateLoadOptions and CreateSaveOptions methods have been added to FileFormat Class.
    
*   The Excluded property has been added to the Entity and Node classes.
    
*   The RenderState class and BlendFactor, CompareFunction, CullFaceMode, FrontFace, PolygonMode, StencilAction and StencilState enums have been added.
    
*   An abstract class ShaderSource and subclass GLSLSource have been added.
    
*   The ShaderException, ShaderProgram and ShaderVariable classes have been added.
    
*   The VariableSemantic enum has been added.
    
*   The IBuffer, IIndexBuffer and IVertexBuffer interfaces have been added.
    
*   The IndexDataType enum has been added.
    
*   The RenderResource, ManualEntity and RenderableResource classes have been added.
    
*   The RenderQueueGroupId and DrawOperation enums have been added.
    
*   The IRenderable interface has been added.
    
*   The overloads of Triangulate method have been added to PolygonModifier class.
    
*   The CreateVertexBuffer, CreateIndexBuffer, CreateTextureUnit, CreateRenderState and CreateShaderProgram methods have been added to the RenderFactory class.
    
*   The BindRenderState, DrawIndexed, Draw and SubmitRenderTask methods have been added in the Renderer class.
    
*   The RenderStage and Shader properties have been added in the Renderer class.
    

This version also addresses an enhancement to display a proper message on 3D models if the used texture file is missing. It also exposes the low-level APIs to customize the rendering procedure. These enhancements and bug fixes improve performance and accuracy of Aspose.3D API. Please check a list of the resolved defects:

*   Fixed: Diffuse/Specular/Emissive won't work if no texture is used.
    
*   Fixed: The display texture is not found on 3D model.
    
*   Fixed: Allow Vector2/Vector3/Vector4/Quaternion to be editable in the property grid.
    

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][4]
    
*   [Download Aspose.3D for .NET][5]
    
*   [Aspose.3D product family forum][6] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
    
*   Aspose.3D for .NET online documentation – help documentation and API reference documents.
    
*   [Enable Blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
    
*   [Aspose.3D for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
    
*   Migrate from Earlier Versions of Aspose.3D API – We keep track of Aspose.3D API change version by version. So we recommend to get help from this section while upgrading to the latest API version or if Aspose.3D API code is broken at some stage.
    

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.

# _convert 3d files_




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/10/Aspose.3d-for-net-100x100.png "Aspose.3d- for-net-100x100"
[2]: http://www.aspose.com/downloads/3d/net/new-releases/aspose.3d-for-.net-2.1.0/
[3]: https://www.nuget.org/packages/Aspose.3d
[4]: http://www.aspose.com/.net/3d-component.aspx
[5]: http://www.aspose.com/community/files/51/.net-components/aspose.3d-for-.net/default.aspx
[6]: http://www.aspose.com/community/forums/aspose.3d-product-family/535/showforum.aspx
[7]: https://blog.aspose.com/ "Aspose.3D for .NET Blog Subscription"
[8]: https://github.com/aspose3D/Aspose_3d_NET




