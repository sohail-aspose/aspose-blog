---
title: 'Convert OBJ to FBX File in Java'
seoTitle: "Convert OBJ to FBX File Programmatically in Java"
description: "Convert OBJ 3D Object File to FBX programmatically in Java. You can export OBJ file to different formats of FBX file FBX7500ASCII, FBX7500ASCII etc."
date: Sat, 16 Oct 2021 07:45:00 +0000
draft: false
url: /2021/10/16/convert-obj-to-fbx-java/
author: Farhan Raza
summary: 'OBJ files are used to create, edit, or manipulate 3D objects. In certain situations, you may need to convert an OBJ file to an FBX file in Java. This article covers how to **convert a 3D object file to an FBX file programmatically using Java**.'
tags: ['Convert OBJ to FBX', 'Convert OBJ to FBX using Java']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Convert-OBJ-to-FBX-Java.jpg" alt="Convert OBJ to FBX in Java">}}


[OBJ][1] files are used to create, edit, or manipulate 3D objects. In certain situations, you may need to **convert** **an** **OBJ file to an **[**FBX**][2] file in Java. This article covers how to convert a 3D object file to an FBX file programmatically using Java.

*   [OBJ to FBX Converter – 3D API Installation][3]
*   [Convert OBJ to FBX File in Java][4]

## OBJ to FBX File Converter – API Installation {#section1}

You can create, edit, or convert 3D objects with [Aspose.3D for Java][5] API. You can quickly install the API by downloading the JAR file from the [New Releases][6] section or with the following Maven configurations in pom.xml file of your project.

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
        <version>22.1</version>
    </dependency>
</dependencies>
```

## Convert OBJ to FBX File in Java {#section2}

You can easily convert OBJ to FBX with a few API calls. The API itself takes care of the output file format while performing the conversion so that you can focus on other important tasks related to your application. Please follow the steps below for converting a 3D object OBJ file to an FBX file:

1.  Load the input OBJ file using the [Scene][7] class.
2.  Initialize an object of [FbxSaveOptions][8] class.
3.  Save output FBX file with the [save][9] method.

The code sample below explains how to convert an OBJ file to an FBX file programmatically in Java:

{{< gist aspose-com-gists fe3a72e93e954cb0200ef625e7af2bf0 "Convert-OBJ-to-FBX.java" >}}

## Explore API Features

You can take a look at several other features of the API by visiting the [documentation][10]. It covers different properties and method calls to work with [supported file formats][11].

## Conclusion

In conclusion, you have learned how to convert an OBJ file to an FBX file programmatically using Java. You may also like to visit the API References for a detailed look at different classes. Furthermore, please feel free to contact us via the [forum][12] in case of any inquiries.

## See Also

[Convert DAE to OBJ File in Java][13]




[1]: https://docs.fileformat.com/3d/obj/
[2]: https://docs.fileformat.com/3d/fbx/
[3]: #section1
[4]: #section2
[5]: https://products.aspose.com/3d/java
[6]: https://downloads.aspose.com/3d/java
[7]: https://apireference.aspose.com/3d/java/com.aspose.threed/scene
[8]: https://apireference.aspose.com/3d/java/com.aspose.threed/FbxSaveOptions
[9]: https://apireference.aspose.com/3d/java/com.aspose.threed/Scene#save-com.aspose.threed.Stream-com.aspose.threed.FileFormat-
[10]: https://docs.aspose.com/3d/java/
[11]: https://docs.aspose.com/3d/java/supported-file-formats/
[12]: https://forum.aspose.com/c/3d
[13]: https://blog.aspose.com/2021/12/15/convert-dae-to-obj-java/




