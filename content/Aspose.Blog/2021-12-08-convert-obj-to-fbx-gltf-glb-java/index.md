---
title: 'Convert OBJ File to FBX or glTF GLB File in Java'
seoTitle: "Convert OBJ File to FBX or glTF GLB File Programmatically in Java"
description: "Convert OBJ File to FBX or glTF GLB File Programmatically using Java. Export or change 3D Object Files with high fidelity."
date: Wed, 08 Dec 2021 19:50:00 +0000
draft: false
url: /2021/12/08/convert-obj-to-fbx-gltf-glb-java/
author: Farhan Raza
summary: '3D Object OBJ files contain 3D objects information like the texture and coordinates. You can convert an OBJ file to a GLTF or FBX file programmatically in Java. In some scenarios, you might need to convert an OBJ file to different files. In accordance with that, this article covers **how to convert an OBJ file to GLTF or FBX file in Java.**'
tags: ['Convert OBJ to FBX', 'OBJ File to GLB in Java', 'OBJ file to FBX', 'OBJ file to FBX in Java', 'OBJ to glTF']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/OBJ-to-FBX-glTF-GLB.jpg" alt="OBJ to glTF FBX">}}


3D Object [OBJ][1] files contain 3D objects information like the texture and coordinates. You can **convert** **an** **OBJ file to a [GLTF][2] or [FBX][3]** file programmatically in Java. In some scenarios, you might need to convert an OBJ file to different files. In accordance with that, this article covers how to convert an OBJ file to GLTF or FBX file.

*   [Java API to Convert OBJ to glTF GLB or FBX File][4]
*   [Convert OBJ to glTF GLB File Programmatically in Java][5]
*   [Convert OBJ to FBX File in Java][6]

## Java API to Convert OBJ to glTF GLB or FBX File

[Aspose.3D for Java][7] API supports manipulating 3D Object files like converting them to glTF GLB or FBX files. API. You can install the API by downloading the JAR file from the [New Releases][8] section or with the following Maven configurations in pom.xml file of your project:

### Repository```
 <repositories>
    <repository>
        <id>AsposeJavaAPI</id>
        <name>Aspose Java API</name>
        <url>http://repository.aspose.com/repo/</url>
    </repository>
</repositories>
```

### Dependency```
 <dependencies>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-3d</artifactId>
        <version>21.12</version>
    </dependency>
</dependencies>
```

## Convert OBJ to glTF GLB File Programmatically in Java

You can convert an OBJ file to a glTF file in Java by following the steps below:

1.  Load the input OBJ file with the [Scene][9] constructor.
2.  Initialize a [GltfSaveOptions][10] class object.
3.  Save the output glTF GLB document.

The code snippet below demonstrates how to convert an OBJ file to glTF document in Java:

{{< gist aspose-com-gists 959a1d627af6c8f8b9fd80cd9306b407 "Convert-OBJ-to-glTF-GLB.java" >}}

## Convert OBJ to FBX File in Java

You can convert an OBJ file to an FBX file with the following steps:

1.  Load the input object OBJ file using the [Scene][11] class constructor.
2.  Initialize an object of [FbxSaveOptions][12] class.
3.  Save the output FBX file using the [Save][13] method.

The following code snippet shows how to convert an OBJ file to an FBX file programmatically using Java:

{{< gist aspose-com-gists 959a1d627af6c8f8b9fd80cd9306b407 "Convert-OBJ-to-FBX.java" >}}

## Conclusion

In this article, you have learned how to convert an OBJ object file to a glTF GLB or FBX file programmatically in Java. Moreover, you may take visit the [API Reference][14] or the [documentation][15] to learn other features offered by the API.  In case of any concerns, please feel free to contact us at the [forum][16].

## See Also

[Convert FBX to RVM or RVM to FBX File in Java][17]




[1]: https://docs.fileformat.com/3d/obj/
[2]: https://docs.fileformat.com/3d/gltf/
[3]: https://docs.fileformat.com/3d/fbx/
[4]: #section1
[5]: #section2
[6]: #section3
[7]: https://products.aspose.com/3d/java
[8]: https://downloads.aspose.com/3d/java
[9]: https://apireference.aspose.com/3d/java/com.aspose.threed/Scene
[10]: https://apireference.aspose.com/3d/java/com.aspose.threed/GltfSaveOptions
[11]: https://apireference.aspose.com/3d/java/com.aspose.threed/Scene
[12]: https://apireference.aspose.com/3d/java/com.aspose.threed/FBXSaveOptions
[13]: https://apireference.aspose.com/3d/java/com.aspose.threed/Scene#save-java.lang.String-com.aspose.threed.FileFormat-
[14]: https://apireference.aspose.com/3d/java
[15]: https://docs.aspose.com/3d/java/
[16]: https://forum.aspose.com/c/3d
[17]: https://blog.aspose.com/2021/11/19/convert-fbx-to-rvm-or-rvm-to-fbx-file-in-java/




