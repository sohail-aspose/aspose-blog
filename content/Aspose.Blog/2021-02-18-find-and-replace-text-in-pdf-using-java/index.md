---
title: 'Find and Replace Text in PDF using Java'
seoTitle: "Java: Find and Replace Text in PDF | Search and Replace Text with Regex"
description: "Use Java PDF API to find and replace text in PDF files using Java. Replace text in a particular page or all pages in PDF using regular expressions in Java."
date: Thu, 18 Feb 2021 09:51:08 +0000
draft: false
url: /2021/02/18/find-and-replace-text-in-pdf-using-java/
author: Usman Aziz
summary: 'In various cases, you may need to find and replace a particular piece of text in the PDF document. However, finding and updating each occurrence manually may cost you extra time and effort. For such cases, the find and replace option makes your life easier. In this article, you will learn how to automate the feature of finding and replacing text in PDF documents using Java.'
tags: ['Find and Replace Text in PDF using Java', 'Java API to Find and Replace Text in PDF', 'Replace Text on a Particular Page in PDF Java', 'Replace Text using Regular Expression in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Find-and-Replace-Text-in-PDF.jpg" alt="Find and replace text in PDF Java">}}


In various cases, you may need to find and replace a particular piece of text in the [PDF][1] documents. However, searching and updating each occurrence manually may cost you extra time and effort. For such cases, the find and replace option makes your life easier. In this article, you will learn **how to find and replace text in PDF documents using [Java][2]**.

*   [Java API to Find and Replace Text in PDF][3]
*   [Find and Replace Text in PDF using Java][4]
*   [Replace Text on a Particular Page in PDF][5]
*   [Replace Text using Regular Expression][6]

## Java API to Find and Replace Text in PDF - Free Download {#Java-API-to-Find-and-Replace-Text-in-PDF}

[Aspose.PDF for Java][7] is designed for generating and manipulating PDF files from within the Java applications. The API provides a wide range of basic as well as advanced PDF manipulation features including finding and replacing text. You can either [download][8] the API or install it using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>21.1</version>    
</dependency>
```

## Find and Replace Text in PDF using Java {#Find-and-Replace-Text-in-PDF-using-Java}

In order to replace a particular text in PDF, you would first get all the text fragments matching the search string. Once you have them, simply replace each fragment with updated text one by one.

The following are the steps to find and replace text in a PDF file using Java.

*   Load the PDF file using [Document][9] class.
*   Create an object of [TextFragmentAbsorber][10] class and initialize it with the text you want to find and replace.
*   Accept the absorber for the pages in PDF using [Document.getPages().accept(TextFragmentAbsorber)][11] method.
*   Get all the occurrences of the text returned by [TextFragmentAbsorber.getTextFragments()][12] into a [TextFragmentCollection][13] object.
*   Loop through each [TextFragment][14] in the [TextFragmentCollection][15] object and replace the text using [TextFragment.setText(String)][16] method.
*   Save the updated PDF file using [Document.save(String)][17] method.

The following code sample shows how to find and replace text in PDF.

{{< gist aspose-com-gists 52502af0613b9151b22c72979727dfa2 "find-replace-text-pdf.java" >}}

## Search and Replace Text on a Particular Page in PDF {#Replace-Text-on-a-Particular-Page-in-PDF}

Instead of finding and replacing text in the whole PDF, you can specify a single page on which you want to replace the text occurrences. In this case, you will accept the [TextFragmentAbsorber][18] for a particular page only by specifying the page index.

The following are the steps to search and replace text on a particular page in PDF in Java.

*   Load the PDF file using [Document][19] class.
*   Create an object of [TextFragmentAbsorber][20] class and initialize it with the text you want to find and replace.
*   Accept the absorber for a particular page in PDF using [Document.getPages().get\_Item(Int pageIndex).accept(TextFragmentAbsorber)][21] method.
*   Get all the occurrences of the text returned by [TextFragmentAbsorber.getTextFragments()][22] into [TextFragmentCollection][23] object.
*   Loop through each [TextFragment][24] in the [TextFragmentCollection][25] object and replace the text using [TextFragment.setText(String)][26] method.
*   Save the updated PDF file using [Document.save(String)][27] method.

The following code sample shows how to find and replace text on a particular page in PDF using Java.

{{< gist aspose-com-gists 52502af0613b9151b22c72979727dfa2 "find-replace-text-pdf-page.java" >}}

## Find and Replace Text using Regular Expressions in PDF {#Replace-Text-using-Regular-Expression}

You can also specify a regular expression to search the text that matches a particular pattern such as emails, SSNs, etc. The following are the steps to define and use a regular expression to search and replace text in PDF using Java.

*   Load the PDF file using [Document][28] class.
*   Create an object of [TextFragmentAbsorber][29] class and initialize it with the regular expression you want to use.
*   Create an object of [TextSearchOptions][30] class and initialize it with _true_ to enable the regular expression-based search.
*   Set options using [TextFragmentAbsorber.setTextSearchOptions(TextSearchOptions)][31] method.
*   Accept the absorber for the pages in PDF using [Document.getPages().accept(TextFragmentAbsorber)][32] method.
*   Get all the found occurrences of the text returned by [TextFragmentAbsorber.getTextFragments()][33] into [TextFragmentCollection][34] object.
*   Loop through each [TextFragment][35] in the [TextFragmentCollection][36] object and replace the text using [TextFragment.setText(String)][37] method.
*   Save the updated PDF file using [Document.save(String)][38] method.

The following code sample shows how to find and replace text in PDF using regular expression.

{{< gist aspose-com-gists 52502af0613b9151b22c72979727dfa2 "find-replace-text-pdf-regex.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try the API without evaluation limitations for free. [Get a free temporary license][39] now.

## Conclusion

In this article, you have learned how to find and replace text in PDF using Java. Furthermore, you have seen how to use a regular expression to search and replace text following a particular pattern. You can explore more about the Java PDF API using [documentation][40].

## See Also

*   [Create PDF Files using Java][41]
*   [Split a PDF Files using Java][42]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/programming/java/
[3]: #Java-API-to-Find-and-Replace-Text-in-PDF
[4]: #Find-and-Replace-Text-in-PDF-using-Java
[5]: #Replace-Text-on-a-Particular-Page-in-PDF
[6]: #Replace-Text-using-Regular-Expression
[7]: https://products.aspose.com/pdf/java
[8]: https://downloads.aspose.com/pdf/java
[9]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentAbsorber
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PageCollection#accept-com.aspose.pdf.TextFragmentAbsorber-
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentAbsorber#getTextFragments--
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentCollection
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentCollection
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment#setText-java.lang.String-
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentAbsorber
[19]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[20]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentAbsorber
[21]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Page#accept-com.aspose.pdf.TextFragmentAbsorber-
[22]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentAbsorber#getTextFragments--
[23]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentCollection
[24]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment
[25]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentCollection
[26]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment#setText-java.lang.String-
[27]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[28]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[29]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentAbsorber
[30]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextSearchOptions
[31]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentAbsorber#setTextSearchOptions-com.aspose.pdf.TextSearchOptions-
[32]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PageCollection#accept-com.aspose.pdf.TextFragmentAbsorber-
[33]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentAbsorber#getTextFragments--
[34]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentCollection
[35]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment
[36]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentCollection
[37]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment#setText-java.lang.String-
[38]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[39]: https://purchase.aspose.com/temporary-license
[40]: https://docs.aspose.com/pdf/java/
[41]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/
[42]: https://blog.aspose.com/2021/01/15/Split-PDF-Files-using-Java/





