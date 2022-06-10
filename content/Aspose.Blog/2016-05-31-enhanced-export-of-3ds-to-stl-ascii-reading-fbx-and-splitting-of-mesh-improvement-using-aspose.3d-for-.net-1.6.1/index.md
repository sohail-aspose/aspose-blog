---
title: 'Enhanced Export of 3DS to STL ASCII, Reading FBX and Splitting of Mesh Improvement using Aspose.3D for .NET 1.6.1'
date: Tue, 31 May 2016 15:49:06 +0000
draft: false
url: /2016/05/31/enhanced-export-of-3ds-to-stl-ascii-reading-fbx-and-splitting-of-mesh-improvement-using-aspose.3d-for-.net-1.6.1/
author: Imran Rafique
summary: ''
tags: ['3D API', 'Convert 3DS to STL ASCII', 'Export FBX', 'Import FBX', 'Splitting of Mesh']
categories: ['Aspose.3D Product Family']
---

[![Aspose.3D for NET APIs][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2015/10/Aspose.3d-for-net-100x100.png)

[](https://blog.aspose.com/wp-content/uploads/sites/2/2015/10/Aspose.3d-for-net-100x100.png)We’re pleased to announce the availability of new version 1.6.1 of Aspose.3D for .NET API. In this new version, the way of converting 3DS files to STL ASCII has been improved. The common 3D software packages can now easily import the resulting STL ASCII files. Previously, the opening of STL ASCII files in 3D Builder was displaying a loading error in most of the use cases. Similarly, the import of FBX and splitting the Mesh features have also been improved internally. We still have more to do in improving appearance of meshes. In reference to this, our product team is working hard to bring more features and enhancements in the upcoming versions.

## Import of the FBX Files

Based on the client's feedback, we noticed, the FBX import was crashing due to the complex internal structure of meshes. It was specific to the FBX sample. The FBX importer now handles this more gracefully. We recommend our clients upgrade to this newer version from their old version to get this enhancement.

## Split the Mesh of an Existing 3D File

In the previous version 1.5.0, we have added features to split the mesh in several ways in order to split more complex meshes. The SplitMesh method of the PolygonModifier class was always throwing a stack overflow error for any existing 3D file. We have incorporated this bug fix in the latest version 1.6.1.

We have also fixed the bugs of complex FBX files caused by the obfuscation. Please check a list of the resolved defects:

*   Fixed: PolygonModifier.SplitMesh method throws a stack overflow exception for the scene.
    
*   Fixed: 3DS to STL ASCII export - can't load an STL ASCII file in 3D Builder.
    
*   Fixed: NullReferenceException occurs while loading the FBX file.
    

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

# _convert 3d files_




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/10/Aspose.3d-for-net-100x100.png "Aspose.3d- for-net-100x100"
[2]: http://www.aspose.com/.net/3d-component.aspx
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.3d-for-.net/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.3d-product-family/535/showforum.aspx
[5]: https://blog.aspose.com/ "Aspose.3D for .NET Blog Subscription"
[6]: https://github.com/aspose3D/Aspose_3d_NET




