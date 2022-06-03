---
title: 'Convert DWG to OBJ in Java'
date: Thu, 31 Mar 2022 10:04:00 +0000
draft: false
url: /2022/03/31/convert-dwg-to-obj-java/
author: ''Farhan Raza''
summary: 'DWG files contain vector images as well as metadata so that any off-book information is not needed to comprehend the drawings. Such drawings are used by engineers, architects, or town planners to create huge designs. In certain situations, you might require to convert a DWG file to an OBJ 3D Object format file. According to such use cases, this article covers how to **convert a DWG file to an OBJ file programmatically in Java**.'
tags: ['DWG Drawing to OBJ Object', 'DWG to OBJ in Java', 'Java DWG to OBJ']
categories: ['Aspose.CAD Product Family']
---



{{< figure align=center src="images/DWG-to-OBJ-1.jpeg" alt="DWG to OBJ Java">}}


[DWG][1] files contain vector images as well as metadata so that any off-book information is not needed to comprehend the drawings. Such drawings are used by engineers, architects, or town planners to create huge designs. In certain situations, you might require to convert a DWG file to an [OBJ][2] 3D Object format file. According to such use cases, this article covers how to convert a DWG file to an OBJ file programmatically in Java.

*   [DWG to OBJ Converter –  Java API Installation][3]
*   [Convert DWG to OBJ File Programmatically in Java][4]

## DWG to OBJ Converter – Java API Installation {#section1}

[Aspose.CAD for Java][5] API supports working with different [file formats][6] including DWG, IGES, and PLT files. You can configure the API by downloading its JAR file from the [Downloads][7] or specify the following configurations under the pom.xml file to install it from [Aspose Repository][8]:

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
        <artifactId>aspose-cad</artifactId>
        <version>22.1</version>        
   </dependency>
</dependencies>
```

## Convert DWG to OBJ File Programmatically in Java {#section2}

You need to follow the steps below to convert a DWG file to OBJ format:

1.  Create an object of the [Image][9] class to load the source DWG file.
2.  Type-cast formerly declared object to [CadImage][10] class.
3.  Export the DWG file to OBJ format with the [Save][11] method.

The code snippet below demonstrates how to convert DWG to OBJ file programmatically in Java:



## Explore More Features

You may visit the [documentation][12] space to explore working with different CAD image formats. It covers working with different AutoCAD drawings in your projects.

## Conclusion

In this article, you have learned the steps and the sample code snippet to convert DWG drawings to 3D Object files in OBJ format. Moreover, this article also explains the simple configuration details which do not require any other UI application. Please feel free to reach out to us at the [forum][13] for discussing any of your requirements or concerns.

## See Also

[Convert DWG to FBX in Java][14]




[1]: https://docs.fileformat.com/cad/dwg/
[2]: https://docs.fileformat.com/3d/obj/
[3]: #section1
[4]: #section2
[5]: https://products.aspose.com/cad/java
[6]: https://docs.aspose.com/cad/java/supported-file-formats/
[7]: https://downloads.aspose.com/cad/java
[8]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-cad
[9]: https://apireference.aspose.com/cad/java/com.aspose.cad/Image
[10]: https://apireference.aspose.com/cad/java/com.aspose.cad.fileformats.cad/CadImage
[11]: https://apireference.aspose.com/cad/java/com.aspose.cad/Image#save-java.lang.String-com.aspose.cad.ImageOptionsBase-
[12]: https://docs.aspose.com/cad/net/
[13]: https://forum.aspose.com/c/cad
[14]: https://blog.aspose.com/2022/02/14/convert-dwg-to-fbx-java/




