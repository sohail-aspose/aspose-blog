---
title: 'Convert EPS or PS PostScript File to an SVG Image using Java'
seoTitle: "Convert EPS or PS PostScript File to an SVG Image | Scalable Vector"
description: "Convert EPS or PS Postscript file to SVG Scalable Vector Graphics image. Export EPS Page Description Language file to SVG in Java."
date: Wed, 29 Sep 2021 11:25:34 +0000
draft: false
url: /2021/09/29/convert-eps-or-ps-postscript-to-svg/
author: Farhan Raza
summary: 'EPS or PS PostScript files are based on page description language that can contain different artifacts like Text, Images, Drawings, etc. You can convert an EPS or PS Postscript file to an SVG image (Scalable Vector Graphic) as per your requirements. Please refer to the following headings for more information.'
tags: ['Convert EPS to SVG', 'EPS to SVG', 'EPS to SVG in Java', 'PS to SVG', 'PostScript to SVG']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/Convert-EPS-PS-to-SVG.png" alt="Convert EPS PS to SVG">}}


EPS or PS PostScript files are based on page description language that can contain different artifacts like Text, Images, Drawings, etc. You can convert an [EPS][1] or [PS][2] Postscript file to an [SVG][3] image (Scalable Vector Graphic) as per your requirements. Please refer to the following headings for more information:

*   [EPS or PS PostScript File to SVG Image Converter – Java API Configuration][4]
*   [Convert EPS or PS PostScript File to an SVG Image with Java][5]

## EPS or PS PostScript File to SVG Image Converter – Java API Configuration {#section1}

EPS or PS PostScript file to SVG image conversion is a two-step process. First, you need to convert the input EPS/PS file to a PDF document with [Aspose.Page for Java][6]. Then render the PDF file to an SVG image with [Aspose.PDF for Java][7]. Please download the JAR files from the [New Releases][8] section, or use the following configurations in the pom.xml file of your Maven-based project:

### Repository```
 <repositories>
     <repository>
         <id>snapshots</id>
         <name>repo</name>
         <url>http://repository.aspose.com/repo/</url>
     </repository>

</repositories>
```

### Dependency```
 <dependencies>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-page</artifactId>
        <version>21.8</version>
    </dependency>

    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-pdf</artifactId>
        <version>21.9</version>
    </dependency>

</dependencies>
```

## Convert EPS or PS PostScript File to an SVG Image with Java {#section2}

You can convert an EPS or PS PostScript File to an SVG image with the below steps:

1.  Initialize [ByteArrayOutputStream][9] to hold intermediary file.
2.  Initialize EPS or PS PostScript input stream.
3.  Declare [PsDocument][10] class object.
4.  Initialize [PdfSaveOptions][11] object with necessary parameters.
5.  Convert EPS or PS Postscript file to PDF with the [save][12] method.
6.  Load the PDF file and convert the EPS or PS PostScript file to an SVG file.

The following code shows how to convert an EPS or PS PostScript file to an SVG (Scalable Vector Graphic) image file with Java:

{{< gist aspose-com-gists babc9d668d2de044ae835145ea6bc86e "EPS-to-SVG.java" >}}

## Get Free Evaluation License

There are some evaluation limitations for the APIs, which you can avoid by requesting a [Free Temporary License][13] and test the APIs in full capacity.

## Conclusion

In this article, you have learned how to convert an EPS or PS PostScript file to an SVG image using Java. You have explored the simple and easy steps for the conversion. Moreover, please explore the [Documentation][14] for further information about the APIs, and feel free to contact us at the [Free Support Forum][15] to discuss any of your concerns.

## See Also

[Convert OXPS or XPS to PDF Programmatically with Java][16]




[1]: https://docs.fileformat.com/page-description-language/eps/
[2]: https://docs.fileformat.com/page-description-language/ps/
[3]: https://docs.fileformat.com/page-description-language/svg/
[4]: #section1
[5]: #section2
[6]: https://products.aspose.com/page/java/
[7]: https://products.aspose.com/pdf/java/
[8]: https://releases.aspose.com/
[9]: https://docs.oracle.com/javase/7/docs/api/java/io/ByteArrayOutputStream.html
[10]: https://apireference.aspose.com/page/java/com.aspose.eps/PsDocument
[11]: https://apireference.aspose.com/page/java/com.aspose.eps.device/PdfSaveOptions
[12]: https://apireference.aspose.com/page/java/com.aspose.eps/PsDocument#save-com.aspose.page.Device-com.aspose.page.SaveOptions-
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2021/02/09/convert-oxps-xps-pdf-java/




