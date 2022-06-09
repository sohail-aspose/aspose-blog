---
title: 'Find and Replace Text in Word Documents using Java'
seoTitle: ""
description: ""
date: Tue, 16 Jun 2020 01:47:54 +0000
draft: false
url: /2020/06/16/find-and-replace-text-in-word-doc-docx-using-java/
author: Usman Aziz
summary: ''
tags: ['find and replace text in DOCX using Java', 'find and replace text in word document']
categories: ['Aspose.Words Product Family']
---

In this article, I'll demonstrate **how to find and replace text in Word** (DOC/DOCX) documents programmatically using Java. The step by step guide and code samples will cover various scenarios of finding and replacing text in Word documents.



{{< figure align=center src="images/C-Find-and-Replace-Text.png" alt="Find and replace text in Word documents">}}


MS Word provides an easy way to **find and replace text** in the documents. One of the popular use cases of finding and replacing text could be removing or replacing sensitive information within the documents before they are shared among various entities. However, the manual process may require you to install MS Word and update every document separately. In such situations, it would be handy and time-saving especially when you have integrated find and replace features within your desktop or web application. So let's begin and see how to **find and replace text in Word documents using Java** in various scenarios.

*   [Find and Replace Text in Word DOC/DOCX using Java][1]
*   [Replace Similar Words based on Regex Pattern in Word DOC/DOCX][2]
*   [Find and Replace Text in the Header/Footer of Word Document][3]
*   [Find and Replace Text with Meta-Characters in Word DOC/DOCX][4]

## Java API to Find and Replace Text in Word Documents

In order to implement the find and replace feature, we'll use [Aspose.Words for Java][5] which is a powerful, feature-rich, and easy to use Word processing API for Java platform. You can either [download][6] its JAR or install it within your Maven-based application using the following configurations.

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-words</artifactId>
    <version>20.5</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Find and Replace Text in Word Documents (DOC/DOCX) using Java {#Find-and-Replace-Text-in-Word-DOC/DOCX-using-Java}

Let's start by addressing a simple find and replace scenario where we will find the word "Sad" within the input Word document. The following are the steps to perform this operation.

*   Create an instance of [Document][7] class and pass to it the Word document's path.
*   Find and replace text using [Document.getRange.replace(String, String, FindReplaceOptions)][8] method.
*   Save the document using [Document.save(String)][9] method.

The following code sample shows how to find and replace text in Word DOCX documents using Java.

{{< gist aspose-com-gists 2eba8d1b1d2802076cd1252d49ebdf16 "find-replace-text-in-Word.java" >}}

Below is the input Word document that we have used in this article.



{{< figure align=center src="images/Word-Document.png" alt="find and replace text in DOCX using Java">}}


The following is the output after finding and replacing the word "sad".



{{< figure align=center src="images/Find-And-Replace-Text-In-Document.png" alt="find and replace a word">}}


## Find and Replace Similar Words in Word DOC/DOCX using Java {#Find-and-Replace-Similar-Words-in-Word-Documents}

You can also customize the API to find and replace text based on the similarity. For example, the words "sad", "mad" and "bad" are following a similar pattern that ends on "ad". Email IDs are another example of such a text. In such cases, you can define a regex pattern to find and replace all the text occurrences having a particular pattern. The following are the steps to achieve this.

*   Create an instance of [Document][10] class and pass to it the Word document's path.
*   Define a regex pattern using _Pattern.compile()_ method and pass it to [Document.getRange().replace(Pattern pattern, String replacement, FindReplaceOptions options)][11] method.
*   Save the updated document using [Document.save(String)][12] method.

The following code sample shows how to find and replace similar words based on a particular pattern using Java.

{{< gist aspose-com-gists 2eba8d1b1d2802076cd1252d49ebdf16 "find-replace-similar-words.java" >}}

The following is the screenshot of the Word document after updating similar words.



{{< figure align=center src="images/Find-And-Replace-Multiple-Word-In-Document.png" alt="find and replace similar words using Java">}}


## Replace Text in the Header/Footer of Word Document {#Find-and-Replace-Text-in-the-Header/Footer-of-Word-Document}

Aspose.Words also allows you to find and replace text only in the header/footer of the Word document. The following are the steps to perform this operation.

*   Create an instance of [Document][13] class and pass to it the Word document's path.
*   Get [HeaderFooterCollection][14] of the document using [Document.getFirstSection().getHeadersFooters()][15] method.
*   Retrieve the particular header/footer in the [HeaderFooter][16] object.
*   Use [HeaderFooter.getRange().replace()][17] method to find and replace text.
*   Save the updated Word document.

The following code sample shows how to find and replace text in the header/footer of Word document using Java.

{{< gist aspose-com-gists 2eba8d1b1d2802076cd1252d49ebdf16 "find-replace-text-footer.java" >}}

The following screenshot shows the updated text in the footer of the Word document.



{{< figure align=center src="images/Find-And-Replace-Text-In-Footer.png" alt="find and replace text in footer">}}


## Find and Replace Text with Meta-Characters in Word DOCX using Java {#Find-and-Replace-Text-with-Meta-Characters-in-Word-DOC/DOCX}

There could be the case when you need to find and replace a phrase that is divided into multiple lines or paragraphs. In such cases, you will have to take care of the paragraph, section, or line breaks. Aspose.Words for Java makes it simple for you to handle such cases quite easily. The following are the meta-characters that you can use for different breaks:

*   **&p**: paragraph break
*   **&b**: section break
*   **&m**: page break 
*   **&l**: line break

The following code sample demonstrates how to find and replace the text with a paragraph break in a Word document.

{{< gist aspose-com-gists 2eba8d1b1d2802076cd1252d49ebdf16 "find-replace-text-metachars.java" >}}

The following is the screenshot of the output Word document.



{{< figure align=center src="images/Find-And-Replace-Text-with-Paragraph-Break.png" alt="find and replace text with meta characters">}}


## Conclusion

In this article, you have seen how to find and replace text in Word DOC/DOCX documents programmatically using Java. Various scenarios of finding and replacing text in MS Word DOCX files have been addressed with the help of code samples. You can learn more about Aspose.Words for Java from the [documentation][18].

## See Also

*   [Find and Replace Text in Word Documents using C#][19]




[1]: #Find-and-Replace-Text-in-Word-DOC/DOCX-using-Java
[2]: #Find-and-Replace-Similar-Words-in-Word-Documents
[3]: #Find-and-Replace-Text-in-the-Header/Footer-of-Word-Document
[4]: #Find-and-Replace-Text-with-Meta-Characters-in-Word-DOC/DOCX
[5]: https://products.aspose.com/words/java
[6]: https://downloads.aspose.com/words/java
[7]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[8]: https://apireference.aspose.com/words/java/com.aspose.words/range#replace(java.lang.String,java.lang.String)
[9]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[10]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[11]: https://apireference.aspose.com/words/java/com.aspose.words/range#replace(java.util.regex.Pattern,java.lang.String,com.aspose.words.FindReplaceOptions)
[12]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[13]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[14]: https://apireference.aspose.com/words/java/com.aspose.words/HeaderFooterCollection
[15]: https://apireference.aspose.com/words/java/com.aspose.words/section#HeadersFooters
[16]: https://apireference.aspose.com/words/java/com.aspose.words/HeaderFooter
[17]: https://apireference.aspose.com/words/java/com.aspose.words/range#replace(java.lang.String,java.lang.String,com.aspose.words.FindReplaceOptions)
[18]: https://docs.aspose.com/display/wordsjava/Find+and+Replace
[19]: https://blog.aspose.com/2020/01/24/find-and-replace-text-in-word-documents-in-csharp-net/





