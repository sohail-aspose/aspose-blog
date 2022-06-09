---
title: 'Convert Markdown to HTML or HTML to MD File in Java'
seoTitle: "Convert MD to HTML or HTML Webpage to Markdown File in Java"
description: "Convert Markdown MD to HTML Webpage Programmatically using Java. Convert or Export HTML webpage to File in Java applications."
date: Tue, 23 Nov 2021 06:25:00 +0000
draft: false
url: /2021/11/23/convert-md-html-java/
author: Farhan Raza
summary: 'Markdown is used to create formatted text with plain text symbols. You can easily format text as bold, italic, underline, and other formatting types. You can **convert Markdown MD to HTML as well as HTML to Markdown programmatically in Java**. The following sections explain these conversion scenarios.'
tags: ['HTML to MD', 'HTML to MD in Java', 'HTML to Markdown', 'MD to HTML', 'MD to HTML in Java', 'Markdown to HTML']
categories: ['Aspose.HTML Product Family']
---



{{< figure align=center src="images/Convert-HTML-Markdown.png" alt="Convert MD HTML Java">}}


[Markdown][1] is used to create formatted text with plain text symbols. You can easily format text as bold, italic, underline, and other formatting types. You can **convert Markdown MD to [HTML][2] as well as HTML to Markdown** programmatically in Java. The following sections explain these conversion scenarios.

*   [HTML and Markdown Converter – API Installation][3]
*   [Convert HTML Webpage to Markdown Programmatically in Java][4]
*   [Convert Markdown to HTML Webpage Programmatically in Java][5]

## HTML and Markdown Converter – API Installation {#section1}

You can convert the HTML webpage to a Markdown file using Java. You can configure [Aspose.HTML for Java][6] API by downloading the JAR file from the [Downloads][7] section or using the following Maven configurations in your project.

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
        <artifactId>aspose-html</artifactId>
        <version>21.6</version>
        <classifier>jdk16</classifier>
    </dependency>
</dependencies>
```

## Convert HTML Webpage to Markdown MD Programmatically in Java {#section2}

You can convert HTML Webpage to Markdown text with the following steps.

1.  Load the input HTML file.
2.  Specify [MarkdownSaveOptions][8] object.
3.  Call [ConvertHTML][9] method and save output Markdown .md file.

The code snippet below shows how to convert HTML Webpage to Markdown .md in Java:

{{< gist aspose-com-gists c709fbcda21b373ca9c96a3711a6767a "Convert-HTML-to-Markdown.java" >}}

## Convert Markdown .md File to HTML Webpage Programmatically in Java {#section3}

You can convert a Markdown .md file to HTML webpage with the following steps:

1.  Load the input Markdown file.
2.  Save output HTML file with [ConvertMarkdown][10] method.

The following code snippet explains how to convert a Markdown file to HTML Webpage in Java:

{{< gist aspose-com-gists c709fbcda21b373ca9c96a3711a6767a "Convert-Markdown-to-HTML.java" >}}

## Conclusion

In this article, you have learned how to convert Markdown files to HTML or HTML webpage to Markdown programmatically in Java. Moreover, you can learn other features of the API by visiting the [documentation][11]. In case of any concerns, please feel free to contact us at the [forum][12].

## See Also

[Convert (MD) Markdown to PDF or Image in Java][13]




[1]: https://docs.fileformat.com/word-processing/md/
[2]: https://docs.fileformat.com/web/html/
[3]: #section1
[4]: #section2
[5]: #section3
[6]: https://products.aspose.com/html/java
[7]: https://downloads.aspose.com/html/java
[8]: https://apireference.aspose.com/html/java/com.aspose.html.saving/MarkdownSaveOptions
[9]: https://apireference.aspose.com/html/java/com.aspose.html.converters/Converter#convertHTML-com.aspose.HTMLDocument-com.aspose.saving.ImageSaveOptions-java.util.Collection-
[10]: https://apireference.aspose.com/html/java/com.aspose.html.converters/Converter#convertMarkdown-java.io.InputStream-java.lang.String-
[11]: https://docs.aspose.com/html/java/
[12]: https://forum.aspose.com/c/html
[13]: https://blog.aspose.com/2021/01/23/convert-md-to-pdf-image-java/




