---
title: 'Convert Word Documents to HTML using C#'
seoTitle: "Convert Word to HTML in C# | DOCX to HTML | DOC to HTML | .NET API"
description: "Use .NET Word API to convert Word document to HTML using C# or VB.NET. Control DOCX or DOC to HTML conversion with additional options dynamically."
date: Sat, 02 Oct 2021 17:06:00 +0000
draft: false
url: /2021/10/02/convert-word-to-html-using-csharp/
author: Usman Aziz
summary: 'In various cases, you need to display the content of the Word documents in your web or desktop applications. One of the suitable options in such cases is the conversion of Word documents to [HTML][1]. To achieve this from within the .NET applications, this article covers **how to convert Word [DOCX][2] or [DOC][3] files to HTML using C#**. Moreover, you will learn how to control Word to HTML conversion dynamically using different options.'
tags: ['DOC to HTML Csharp', 'DOCX to HTML Csharp', 'Word to HTML Csharp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-HTML.jpg" alt="Word to HTML C#">}}


In various cases, you need to display the content of the Word documents in your web or desktop applications. One of the suitable options in such cases is the conversion of Word documents to [HTML][4]. To achieve this from within the .NET applications, this article covers **how to convert Word [DOCX][5] or [DOC][6] files to HTML using C#**. Moreover, you will learn how to control Word to HTML conversion dynamically using different options.

*   [C# API for Word to HTML Conversion][7]
*   [Convert a Word Document to HTML][8]
*   [Customize Word to HTML Conversion][9]

## C# API for Word to HTML Conversion {#API-for-Word-to-HTML-Conversion}

To perform Word to HTML conversion from within the .NET applications, we will use [Aspose.Words for .NET][10]. It is a powerful class library that lets you create and manipulate Word documents. Also, it allows you to convert Word documents to various other file formats. You can either [download][11] the API or install it using [NuGet][12].

```
PM> Install-Package Aspose.Words 
```

## Convert a Word Document to HTML in C# {#Convert-a-Word-Document-to-HTML}

Aspose.Words for .NET makes it quite easier for you to convert a Word document to HTML. Simply load the Word document and save it as an HTML file. The following are the steps to convert a Word DOCX file to HTML in C#.

*   Load the Word document using [Document][13] class.
*   Convert Word document to HTML using [Document.Save(string, SaveFormat)][14] method.

The following code sample shows how to convert a Word document to HTML using C#.

{{< gist aspose-com-gists 4ab4b49bfb1d048e531c1811ac307560 "word-to-html.cs" >}}

## Customize Word to HTML Conversion in C# {#Customize-Word-to-HTML-Conversion}

Aspose.Words for .NET also allows you to customize the Word to HTML conversion using different options. For example, you can specify a folder to keep the resource files (CSS, fonts, and image) separately. In addition, you can export round-trip information of the document. The following sections demonstrate how to use these options.

### Export Round-trip Information in Word to HTML Conversion

MS Word provides a wide range of features and not all of these are supported by HTML. Therefore, to make the content of HTML close to the original document, round-trip information is used. The following steps show how to export round-trip information in Word to HTML conversion.

*   Load the Word document using [Document][15] class.
*   Create an object of [HtmlSaveOptions][16] class.
*   Enable export of round-trip information using [HtmlSaveOptions.ExportRoundtripInformation][17] property.
*   Convert Word document to HTML using [Document.Save(string, HtmlSaveOptions)][18] method.

The following code sample shows how to export round-trip information in Word to HTML conversion.

{{< gist aspose-com-gists 4ab4b49bfb1d048e531c1811ac307560 "word-to-html-roundtrip-info.cs" >}}

### Specify Resource Folder in Word to HTML Conversion

While performing Word to HTML conversion, you can save the resource files in a separate folder. Also, you can specify folders to keep fonts and images separately. The following are the steps to achieve this.

*   Load the Word document using [Document][19] class.
*   Create an object of [HtmlSaveOptions][20] class.
*   Set resource folder using [HtmlSaveOptions.ResourceFolder][21] property.
*   Convert Word document to HTML using [Document.Save(string, HtmlSaveOptions)][22] method.

The following code sample shows how to keep resources in a separate folder in Word to HTML conversion.

{{< gist aspose-com-gists 4ab4b49bfb1d048e531c1811ac307560 "word-to-html-resources.cs" >}}

[Read more][23] about working with resource folders in Word to HTML conversion.

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][24] in order to use Aspose.Words for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to convert Word DOCX or DOC documents to HTML using C#. Furthermore, you have seen how to use different options to customize Word to HTML conversion. You can also explore other features of Aspose.Words for .NET using the [documentation][25]. In addition, you can post your queries on our [forum][26].

## See Also

*   [Create Word Documents in C# wihtout MS Office][27]
*   [Convert Word Documents to PDF in C#][28]




[1]: https://docs.fileformat.com/web/html/
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: https://docs.fileformat.com/word-processing/doc/
[4]: https://docs.fileformat.com/web/html/
[5]: https://docs.fileformat.com/word-processing/docx/
[6]: https://docs.fileformat.com/word-processing/doc/
[7]: #API-for-Word-to-HTML-Conversion
[8]: #Convert-a-Word-Document-to-HTML
[9]: #Customize-Word-to-HTML-Conversion
[10]: https://products.aspose.com/words/net/
[11]: https://downloads.aspose.com/words/net
[12]: https://nuget.org/packages/Aspose.Words
[13]: https://apireference.aspose.com/words/net/aspose.words/document
[14]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/3
[15]: https://apireference.aspose.com/words/net/aspose.words/document
[16]: https://apireference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions
[17]: https://apireference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/properties/exportroundtripinformation
[18]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/4
[19]: https://apireference.aspose.com/words/net/aspose.words/document
[20]: https://apireference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions
[21]: https://apireference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/properties/resourcefolder
[22]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/4
[23]: https://docs.aspose.com/words/net/convert-a-document-to-html-mhtml-or-epub/#specify-a-folder-for-saving-resources
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/words/net
[26]: https://forum.aspose.com/
[27]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/
[28]: https://blog.aspose.com/2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/




