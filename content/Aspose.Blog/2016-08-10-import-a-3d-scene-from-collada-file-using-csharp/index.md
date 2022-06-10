---
title: 'Import a 3D Scene from Collada File using Aspose.3D for .NET 2.0.0'
date: Wed, 10 Aug 2016 10:45:35 +0000
draft: false
url: /2016/08/10/import-a-3d-scene-from-collada-file-using-csharp/
author: Imran Rafique
summary: ''
tags: ['Apply Visual Effects', 'Capture 3D Viewports', 'Collada', 'Convert Collada file', 'Import Collada Scene', 'Render Viewports', 'viewports of a 3D Scene']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for NET APIs">}}


We’re pleased to announce the availability of new version 2.0.0 of [Aspose.3D for .NET][1] API. The new version allows developers to automatically set up one or multiple viewports in a single screenshot. Using multiple viewports technique can help in visualizing some large sized 3D scenes. Developers may add feature in their applications to capture the specific 3D viewports by positioning a camera and light, and then highlight them in multiple ways to give a better conceptual understanding of a 3D model. Developers may apply various visual effects to these viewports. We have also added four built in visual effects (also known as post-processing effects). We'll allow developers to customize the post-processing algorithms in the future versions. For more details on this version, please take a look at the Release Notes.

## Import a Collada Scene and Save in other 3D Format

Aspose.3D API has added support to import the Collada scenes. Collada is an open XML file format for 3D assets, supported by various 3D software packages. Developers would be able to import 3D scene elements like material, light, camera, texture and geometries (polygon, polylist, triangles, triangle fans and triangle strips). Developers may also import an existing Collada scene, and then save in other supported 3D file formats. We have plans to enhance the import operations of Collada files as well as incorporate the export feature in the upcoming releases.

## Capture and Present Various Viewports of a 3D Scene

Using Aspose.3D API, developers can now capture various new viewports to present complex areas of a 3D scene in better presentable form. They can also save multiple viewports in a single screenshot. Aspose.3D API performs OpenGL rendering. It creates a hardware OpenGL-backend renderer. An initialization error will occur, if the machine has no hardware support of OpenGL 4.0. We'll extend rendering in the future releases. Developers may also render the viewport to a texture or window (using native window handle from Microsoft Windows). This help topic shows how developers can capture and present the viewports of a 3D scene: Capture the Viewports of 3D Scene and Render to a Texture or Window

## Apply Visual Effects on Saving a 3D View

Aspose.3D API has added support of four built in effects like grayscale, pixelated, edge detection and blur. These visual effects help in enhancing a 3D view. In the future, we have plans to customize the algorithms. This help topic shows how developers can apply visual effects on a 3D view: Apply Visual Effects on Saving 3D Views

## Public API Changes

The following API changes in the new version are also worth noting:

*   The new Collada format is added to Aspose.ThreeD.FileFormatType and Aspose.ThreeD.FileFormat enums.
*   Distreet3DS format has been removed because the new Discreet3DS format has already been included.
*   Aspose.ThreeD.Utilities.BoundingBox and Aspose.ThreeD.Utilities.BoundingBoxExtent classes are added - The BoundingBox and BoundingBoxExtent classes represent bounding box of a 3D node. Developers may reset the camera, and calculate the elevation from bounding box. The infinite or null bounding box means the scene has no geometries and only adjust camera's elevation when it's finite.
*   Aspose.ThreeD.UpVector class has been renamed to Aspose.ThreeD.Axis class.
*   Aspose.ThreeD.Render.DriverException class is added - The exceptions of the internal renderer are wrapped as DriverException.
*   Aspose.ThreeD.Render.InitializationException class is added - This exception is thrown while failing to initialize the renderer, for example to initialize it on a computer that has no hardware support of OpenGL 4.0.
*   Aspose.ThreeD.Render.Renderer class is added - It creates a Renderer object and render window from the window's native handle. Right now, we only support native window handle from Microsoft Windows. We have plans to support more platforms in the future. The CreateRenderer method of Renderer class creates a hardware OpenGL-backend renderer and some internal initializations will be done. When the renderer goes out of the scope, the unmanaged hardware resources will also be disposed.
*   Aspose.ThreeD.Render.Viewport class has been added - Aspose.3D API supports three types of viewports. Since the renderer target any viewport of these types.
*   Aspose.ThreeD.Render.IRenderTarget/IRenderTexture/IRenderWindow classes are added.
    *   IRenderTarget is the base interface of IRenderTexture/IRenderWindow.
    *   IRenderTexture allows to render the scene to one or more textures (textures are located in video memory and can be transferred to system memory).
    *   IRenderWindow allows to render the scene to window in real-time.
*   Aspose.ThreeD.Render.ITextureUnit and Aspose.ThreeD.Render.TextureType classes are added - ITextureUnit is actually the texture sampler in GPU side and the texture data in CPU or GPU memory.
*   Aspose.ThreeD.Render.PostProcessing class has been added - PostProcessing class allows developers to apply real-time image processing filter to the rendered image. In this version, we have provided 4 built-in post-processing effects. We'll allow developers to have their own custom post-processing algorithm in the future version.
*   Aspose.ThreeD.Render.RenderFactory class is added - It helps in rendering a scene to textures or window in real-time.
*   Aspose.ThreeD.Render.RenderParameters class is added - It defines the parameters about how to create the render target like color bits, depth bits, stencil bits, double buffering.
*   AddData methods are added to Aspose.ThreeD.Entities.VertexElementUV class -The VertexElementUV's base class has been changed from VertexElementTemplate<Vector2> to VertexElementTemplate<Vector4>, it will only store Vector4 since 2.0.0, so two helper methods were added to allow user to add a list of Vector2 and Vector3 to VertexElementUV, it will internally expand the Vector2/Vector3 to Vector4 and leave the rest fields zero.
*   Aspose.ThreeD.FileFormat class is changed - The FileFormat properties are changed from integer to System.Version.
*   GetBoundingBox method is added to Aspose.ThreeD.Node class - It allows developers to get the axis-aligned bounding box.

We have also improved the rendering on 64-bit operating systems.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][2]
*   [Download Aspose.3D for .NET][3]
*   [Aspose.3D product family forum][4] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   Aspose.3D for .NET online documentation – help documentation and API reference documents.
*   [Enable Blog Subscription][5] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Migrate from Earlier Versions of Aspose.3D API – We keep track of Aspose.3D API change version by version. So we recommend to get help from this section while upgrading to the latest API version or if Aspose.3D API code is broken at some stage.

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/3d/net
[2]: http://www.aspose.com/.net/3d-component.aspx
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.3d-for-.net/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.3d-product-family/535/showforum.aspx
[5]: https://blog.aspose.com/
[6]: https://github.com/aspose3D/Aspose_3d_NET




