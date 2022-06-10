---
title: 'Convert 3D Files to Google Draco Format with Compressions Options in C# .NET'
date: Thu, 13 Apr 2017 16:21:45 +0000
draft: false
url: /2017/04/13/convert-3d-meshes-google-draco-format-zoom-camera-orthographic-projection-using-aspose.3d-.net-17.4.0/
author: Imran Rafique
summary: ''
tags: ['Convert 3D files to Google Darco', 'Google Draco', 'Magnify 3D View', 'Orthographic Projection', 'Set compression level in Google Darco']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for NET APIs">}}


We are pleased to announce the availability of a new version, 17.4.0, of [Aspose.3D for .NET][1] API. The new version of the API adds support of **converting 3D models to the Google Draco (.drc)** format. You can import any supported 3D file, and then export it in DRC format. All 3D import formats are listed on this page: [Import an Existing 3D File][2]. The Draco saving options of the API also allow specifying the compression level. The following topic shows how to specify save options for Google Darco files: 

*   [Use of the Google Draco (.drc) Save Options][3]SaveOptions)

## Retrieve Mesh of a 3D Shape to Encode in Google Draco File

3D meshes are widely used in computer graphics applications for approximating 3D models. When representing complex shapes in raw data format, meshes consume a large amount of space. Using Aspose.3D for .NET API, developers can retrieve a mesh of any 3D shape, and then encode it in the Google Draco (.drc) file. This help topic will help to know the way of encoding a mesh in DRC file: [Encoding a 3D Mesh in the Google Draco File][4]

## Improved Camera Movement and Magnification Support

Using Aspose.3D for .NET API, developers can already place a camera in 3D scene to define a view as narrated in this help topic: [Take a Picture of 3D Model from the Camera][5]. Developers can now find improvements in the Camera and Light movements with orthographic projection mode. There are two rotation modes as below:

*   **FixedTarget** mode is compatible with old code in real-time rendering. The orientation of the Frustum (base class of Camera and Light) is specified by its LookAt property which is an absolute position in the world space, in this mode developers can always get different Direction property when its position gets changed.
*   **FixedDirection** mode is useful in designing tools like CAD or FPS games. It will no longer look at a target, but keep the same direction (specified by its Direction property) relative to its position. In this mode, developers can always get different LookAt property when its position gets changed.

Developers can also zoom out the camera to quickly magnify the view. The following source code demonstrates how to set the rotation and magnification of a Camera object:

```
// initialize a Camera object
Camera camera = new Camera();
// set the rotation mode
camera.RotationMode = RotationMode.FixedDirection;
// Gets or sets the magnification used in orthographic camera
camera.Magnification = new Vector2(2, 2); 
```

## Public API Changes

The following API changes in the new version are also worth noting:

*   DracoCompressionLevel Enum has been added. It helps in defining a compression level before saving a 3D model in the Google Draco (.drc) format.
*   DracoSaveOptions class has been added. It helps to apply settings before saving a 3D model in the Google Draco (.drc) format.
*   DracoFormat class has been added. It helps to encode the mesh of 3D shape to Draco mesh (raw data).
*   RotationMode member is added to Aspose.ThreeD.Entities.Frustum (Base class of Camera and Light) Class. It helps in the Camera and Light movement.
*   Magnification member is added to Aspose.ThreeD.Entities.Camera Class. It helps in magnifying a view.

Aspose.3D can be installed via the NuGet package in the .NET applications because we publish each version as [a NuGet package on the NuGet gallery][6]. We recommend our clients upgrade an older version of the Aspose.3D API to the latest one. For details on API fixes, please check [Release Notes][7] having a complete list of the features, enhancements and bug fixes.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspos][8][e][9][.3D for .NET API][10]
*   [Download Aspose.3D for .NET][11]
*   [Aspose.3D product family forum][12] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   Aspose.3D for .NET online documentation – help documentation and API reference documents.
*   [Enable Blog Subscription][13] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][14] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you will enjoy this new release that saves time and effort. The API is quite simple and developers can use it in application easily.




[1]: https://downloads.aspose.com/3d/net/
[2]: https://docs.aspose.com/display/3dnet/Create+and+Read+an+Existing+3D+Scene
[3]: https://docs.aspose.com/display/3dnet/Specify+3D+File+Save+Options#Specify3DFileSaveOptions-UseoftheGoogleDraco(.drc
[4]: https://docs.aspose.com/display/3dnet
[5]: https://docs.aspose.com/display/3dnet/Render+3D+View+in+Image+format+from+Camera#Render3DViewinImageformatfromCamera-TakeaPictureof3DModelfromtheCamera
[6]: https://www.nuget.org/packages/Aspose.3d
[7]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+17.4.0+Release+Notes
[8]: http://www.aspose.com/products/3d/net
[9]: http://products.aspose.com/3d/net
[10]: http://www.aspose.com/products/3d/net
[11]: http://downloads.aspose.com/3d/net
[12]: http://www.aspose.com/community/forums/aspose.3d-product-family/535/showforum.aspx
[13]: https://blog.aspose.com/category/aspose-products/aspose-3d-product-family
[14]: https://github.com/aspose3D/Aspose_3d_NET




