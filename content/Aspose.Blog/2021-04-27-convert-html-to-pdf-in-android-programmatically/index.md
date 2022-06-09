---
title: 'Convert HTML to PDF in Android Programmatically'
seoTitle: "HTML to PDF in Android Programmatically | Android Converter Library"
description: "Use Android HTML to PDF converter library to convert HTML files to PDF in Android apps programmatically. Convert HTML to password-protected PDF."
date: Tue, 27 Apr 2021 21:00:05 +0000
draft: false
url: /2021/04/27/convert-html-to-pdf-in-android-programmatically/
author: Usman Aziz
summary: 'In various cases, you may need to convert the HTML pages to PDF format. On the other hand, you may want to generate PDF from the content of a WYSIWYG HTML editor. For such scenarios, this article covers **how to convert HTML to PDF in Android apps programmatically**. Furthermore, you will learn about additional options to customize HTML to PDF conversion.'
tags: ['Android HTML to PDF Conversion using URL', 'Android HTML to PDF Converter Library', 'Convert HTML to PDF Android', 'Convert HTML to Password-protected PDF in Android']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/HTML-to-PDF-Java.png" alt="HTML to PDF Android Java">}}


In various cases, you may need to convert the [HTML][1] pages to [PDF][2] format. On the other hand, you may want to generate PDF from the content of a WYSIWYG HTML editor. For such scenarios, this article covers **how to convert HTML to PDF in Android apps programmatically**. Furthermore, you will learn about additional options to customize HTML to PDF conversion.

*   [Android HTML to PDF Converter Library][3]
*   [Convert HTML to PDF][4]
*   [Convert HTML to Password-protected PDF][5]
*   [HTML to PDF Conversion using URL][6]
*   [Get a Free Licence][7]

## Android HTML to PDF Converter Library {#Android-HTML-to-PDF-Converter-Library}

In order to convert HTML to PDF, we'll use [Aspose.PDF for Android via Java][8] library. It provides a complete set of features to create, modify or convert PDF files programmatically from within your Android apps. You can either [download][9] the library files or install them using the following configurations.

```
maven {
    url "http://repository.aspose.com/repo/" }
```
```
compile (
        group: 'com.aspose',
        name: 'aspose-pdf',
        version: '20.11',
        classifier: 'android.via.java')
```

## Convert HTML to PDF in Android Programmatically {#HTML-to-PDF-in-Android-Programmatically}

The following are the steps to convert HTML to PDF in Android programmatically.

*   Create an object of the [HtmlLoadOptions][10] class.
*   Create an object of [Document][11] class and initialize it with the HTML file’s path and _HtmlLoadOptions_ object.
*   Save HTML as PDF using [Document.save(String)][12] method.

The following code sample shows how to convert an HTML file to PDF.

{{< gist aspose-com-gists c6fe5ccefe38a5ec03d983307eb0e850 "convert-html-to-pdf.java" >}}

### HTML File



{{< figure align=center src="images/HTML-Document.png" alt="HTML to PDF Android">}}


### HTML to PDF



{{< figure align=center src="images/HTML-to-PDF.png" alt="Android HTML to PDF Converter Library">}}


## Convert HTML to Password-protected PDF {#Convert-HTML-to-Password-protected-PDF}

You can also convert HTML to a password-protect PDF within a few lines of code. The following are the steps to perform this operation.

*   Create an object of the [HtmlLoadOptions][13] class.
*   Create an object of the [Document][14] class and initialize it with the HTML file’s path and _HtmlLoadOptions_ object.
*   Use [Document.encrypt(String, String, Permissions, CryptoAlgorithm)][15] method to password-protect the PDF.
*   Save HTML as PDF using [Document.save(String)][16] method.

The following code sample shows how to convert HTML to password-protected PDF.

{{< gist aspose-com-gists c6fe5ccefe38a5ec03d983307eb0e850 "convert-html-to-password-protected-pdf.java" >}}

## HTML to PDF Conversion using URL {#HTML-to-PDF-Conversion-using-URL}

The following are the steps to convert a web page to PDF using a URL.

*   Create and initialize the [URL][17] object.
*   Get the web page into the [InputStream][18]object.
*   Create the [Document][19] object and initialize it with _InputStream _and _HtmlLoadOptions _objects.
*   Save HTML as PDF using [Document.save(String)][20] method.

The following code sample shows how to save a web page as PDF in Android programmatically.

{{< gist aspose-com-gists c6fe5ccefe38a5ec03d983307eb0e850 "convert-html-to-pdf-using-URL.java" >}}

## Get a Free License {#Get-Free-Licence}

You can [get a free license][21] in order to use Android HTML to PDF converter library without evaluation limitations.

## Conclusion

In this article, you have learned how to convert HTML files to PDF in Android programmatically. Furthermore, you have seen how to convert a web page to PDF or generate a password-protected PDF from HTML. You can explore more about the Android PDF library using [documentation][22]. In case you would have any queries, feel free to let us know via our [forum][23].

## See Also

*   [Create PDF Files using Java – Java PDF API][24]




[1]: https://docs.fileformat.com/web/html/
[2]: https://docs.fileformat.com/pdf/
[3]: #Android-HTML-to-PDF-Converter-Library
[4]: #HTML-to-PDF-in-Android-Programmatically
[5]: #Convert-HTML-to-Password-protected-PDF
[6]: #HTML-to-PDF-Conversion-using-URL
[7]: #Get-Free-Licence
[8]: https://products.aspose.com/pdf/android-java
[9]: https://downloads.aspose.com/pdf/androidjava
[10]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/HtmlLoadOptions
[11]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[12]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document#save-java.lang.String-
[13]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/HtmlLoadOptions
[14]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[15]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document#encrypt-java.lang.String-java.lang.String-int-int-
[16]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document#save-java.lang.String-
[17]: https://docs.oracle.com/javase/7/docs/api/java/net/URL.html
[18]: https://docs.oracle.com/javase/7/docs/api/java/io/InputStream.html
[19]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[20]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document#save-java.lang.String-
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/pdf/androidjava/
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/





