---
title: 'Work with 3D Files in .NET Standard 2.0 and Java'
date: Mon, 22 Oct 2018 20:23:08 +0000
draft: false
url: /2018/10/22/work-with-3d-files-in-.net-standard-2.0-and-java-3d-modeling-api/
author: Farhan Raza
summary: ''
tags: []
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for .NET logo">}}


We are honored to announce the October release of Aspose.3D API. This release includes the long-awaited feature of Support for .NET Standard 2.0 (.NET Core) Framework. Several other performance-related enhancements have also been incorporated in this release. You can use the following links to download Aspose.3D for .NET and Java APIs.

*   [Aspose.3D for .NET 18.10][1]
*   [Aspose.3D for Java 18.10][2]

## Control File Compression {#title-heading}

Aspose.3D API provides you even better control over your applications. We have added EnableCompression property to FBXSaveOptions class, which allows you to decide if you want to enable or disable file compression while saving FBX file. You can use this property as follows:

**C#**

```
Scene scene = new Scene("test.fbx");
scene.Save("test.fbx", new FBXSaveOptions(FileFormat.FBX7500ASCII) {EnableCompression = false});
```

Few other exceptions pertaining to huge FBX file have also been rectified.  Please visit [Release Notes (Java)][3] or [Release Notes (.NET)][4] for further information about this release. In case you have any question about Aspose.3D API, you can post your inquiry in [Aspose.3D forums][5]. We will be more than happy to assist you there.

## Aspose.3D for .NET and Java Resources

The following resources will help you work with Aspose.3D for .NET and Java APIs:

*   [Home page for Aspose.3D API][6].
*   [Aspose.3D API wiki docs][7]\- Help documentation and API reference documents.
*   [Aspose.3D product family forum][8]\- Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   [Enable email subscription][9]\- Do not limit yourself, stay up-to-date with the latest news about the Aspose.3D APIs and new features, fixes, plus other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][10]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.3D for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Release Notes ([.NET][12] and [Java][13] – For details on API fixes, please check Release Notes having a complete list of the new features.




[1]: https://www.nuget.org/packages/Aspose.3D/18.10.0
[2]: https://artifact.aspose.com/repo/com/aspose/aspose-3d/18.10/
[3]: https://docs.aspose.com/display/3djava/Aspose.3D+for+Java+18.10+-+October+2018
[4]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+18.10+-+October+2018
[5]: https://forum.aspose.com/c/3d
[6]: http://www.aspose.com/products/3d
[7]: https://docs.aspose.com/display/3Dproductfamily/Home
[8]: https://forum.aspose.com/c/3d
[9]: https://blog.aspose.com/category/aspose-products/aspose-3d-product-family/
[10]: https://github.com/aspose3d/Aspose_3D_NET
[11]: https://github.com/aspose-3d/Aspose.3D-for-Java
[12]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+18.10+-+October+2018
[13]: https://docs.aspose.com/display/3djava/Aspose.3D+for+Java+18.10+-+October+2018)




