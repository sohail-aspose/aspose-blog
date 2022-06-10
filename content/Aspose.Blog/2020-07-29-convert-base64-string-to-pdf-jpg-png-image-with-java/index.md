---
title: 'Convert Base64 String to PDF or JPG/PNG Image with Java'
seoTitle: "Java Convert Base64 String to PDF or JPG/PNG Images"
description: "Convert Base64 string to PDF or image like JPG, PNG in Java. Convert Base64 string in HTML page to image to view Base64 image and string example."
date: Wed, 29 Jul 2020 16:40:17 +0000
draft: false
url: /2020/07/29/convert-base64-string-to-pdf-jpg-png-image-with-java/
author: Farhan Raza
summary: ''
tags: ['base64 converter', 'base64 string', 'base64 to image', 'base64 to pdf', 'base64 to png', 'convert base64 string', 'convert base64 to image']
categories: ['Aspose.PDF Product Family']
---

[Base64][1] string shows data in [ASCII][2] format. It is popular for embedding inline images and other information in HTML webpages or style sheets. In this article, we will be learning **how to convert the Base64 string to [PDF][3], [JPG][4] and [PNG][5] using Java**.

## Java Base64 to PDF Converter API - Installation

You can download the JAR files of [Aspose.PDF for Java][6] API from [Releases][7] section, or using following Maven configurations:

### **Repository**```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository
```

### **Dependency**```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>20.7</version>
</dependency>
```

So Aspose.PDF for Java API has been configured. Before proceeding for the conversion of a Base64 string, let us take a look at sample data:

## Example String for Base64 Conversion

You can download the Base64 string from [here][8].

### Preview of the Base64 Example String



{{< figure align=center src="images/Base64-to-JPG-PNG.png" alt="Base64 to PNG JPG">}}


Now, let us proceed to the following Base64 string conversion scenarios:

*   [Convert Base64 String to JPG or PNG Image using Java][9]
*   [Convert Base64 String to PDF File using Java][10]

## Convert Base64 String to JPG or PNG Image using Java {#section1}

JPG, PNG, and other kinds of images are sometimes encoded to Base64 string for safe and reliable communication and transfer of data. Moreover, before we explore PDF conversion, we need to learn about the conversion of a Base64 string to JPG or PNG images using Java. Therefore, you need to follow these steps for the conversion:

1.  Save the data in a TXT file because of a long string
2.  Read the string value
3.  Replace the prefixes
4.  Save Base64 string to JPG or PNG Image

The following code snippet shows how to convert Base64 string to a JPG or PNG image using Java:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Base64-to-PNG-JPG-Images.java" >}}

## Convert Base64 to PDF using Java {#section2}

We have learned about converting the Base64 to PNG or JPG images. This is actually an intermediate step of converting Base64 to PDF file. Let us move another step further. Once the string is saved as a raster image, you can easily convert it to PDF. You can follow below steps for converting Base64 string to PDF:

1.  Remove prefixes of Base64 String
2.  Convert Base64 string to PNG or JPG image
3.  Then convert output image to PDF

So the code snippet below shows how to convert Base64 String to PDF using Java language:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Base64-to-PDF.java" >}}

## Conclusion

To sum up, we have explored how to convert the Base64 string to PDF, PNG, and JPG images. using Java Moreover, generating a PDF file will open up a lot more options for further conversion. Like a PDF file can be converted to SVG, XPS, DOCX, and many other formats. Interested to explore other possibilities? Do not hesitate to discuss this with us via Free Support Forums.

## See Also

[Convert JPG, PNG, TIFF, EMF, or BMP Images to PDF using C#][11]




[1]: https://en.wikipedia.org/wiki/Base64
[2]: https://en.wikipedia.org/wiki/ASCII
[3]: https://docs.fileformat.com/pdf/
[4]: https://docs.fileformat.com/image/jpeg/
[5]: https://docs.fileformat.com/image/png/
[6]: https://products.aspose.com/pdf/java
[7]: https://releases.aspose.com/
[8]: https://drive.google.com/file/d/11VZNcha6TPTGvSEWklUTOXcKGTqGLPhd/view?usp=sharing
[9]: #section1
[10]: #section2
[11]: https://blog.aspose.com/2020/07/26/images-to-pdf-csharp/





