---
title: 'Find and Replace Text in PDF using C#'
seoTitle: ""
description: ""
date: Tue, 22 Dec 2020 10:57:00 +0000
draft: false
url: /2020/12/22/find-and-replace-text-in-pdf-using-csharp/
author: Usman Aziz
summary: 'The find and replace option makes it possible to replace a particular piece of text in a document in one go. This way, you do not have to locate and update each occurrence of the text in the whole document manually. This article even goes one step further and covers how to automate find and replace text feature in PDF documents. Particularly, you will learn **how to find and replace text in a whole PDF, a particular page, or a page region using C#**.'
tags: ['find and replace text in pdf using csharp', 'find and replace text in pdf using regex']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/C-Find-and-Replace-Text-in-PDF.jpg" alt="C# find and replace text in PDF">}}


The find and replace option makes it possible to replace a particular piece of text in a document in one go. This way, you do not have to locate and update each occurrence of the text in the whole document manually. This article even goes one step further and covers how to automate the find and replace text feature in PDF documents. Particularly, you will learn **how to find and replace text in a whole PDF, a particular page, or a page region using C#**.

*   [C# API to Find and Replace Text in PDF][1]
*   [Find and Replace Text in PDF using C#][2]
*   [Replace Text in a Particular Page in PDF][3]
*   [Replace Text in PDF Page Region][4]
*   [Find and Replace Text in PDF using Regex][5]

## C# API to Find and Replace Text in PDF {#CSharp-API-to-Find-and-Replace-Text-in-PDF}

[Aspose.PDF for .NET][6] is a C# class library that provides basic as well as advanced PDF manipulation features for .NET applications. The API also lets you find and replace text in PDF files in different ways seamlessly. You can either [download][7] the API's DLL or install it using [NuGet][8].

```
PM> Install-Package Aspose.PDF
```

## Find and Replace Text in PDF using C# {#Find-and-Replace-Text-in-PDF-using-CSharp}

The following are steps to find and replace text in a PDF document.

*   Use [Document][9] class to load the PDF document using its path.
*   Create an instance of [TextFragmentAbsorber][10] class and provide the search phrase to its constructor.
*   Accept the text absorber for all the pages of the PDF using [Document.Pages.Accept(TextFragmentAbsorber)][11].
*   Get the extracted text fragments into [TextFragmentCollection][12] object.
*   Loop through the found [TextFragmentCollection][13] and replace text in each fragment.
*   Save updated PDF document using [Document.Save(String)][14] method.

The following code sample shows how to find and replace text in PDF using C#.

{{< gist aspose-com-gists 59dd796a6ed24191345670aff3ad9a99 "find-replace-text-pdf.cs" >}}

## Replace Text in a Particular PDF Page using C# {#Find-and-Replace-Text-in-a-Particular-Page}

The following are steps to find and replace text on a particular page in a PDF document.

*   Use [Document][15] class to load the PDF document using its path.
*   Create an instance of [TextFragmentAbsorber][16] class and provide the search phrase to its constructor.
*   Accept the text absorber for the desired page using [Document.Pages\[1\].Accept(TextFragmentAbsorber)][17].
*   Loop through the found [TextFragmentAbsorber.TextFragments][18] collection and replace text in each fragment.
*   Save updated PDF document using [Document.Save(String)][19] method.

The following code sample shows how to find and replace text in a particular page of the PDF using C#.

{{< gist aspose-com-gists 59dd796a6ed24191345670aff3ad9a99 "find-replace-text-pdf-page.cs" >}}

## Replace Text in PDF Page Region using C# {#Define-Page-Region-to-Find-and-Replace-Text}

You can also find and replace text in a particular region of the page in a PDF document. The following steps show how to define a particular region and then replace text within it.

*   Use [Document][20] class to load the PDF document using its path.
*   Create an instance of [TextFragmentAbsorber][21] class and provide the search phrase to its constructor.
*   Accept the text absorber for the desired page using [Document.Pages\[0\].Accept(TextFragmentAbsorber)][22].
*   Define the page region using the [Rectangle][23] class.
*   Loop through the [TextFragmentAbsorber.TextFragments][24] collection and replace text in each fragment.
*   Save updated PDF document using [Document.Save(String)][25] method.

The following code sample shows how to find and replace text in a particular page region in a PDF using C#.

{{< gist aspose-com-gists 59dd796a6ed24191345670aff3ad9a99 "find-replace-text-pdf-region.cs" >}}

## Replace Text in PDF using Regular Expression in C# {#Use-Regex-to-Find-and-Replace-Text-in-PDF}

You can also use regular expressions to find and replace the text occurrences matching a particular pattern. For this, you only need to provide a regular expression instead of the plain search phrase and use [TextSearchOptions][26]. The following are the steps to do so.

*   Use [Document][27] class to load the PDF document using its path.
*   Create an instance of [TextFragmentAbsorber][28] class and provide the search phrase to its constructor.
*   Create an instance of [TextSearchOptions][29] class and pass _true_ to its constructor to enable the regex-based search.
*   Assign the [TextSearchOptions][30] object to [TextFragmentAbsorber.TextSearchOptions][31] property.
*   Accept the text absorber for the desired page using [Document.Pages\[0\].Accept(TextFragmentAbsorber)][32].
*   Define the page region using the [Rectangle][33] class.
*   Loop through the [TextFragmentAbsorber.TextFragments][34] collection and replace text in each fragment.
*   Save updated PDF document using [Document.Save(String)][35] method.

The following code sample shows how to find and replace text in a PDF using regular expression using C#.

{{< gist aspose-com-gists 59dd796a6ed24191345670aff3ad9a99 "find-replace-text-pdf-regex.cs" >}}

## Conclusion

PDF automation is widely adopted these days in order to manipulate PDF documents from within the web or desktop applications. This article covered a useful PDF automation feature of finding and replacing text programmatically using C#. The step by step guide and code samples have shown how to find and replace text in a whole PDF, a particular page in PDF, or a page region. You can explore more advanced features using the [documentation][36] of the API.

## See Also

*   [Add or Remove Attachments in PDF using C#][37]




[1]: #CSharp-API-to-Find-and-Replace-Text-in-PDF
[2]: #Find-and-Replace-Text-in-PDF-using-CSharp
[3]: #Find-and-Replace-Text-in-a-Particular-Page
[4]: #Define-Page-Region-to-Find-and-Replace-Text
[5]: #Use-Regex-to-Find-and-Replace-Text-in-PDF
[6]: https://products.aspose.com/pdf/net
[7]: https://downloads.aspose.com/pdf/net
[8]: http://nuget.org/packages/Aspose.pdf
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentabsorber
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf.pagecollection/accept/methods/3
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentcollection
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentcollection
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentabsorber
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf.pagecollection/accept/methods/3
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentabsorber/properties/textfragments
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentabsorber
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf.pagecollection/accept/methods/3
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf/rectangle
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentabsorber/properties/textfragments
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textsearchoptions
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[28]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentabsorber
[29]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textsearchoptions
[30]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textsearchoptions
[31]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentabsorber/properties/textsearchoptions
[32]: https://apireference.aspose.com/pdf/net/aspose.pdf.pagecollection/accept/methods/3
[33]: https://apireference.aspose.com/pdf/net/aspose.pdf/rectangle
[34]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentabsorber/properties/textfragments
[35]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[36]: https://docs.aspose.com/pdf/net/overview/
[37]: https://blog.aspose.com/2020/12/15/add-or-remove-attachments-in-pdf-using-csharp/





