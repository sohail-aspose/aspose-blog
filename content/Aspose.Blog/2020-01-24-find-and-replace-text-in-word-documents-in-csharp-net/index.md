---
title: 'Find and Replace Text in a Word Document using C# .NET'
seoTitle: "Find and Replace Text in Word Documents in C# .NET | .NET Core"
description: "Learn useful ways to find and replace text in Word document in C#. Find and replace text or phrase in Word DOC DOCX in C#. Without MS Word/Office interop."
date: Fri, 24 Jan 2020 13:54:06 +0000
draft: false
url: /2020/01/24/find-and-replace-text-in-word-documents-in-csharp-net/
author: Usman Aziz
summary: 'This article covers various approaches to **find and replace text in Word documents** using **C#** in **.NET** or **.NET Core** applications.'
tags: ['Word Document Finding and Replacing Text in C#.NET', 'c# find and replace text in word document', 'c# replace text in docx file', 'find and replace text in word document', 'find text in word document using c#', 'how to replace text in word document']
categories: ['Aspose.Words Product Family']
---

This article covers various approaches to **find and replace text in Word documents** using **C#** in **.NET** or **.NET Core** applications.



{{< figure align=center src="images/C-Find-and-Replace-Text.png" alt="">}}


**Find and Replace** is quite a useful feature of **MS Word** to quickly locate and replace the desired text in the documents. It becomes more handy and time-saving when you are working with longer documents. In cases when you need to find and replace text in hundreds of Word documents or you need to automate this process, you'll definitely opt to do it programmatically. So in this article, I'll show you how to **find and replace text in Word documents** programmatically in different scenarios using **C#**. Once you have read this article, you will be able to:

*   [find and replace text in Word DOC/DOCX using C#][1]
*   [find and replace similar words in Word document][2]
*   [find and replace text using Regex][3]
*   [find and replace text in the header/footer of Word document][4]
*   [find and replace text with meta-characters in Word document][5]

**TIP**: You may be interested in a free [Text to GIF Converter][6] that allows you to generate animations from texts.

## C# Library to Find and Replace Text in a Word Document

First of all, create a new C# project (Console, ASP.NET, etc.) in Visual Studio and install [Aspose.Words for .NET][7] via NuGet Package Manager or Package Manager Console.

### Installing via NuGet Package Manager



{{< figure align=center src="images/Aspose.Words-NuGet.png" alt="Finding and replacing text in Word DOC">}}


### Installing via Package Manager Console```
PM> Install-Package Aspose.Words
```

After we have installed _Aspose.Words for .NET_, let's now begin finding and replacing text in the following Word document.



{{< figure align=center src="images/Word-Document.png" alt="c# find and replace text in word document ">}}


## Find and Replace Text in Word Documents in C# {#find-and-replace-text-in-Word-DOC-DOCX-using-CSharp}

The following are the steps to find and replace a particular text in a Word document using _Aspose.Words for .NET_.

*   Create an instance of [Document][8] class and initialize with Word document's path.
*   Find and replace text using [Document.Range.Replace(string, string, FindReplaceOptions)][9] method.
*   Save the document using [Document.Save(string)][10] method.

The [FindReplaceOptions][11] class provides various options to customize the find/replace operations. The following code sample shows how to find and replace a particular word or string in a Word document using C#.

{{< gist aspose-com-gists dafaf8f41192a14524e1e88cc2ce4742 "find-and-replace-text-in-word-document.cs" >}}

### Output



{{< figure align=center src="images/Find-And-Replace-Text-In-Document.png" alt="find text in word document using c#">}}


## Find and Replace Similar Words in Word Documents using C# {#find-and-replace-similar-words-in-Word-document}

You can also customize the API to find similar words and replace them with a particular word. For example, you can find the words "sad" and "mad" and replace them with a single word. The following code sample shows how to find and replace similar words in Word document using C#.

{{< gist aspose-com-gists dafaf8f41192a14524e1e88cc2ce4742 "find-and-replace-words-in-word-document.cs" >}}

### Output



{{< figure align=center src="images/Find-And-Replace-Multiple-Word-In-Document.png" alt="c# replace text in docx file">}}


## Find and Replace Text using Regex in C# {#find-and-replace-text-using-Regex}

There might be the case when you want to find and replace text that appears in a particular pattern. For example, you need to hide/replace all the email IDs in a Word document. In such cases, you can create a regular expression for email IDs and pass it to [Document.Range.Replace(Regex, string, FindReplaceOptions)][12] method.

The following code sample shows how to find and replace text based on a pattern in Word document.

{{< gist aspose-com-gists dafaf8f41192a14524e1e88cc2ce4742 "find-and-replace-text-in-word-document-regex.cs" >}}

### Output



{{< figure align=center src="images/Find-And-Replace-Text-Regex-In-Document.png" alt="how to replace text in word document">}}


## Find and Replace Text in Header/Footer of Word Document using C# {#find-and-replace-text-in-the-header-footer-of-Word-document}

You can also find and replace text in the header or footer sections of a Word document using the [HeaderFooter][13] class. The _HeaderFooter.Range.Replace(string, string, FindReplaceOptions)_ method is used for this purpose. The following code sample shows how to replace text in the header/footer of Word document in C#.

{{< gist aspose-com-gists dafaf8f41192a14524e1e88cc2ce4742 "find-and-replace-text-in-footer-in-word-document.cs" >}}

### Output



{{< figure align=center src="images/Find-And-Replace-Text-In-Footer.png" alt="Word Document Finding and Replacing Text in C#.NET">}}


## Find and Replace Text with Meta-Characters in Word Documents using C# {#find-and-replace-text-with-meta-characters-in-Word-document}

There could be a scenario where a particular text or phrase is composed of multiple paragraphs, sections, or pages. In such cases, the simple find and replace method wouldn't work effectively and we'll have to handle the paragraphs breaks, section breaks, or page breaks. For this, _Aspose.Words_ allows you to use the following meta-characters in the search string or the replacement string:

*   **&p**: paragraph break
*   **&b**: section break
*   **&m**: page break 
*   **&l**: line break

The following code sample shows how to find and replace the text with a paragraph break in a Word document.

{{< gist aspose-com-gists dafaf8f41192a14524e1e88cc2ce4742 "find-and-replace-text-with-paragraph-break.cs" >}}

### Output



{{< figure align=center src="images/Find-And-Replace-Text-with-Paragraph-Break.png" alt="find and replace text using regular expression C#">}}


## Conclusion

This article covers some useful ways to **find and replace text in a Word document** based on matched or similar words, phrases, and regex patterns programmatically. These features not only automate the text replacement process but save you a lot of time and effort required in manual find and replace operation in Word documents. You can learn more about Aspose's Word Library using [documentation][14].

## Related Article(s)

*   [Find and Replace Text in Word Documents using Java][15]
*   [.NET Word Automation - Create Rich Word Documents in C#][16]




[1]: #find-and-replace-text-in-Word-DOC-DOCX-using-CSharp
[2]: #find-and-replace-similar-words-in-Word-document
[3]: #find-and-replace-text-using-Regex
[4]: #find-and-replace-text-in-the-header-footer-of-Word-document
[5]: #find-and-replace-text-with-meta-characters-in-Word-document
[6]: https://products.aspose.app/slides/text-to-gif
[7]: https://products.aspose.com/words/net
[8]: https://apireference.aspose.com/net/words/aspose.words/document
[9]: https://apireference.aspose.com/net/words/aspose.words.range/replace/methods/1
[10]: https://apireference.aspose.com/net/words/aspose.words.document/save/methods/2
[11]: https://apireference.aspose.com/net/words/aspose.words.replacing/findreplaceoptions
[12]: https://apireference.aspose.com/net/words/aspose.words.range/replace/methods/3
[13]: https://apireference.aspose.com/net/words/aspose.words/headerfooter
[14]: http://docs.aspose.com/display/wordsnet
[15]: https://blog.aspose.com/2020/06/16/find-and-replace-text-in-word-doc-docx-using-java/
[16]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/





