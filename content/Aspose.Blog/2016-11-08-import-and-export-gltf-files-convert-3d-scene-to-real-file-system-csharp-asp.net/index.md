---
title: 'Import or Export 3D Scenes from/to glTF Files using C# .NET'
date: Tue, 08 Nov 2016 12:26:58 +0000
draft: false
url: /2016/11/08/import-and-export-gltf-files-convert-3d-scene-to-real-file-system-csharp-asp.net/
author: Imran Rafique
summary: ''
tags: ['3D scene Dependencies', 'Convert 3D files to glTF', 'Convert glTF', 'Export glTF', 'Import glTF']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for NET APIs">}}


We are pleased to announce the availability of [new version 16.11.0 of Aspose.3D for .NET API][1]. The new version adds support of GL Transmission Format (glTF). Developers can import glTF files into the Aspose.3D API, and then export them in any supported 3D format. Developers can also save all dependencies of a 3D scene in the real file system. The GL Transmission Format (glTF) is an efficient, extensible, interoperable format for the transmission and loading of 3D content. Developers can install Aspose.3D Nuget package in their .NET applications because we publish each version as [a NuGet package on the NuGet gallery][2]. We recommend our clients upgrade the old version of the Aspose.3D API to this latest one. For details on API fixes, please check [Release Notes][3] having a complete list of the features, enhancements and bug fixes.

## Import and Export 3D Scenes from/to glTF in C#

Using Aspose.3D API, developers can now convert any supported 3D file to glTF format, and vice versa. The GL Transmission Format (glTF) is a runtime asset delivery format for GL APIs. Being an open standard, it fills a real and growing need to bring 3D assets quickly and efficiently to a wide variety of platforms and devices. Please check these help topics to set load and save glTF settings: [Use of the glTF Load Options][4] and [Use of the glTF Save Options][5]

## Export Dependencies of a 3D Scene to Real File System

Aspose.3D API allows developers to retrieve all dependency files from a 3D model, and then write them in the real file system or simply discard. There are three ways to save dependency files as define a path of the local directory, save in the MemoryFileSystem class object and simply discard saving dependencies. The FileSystem property is added to all save option classes. These articles show how developers can save dependencies of a 3D scene: [Save Dependencies in the Local Directory][6], [Save Dependencies in the MemoryFileSystem Object][7] and [Discard Saving the Material Files][8].

## Public API Changes

The following API changes in the new version are also worth noting:

*   Aspose.ThreeD.Formats.GLTFLoadOptions class has been added. It helps in importing glTF files into Aspose.3D API.
*   Aspose.ThreeD.Formats.GLTFSaveOptions class has been added. It helps in saving a glTF file.
*   GLTF and GLTF\_Binary format entries have been added in the Aspose.ThreeD.FileFormat class for loading and saving purposes.
*   An Extension property has been added in the FileFormatType class to get the extension name of the file format.
*   Aspose.ThreeD.Utilities.DummyFileSystem class has been added. It helps to discard saving the dependency files of a 3D scene.
*   Aspose.ThreeD.Utilities.LocalFileSystem class has been added. It helps to save dependency in the Local directory.
*   Aspose.ThreeD.Utilities.MemoryFileSystem class has been added. It helps to save the dependency file in the MemoryFileSystem class object.
*   The AddEntity method has been added in the Aspose.ThreeD.Node class. It gives a shortcut way of adding an entity to a node.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][9]
*   [Download Aspose.3D for .NET][10]
*   [Aspose.3D product family forum][11] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][12] – help documentation and API reference documents.
*   [Enable Blog Subscription][13] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][14] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [Migrate from Earlier Versions of Aspose.3D API][15] – We keep track of Aspose.3D API change version by version. So we recommend getting help from this section while upgrading to the latest API version or if Aspose.3D API code is broken at some stage.




[1]: http://downloads.aspose.com/3d/net/new-releases/aspose.3d-for-.net-16.11.0/
[2]: https://www.nuget.org/packages/Aspose.3d
[3]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+16.11.0+Release+Notes
[4]: https://docs.aspose.com/display/3dnet/Specify+3D+File+Load+Options#Specify3DFileLoadOptions-UseoftheglTFLoadOptions
[5]: https://docs.aspose.com/display/3dnet/Specify+3D+File+Save+Options#Specify3DFileSaveOptions-UseoftheglTFSaveOptions
[6]: https://docs.aspose.com/display/3dnet/Specify+3D+File+Save+Options#Specify3DFileSaveOptions-SaveDependenciesintheLocalDirectory
[7]: https://docs.aspose.com/display/3dnet/Specify+3D+File+Save+Options#Specify3DFileSaveOptions-SaveDependenciesintheMemoryFileSystemObject
[8]: https://docs.aspose.com/display/3dnet/Specify+3D+File+Save+Options#Specify3DFileSaveOptions-DiscardSavingtheMaterialFiles
[9]: http://products.aspose.com/3d/net
[10]: http://downloads.aspose.com/3d/net
[11]: http://forum.aspose.com
[12]: http://docs.aspose.com/display/3dnet/Home
[13]: https://blog.aspose.com/category/aspose-products/aspose-3d-product-family
[14]: https://github.com/aspose3D/Aspose_3d_NET
[15]: https://docs.aspose.com/display/3dnet/Migrating+from+Earlier+Versions+of+Aspose.3D




