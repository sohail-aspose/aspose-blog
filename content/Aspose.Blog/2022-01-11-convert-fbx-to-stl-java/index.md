---
title: 'Convert FBX to STL in Java'
date: Tue, 11 Jan 2022 20:04:00 +0000
draft: false
url: /2022/01/11/convert-fbx-to-stl-java/
author: ''Farhan Raza''
summary: 'in certain cases, you might want to convert an FBX file to STL format. Accordingly, this article covers **how to convert FBX to STL programmatically using Java.**'
tags: ['Convert FBX to STL', 'Convert FBX to STL in java', 'FBX to STL', 'Java convert FBX to STL']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/FBX-to-STL-1.jpg" alt="Convert FBX to STL Java">}}


[FBX][1] files are used by a number of data modeling and content creation applications. You may need specific applications or tools to work with the FBX format. However, in certain cases, you might want to convert an FBX file to STL format. Accordingly, this article covers how to convert FBX to STL programmatically using Java.

*   [FBX to STL Converter – Java API Installation][2]
*   [Convert FBX to STL File Programmatically in Java][3]

## FBX to STL Converter – Java API Installation {#section1}

[Aspose.3D for Java][4] API supports working with FBX, STL, as well as other 3D file formats. You can download the JAR files from the [Downloads][5] section or use the [Aspose Repository][6] configurations mentioned below, in the pom.xml file of your project.

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
        <version>22.2</version>
    </dependency>
</dependencies>
```

## Convert FBX to STL File Programmatically in Java {#section2}

You need to follow the steps below to convert an FBX file to STL format:

1.  Load the source FBX document using an instance of the [Scene][7] class.
2.  Create an instance of [StlSaveOptions][8] class.
3.  Write the output STL file with the [Save][9] method.

The code snippet below demonstrates how to convert an FBX file to STL format programmatically using Java:



## Explore Other Features

You may go through the [documentation][10] to explore many other features offered by the API.

## Online Demo

Please try the [FBX to STL Converter][11] web app developed using the above API.

## Conclusion

In conclusion, you have understood how to convert FBX files to STL programmatically using Java. The API takes care of all the minor details for the conversion so that you only need to make a few methods calls to achieve the requirements. Furthermore, please feel free to contact us at the [forum][12] in case of any inquiries.

## See Also

[Convert DAE to OBJ File in Java][13]




[1]: https://docs.fileformat.com/3d/fbx/
[2]: #section1
[3]: #section2
[4]: https://products.aspose.com/3d/java
[5]: https://downloads.aspose.com/3d/java
[6]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-3d
[7]: https://apireference.aspose.com/3d/java/com.aspose.threed/scene
[8]: https://apireference.aspose.com/3d/java/com.aspose.threed/StlSaveOptions
[9]: https://apireference.aspose.com/3d/java/com.aspose.threed/Scene#save-java.lang.String-com.aspose.threed.FileFormat-
[10]: https://docs.aspose.com/3d/java/
[11]: https://products.aspose.app/3d/conversion/fbx-to-stl
[12]: https://forum.aspose.com/c/3d
[13]: https://blog.aspose.com/2021/12/15/convert-dae-to-obj-java/




