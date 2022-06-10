---
title: 'Key Updates and Bug Fixes in Aspose.3D for .NET and Java 19.12'
date: Thu, 19 Dec 2019 18:03:27 +0000
draft: false
url: /2019/12/19/net-java-3d-api-to-create-manipulate-3d-files/
author: Usman Aziz
summary: ''
tags: ['.NET', '3D animation', 'API', 'Aspose.3D API', 'Java 3D API', 'java']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/aspose_3d-brand.png" alt="XPS Document Manipulation API for C++">}}


Hello everyone! Its time to talk about the latest version of [**Aspose.3D**][1] we have recently released. Aspose.3D product family offers .NET and Java 3D modeling APIs to view, read, convert and alter the 3D files without requiring any modeling software. Since there could be a variety of files as well as contents they contain, some of the files may behave unexpectedly and produce the bugs. We have addressed such issues in [**v19.12**][2] of Aspose.3D for .NET and Java APIs. Also, we have made some important updates in the animation system and the renderer. So in this article, I am going to give you an overview of major changes in the API as well as the bug fixes.

## Major Updates in Aspose.3D v19.12

We have done the following changes in v19.12 of Aspose.3D for .NET and Java APIs.

*   The animation system has been refactored and we have renamed classes **Curve** and **CurveMapping** to **KeyframeSequence** and **BindPoint** respectively.
*   The legacy OpenGL renderer has been removed and the renderer has been refactored. Now, it would work best with the underlying Vulkan driver. The low-level interfaces have also been updated while high-level rendering interfaces remain intact.
    *   The refactored renderer provides a better rendering performance with more flexibility and extensibility.
    *   The render method in the **Scene** class is not changed and there is no need for changes when using a high-level rendering interface.
    *   The low-level API has undergone a breaking change. Please contact [support][3] for details about the migration.
*   All the obsolete methods and properties will be removed in v20.03.

For a complete list of obsolete members in classes and their replacements, please have a look at the release notes.

*   [Aspose.3D for .NET 19.12 release notes][4]
*   [Aspose.3D for Java 19.12 release notes][5]

## Bug Fixes

The following issues that were found in the previous versions have been fixed in the latest release.

*   Part of the scene gets lost when converting [RVM][6] to [GLB][7].
*   The problem when loading the 3D files.
*   The shadow is created when a scene is merged.

You can download the latest source code examples from the [GitHub repository][8] and evaluate the API features. Have a look at the [documentation][9] of the API for more details about every feature of the API. In case you would find it difficult to migrate to the latest version, please feel free to contact us via our [forum][10].




[1]: https://products.aspose.com/3d
[2]: https://downloads.aspose.com/3d
[3]: https://forum.aspose.com/c/3d
[4]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+19.12+Release+Notes
[5]: https://docs.aspose.com/display/3djava/Aspose.3D+for+Java+19.12+Release+Notes
[6]: https://docs.fileformat.com/3d/rvm/
[7]: https://docs.fileformat.com/3d/glb/
[8]: https://github.com/aspose-3d
[9]: https://docs.aspose.com/display/3dproductfamily/Home
[10]: https://forum.aspose.com/c/3d




