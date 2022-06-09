---
title: 'Add or Remove Header and Footer in Word Documents using Java'
seoTitle: ""
description: ""
date: Tue, 01 Sep 2020 18:17:04 +0000
draft: false
url: /2020/09/01/add-remove-header-footer-in-word-java/
author: Farhan Raza
summary: 'Header and Footer are commonly used in documents to show important information like page number, topic, chapter, etc. You can add, insert, delete or remove header and footer in Word documents (DOCX/DOC) using your Java applications. In this article, we will be learning about adding or removing headers and footers.'
tags: ['add footer in docx', 'add footer in word', 'add header footer in word', 'add header in docx', 'add header in word', 'footer in word', 'header in word', 'remove header footer in word']
categories: ['Aspose.Words Product Family']
---

Header and Footer are commonly used in documents to show important information like page number, topic, chapter, etc. You can add, insert, delete or remove header and footer in Word documents ([DOCX][1]/[DOC][2] using your Java applications. In this article, we will be learning about adding or removing headers and footers. Following are the topics that we will be exploring in detail:

*   [Insert or Remove Header and Footer API – Installation][3]
*   [Add Header and Footer in Word Document (DOCX/DOC) using Java][4]
*   [Delete Header and Footer of Word Document (DOCX/DOC) using Java][5]
*   [Remove Footer from Word Document (DOCX/DOC) using Java][6]
*   [Remove Header from Word Document (DOCX/DOC) using Java][7]

## Insert or Remove Header Footer API – Installation {#section1}

For working with Header and Footer in Word documents, we will be using [Aspose.Words for Java][8] API where simple API calls will help us achieve the requirements. You can download the JAR file from the [releases section][9], or copy the following Maven configurations in your project. The API will be configured via the Maven repository and you will be good to proceed with further steps explained in this article.

### Repository```
<repositories>
    <repository>
        <id>AsposeJavaAPI</id>
        <name>Aspose Java API</name>
        <url>https://repository.aspose.com/repo/</url>
    </repository>
</repositories>
```

### Dependency```
<dependencies>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-words</artifactId>
        <version>20.8</version>
        <classifier>jdk17</classifier>
    </dependency>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-words</artifactId>
        <version>20.8</version>
        <classifier>javadoc</classifier>
    </dependency>
</dependencies>
```

## Add Header and Footer in Word Document (DOCX/DOC) using Java {#section2}

Adding header and footer in Word documents (DOCX/DOC) is a basic yet important use case of working with word processing documents. However, different scenarios are possible. For example, you might need to add an image, a table, or only some text in the header and footer section. Moreover, sometimes the header and footer are different on the title page as compared to other pages. Sometimes the header and footer are different on even page numbers and different on odd page numbers. Therefore, we have created a concise and basic example of adding header and footer in Word documents.

Here we will insert different header footer on the title page (very first page), and different header footer on the subsequent page. Whereas, the second page will have a custom header footer including image, text, and table element. You need to follow the steps below for adding or inserting header and footer in word documents (DOCX/DOC) using Java.

1.  Initialize [Document][10] and [DocumentBuilder][11] class objects
2.  Specify that you want different header footer for the title page
3.  Set font properties for header text
4.  Create header and for subsequent pages
5.  Insert table and set the page number format
6.  Save output DOCX file

The following code is based on these steps which show how to add header and footer in Word documents (DOCX/DOC) programmatically using Java:

{{< gist aspose-com-gists 427e825b740939e9fd80524baa056f1c "AddHeaderFooter.java" >}}

So far we have learned how to add or insert header and footer in word files. Below is a screenshot of how the output looks when you see it via Print Preview option.

This feature can help a lot when different DOC/DOCX documents are processed by your applications where you want to add some content as header footer of output documents.



{{< figure align=center src="images/Add-Remove-Header-Footer.png" alt="Add or Remove Header Footer">}}


Let us proceed to check out deleting the header and footer from MS Word files (DOCX/DOC).

## Delete Header and Footer of Word Document (DOCX/DOC) using Java {#section3}

You can delete the header as well as footer of word documents using Aspose.Words for Java API. As discussed above, there could be three different types of header and footer added in a document. For instance, on title page, on even pages, and odd page numbers. You can delete all headers and footers in a word file simply by following the steps below:

1.  Load source DOCX/DOC file
2.  Find header and footer on the title page, even page numbers, and odd page numbers
3.  Delete the required section when found
4.  Save output DOCX file

The code below follows these steps and shows how to delete header and footer in word documents using Java:

{{< gist aspose-com-gists 427e825b740939e9fd80524baa056f1c "RemoveHeaderFooter.java" >}}

## Remove Footer from Word Document (DOCX/DOC) using Java {#section4}

We have already discussed how to remove or delete header and footer from word files. However, you may want to remove only the footers of a Word document while leaving the Header intact. These requirements are easily possible with the following steps:

1.  Load source word file (DOCX/DOC)
2.  Iterate through each Section of the word document
3.  Initialize [HeaderFooter][12] object
4.  Delete footer from the input file
5.  Save updated DOCX/DOC file

The following code snippet explains how to remove footer from word document using Java:

{{< gist aspose-com-gists 427e825b740939e9fd80524baa056f1c "RemoveFooter.java" >}}

## Remove Header from Word Document (DOCX/DOC) using Java {#section5}

Since we have learned removing or deleting only the footer from MS Word files. Let us explore this another step further where you might need to remove only the headers from Word documents. The footers will remain the same and unaffected because our focus here is deleting the headers only. The following steps provide an outline of the procedure to be adopted for this purpose:

1.  Load input Word file (DOCX/DOC)
2.  Initialize an instance of [HeaderFooter][13] class
3.  Remove Headers from all section of the input document
4.  Save update DOCX file

Below code shows how to delete or remove the header from word documents using Java:

{{< gist aspose-com-gists 427e825b740939e9fd80524baa056f1c "RemoveHeader.java" >}}

## Conclusion

Add, Insert, Remove or Delete Header and Footer in Word documents is a very important and frequent use case of word processing. Almost all documents contain Headers and Footers, which can be manipulated with Aspose.Words for Java API as per your requirements. This article is an overview of related features where you can discuss any custom use case and requirements with us via [Free Support Forums][14]. Feel free to reach out to us for any queries and concerns.

## See Also

[Word Document (DOC/DOCX) to HTML Conversion][15]




[1]: https://docs.fileformat.com/word-processing/docx/
[2]: https://docs.fileformat.com/word-processing/doc/)
[3]: #section1
[4]: #section2
[5]: #section3
[6]: #section4
[7]: #section5
[8]: https://products.aspose.com/words/java
[9]: https://releases.aspose.com/
[10]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[11]: https://apireference.aspose.com/words/java/com.aspose.words/DocumentBuilder
[12]: https://apireference.aspose.com/words/java/com.aspose.words/HeaderFooter
[13]: https://apireference.aspose.com/words/java/com.aspose.words/HeaderFooter
[14]: https://forum.aspose.com/c/words
[15]: https://blog.aspose.com/2020/07/15/word-document-doc-docx-to-html-conversion-using-java/





