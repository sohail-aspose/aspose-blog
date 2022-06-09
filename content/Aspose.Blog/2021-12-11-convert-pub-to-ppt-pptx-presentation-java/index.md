---
title: 'Convert PUB to PPT or PPTX in Java'
seoTitle: "Convert PUB to PPT or PPTX Presentation in Java"
description: "Convert Microsoft Publisher PUB file to PPT or PPTX Presentation in Java. Export PUB to PPT/PPTX file programmatically using Java."
date: Sat, 11 Dec 2021 10:25:00 +0000
draft: false
url: /2021/12/11/convert-pub-to-ppt-pptx-presentation-java/
author: Farhan Raza
summary: 'Microsoft Publisher files are usually used to design and create documents for publishing on large scale. In some scenarios, you might need to convert PUB to PPT or PPTX Presentation file. In accordance with that, the article describes how to **convert a Publisher PUB file to a PPT or PPTX Presentation file in Java**.'
tags: ['Convert PUB to Presentation', 'PUB to PPT', 'PUB to PPTX']
categories: ['Aspose.PUB Product Family']
---



{{< figure align=center src="images/PUB-to-PPTX-1.png" alt="PUB to PPTX in Java">}}


Microsoft Publisher files are usually used to design and create documents for publishing on large scale. In some scenarios, you might need to convert [PUB][1] to [PPT][2] or [PPTX][3] Presentation file. In accordance with that, the article describes how to convert a Publisher PUB file to a PPT or PPTX Presentation file in Java.

*   [Java API to Convert PUB file to Presentation][4]
*   [Convert PUB to PPT/PPTX Presentation File Programmatically in Java][5]

## Java API to Convert PUB file to PPT/PPTX Presentation {#section1}

You will convert a PUB file to a PowerPoint Presentation as PPT or PPTX file in two steps. Firstly, you need to convert a PUB file to PDF using [Aspose.PUB for Java][6] API. Then you need to convert the intermediate PDF file to a Presentation file with [Aspose.PDF for Java][7] API. You can get the JAR files from the [New Releases][8] section, or specify the following configurations in the pom.xml file of your Maven-based projects:

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
        <artifactId>aspose-pub</artifactId>
        <version>20.8</version>
    </dependency>

    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-pdf</artifactId>
        <version>21.8</version>
    </dependency>
</dependencies>
```

## Convert PUB to PPT/PPTX Presentation File Programmatically in Java {#section2}

You can convert a Microsoft Publisher PUB file to a Presentation file in PPT or PPTX format with the steps below:

1.  Initialize [ByteArrayOutputStream][9] to hold intermediate PDF file.
2.  Initialize [Pub Parser][10] for the PUB file.
3.  [Parse][11] the input Publisher file.
4.  Convert PUB to PDF file and save output into the stream.
5.  Load the intermediate PDF file using the [Document][12] class object.
6.  Save the output PPT or PPTX file.

The following code snippet shows how to convert a PUB file to a PPT or PPTX PowerPoint Presentation programmatically in Java:



## Try Online Demo

Please try the [PUB to PPTX][13] web app developed using this API.

## Get Free API License

You can evaluate the Aspose APIs without any limitations by requesting a [free temporary license][14].

## Conclusion

In this article, you have learned how to convert or export Microsoft Publisher PUB file to a Presentation file as PPT or PPTX file programmatically in Java. You can embed this feature in your Java-based applications. Moreover, you can explore several other features offered by Aspose APIs by visiting the [documentation][15]. In case of any concerns, please feel free to reach out to us at the [forum][16].

## See Also

[Convert PUB to HTML Webpage File with Java][17]




[1]: https://docs.fileformat.com/publisher/pub/
[2]: https://docs.fileformat.com/presentation/ppt/
[3]: https://docs.fileformat.com/presentation/pptx/
[4]: #section1
[5]: #section2
[6]: https://products.aspose.com/pub/java/
[7]: https://products.aspose.com/pdf/java/
[8]: https://releases.aspose.com/
[9]: https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/io/ByteArrayOutputStream.html
[10]: https://apireference.aspose.com/pub/java/com.aspose.pub.class-use/IPubParser
[11]: https://apireference.aspose.com/pub/java/com.aspose.pub/IPubParser#parse--
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[13]: https://products.aspose.app/pub/conversion/pub-to-pptx
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/pub/java/
[16]: https://forum.aspose.com/c/pub
[17]: https://blog.aspose.com/2021/09/24/convert-pub-to-html-webpage/




