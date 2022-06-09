---
title: 'Find and Replace Text in Word Documents using C++'
seoTitle: "Find and Replace Text in Word Documents using C++ | C++ Word API"
description: "Find and replace text in Word documents using C++. Replace text with plain text or regular expressions. Complete tutorial with C++ code samples."
date: Tue, 12 Jan 2021 16:55:32 +0000
draft: false
url: /2021/01/12/Find-and-Replace-Text-in-Word-Documents-using-CPP/
author: Usman Aziz
summary: 'Find and replace is a useful feature provided by MS Word that lets you update all occurrences of a particular text at once. Thus, you do not have to locate and replace the text in the whole document manually. In this article, you will learn **how to find and replace text in Word documents from within C++ applications**. This could be useful when you need to replace a particular text in a number of documents in one go.'
tags: ['CPP-API-to-Find-and-Replace-Text', 'Find-and-Replace-Text-in-Word-Documents', 'Ignore-Text-during-Find-and-Replace-Operation', 'Replace-Text-using-Meta-Characters', 'Use-Regular-Expressions-to-Find-and-Replace-Text']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/C-Find-and-Replace-Text.png" alt="find and replace text in Word C++">}}


Find and replace is a useful feature provided by MS Word that lets you update all occurrences of a particular text at once. Thus, you do not have to locate and replace the text in the whole document manually. In this article, you will learn **how to find and replace text in Word documents from within C++ applications**. This could be useful when you need to replace a particular text in a number of documents in one go.

*   [C++ API to Find and Replace Text][1]
*   [Find and Replace Text in Word Documents][2]
*   [Use Regular Expressions to Find and Replace Text][3]
*   [Replace Text using Meta-Characters][4]
*   [Ignore Text during Find and Replace Operation][5]
*   [Get Free License][6]

## C++ API to Find and Replace Text {#C++-API-to-Find-and-Replace-Text}

[Aspose.Words for C++][7] is a C++ library for creating new and manipulating existing Word documents. The API supports a wide range of basic as well as advanced Word automation features. You can [download][8] the API package or install it using [NuGet][9].

```
Install-Package Aspose.Words.Cpp
```

## Find and Replace Text in Word Documents using C++ {#Find-and-Replace-Text-in-Word-Documents}

The following are the steps to find and replace text in Word documents using Aspose.Words for C++.

*   Load the Word document using [Document][10] class.
*   Replace the desired word using _Document->get\_Range()->Replace(u"sad", u"bad", System::MakeObject<[FindReplaceOptions][11]\>(FindReplaceDirection::Forward))_ method.
*   Save the updated Word document using [Document->Save(String)][12] method.

The following code sample shows how to find and replace the word "sad" with "bad" in a Word document using C++.

{{< gist aspose-com-gists 1e31a5c8733210d428000bc330d6199f "find-replace-text.cpp" >}}

## Find and Replace Text using Regular Expressions {#Use-Regular-Expressions-to-Find-and-Replace-Text}

You can also define the regular expressions in order to find and replace the words that follow a particular pattern. For example, you can replace the words "sad" and "mad" with the word "bad". The following are the steps to find and replace words matching a regular expression in a Word document.

*   Load the Word document using [Document][13] class.
*   Use [Regex][14] class to define the regex.
*   Replace the desired word using _Document->get\_Range()->Replace(System::MakeObject<[System::Text::RegularExpressions::Regex][15]\>(u"\[s|m\]ad"), u"bad", options)_ method.
*   Save the updated Word document using [Document->Save(String)][16] method.

The following code sample shows how to find and replace text using regular expression in C++.

{{< gist aspose-com-gists 1e31a5c8733210d428000bc330d6199f "find-replace-text-regex.cpp" >}}

## Find and Replace Text using Meta-Characters {#Find-and-Replace-Text-using-Meta-Characters}

In certain cases, the text you want to replace could include the breaks i.e. line break, paragraph break, section break, etc. In order to deal with such scenarios, Aspose.Words for C++ supports the following meta characters in the search and replacement strings.

*   **&p** for a paragraph break
*   **&b** for section break
*   **&m** for page break
*   **&l** for a manual line break

The following code sample shows how to find and replace text using meta-characters in a Word document.

{{< gist aspose-com-gists 1e31a5c8733210d428000bc330d6199f "find-replace-text-meta-chars.cpp" >}}

## Ignore Text during Find and Replace Operation {#Ignore-Text-during-Find-and-Replace}

Aspose.Words for C++ also allows you to ignore the text within fields and the revisions during the find and replace operation. The [FindReplaceOptions][17] class lets you specify the options to add this customization. The FindReplaceOptions class provides the following methods to ignore text in different scenarios:

*   [set\_IgnoreFields(bool)][18] - Ignores text inside the fields
*   [set\_IgnoreDeleted(bool)][19] - Ignores text inside the delete revisions
*   [set\_IgnoreInserted(bool)][20] - Ignores text inside the insert revisions

The following code sample shows how to ignore text in each of the above-mentioned scenarios.

{{< gist aspose-com-gists 1e31a5c8733210d428000bc330d6199f "find-replace-text-ignore-text.cpp" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][21] in order to try the API without evaluation limitations.

## Conclusion

In this article, you have seen how to find and replace text in Word documents using C++. The step by step guide and code samples have shown how to customize the find and replace feature in different scenarios. You can explore more about the C++ Word automation API using [documentation][22].

## See Also

*   [Protect or Unprotect Word Documents using C++][23]




[1]: #C++-API-to-Find-and-Replace-Text
[2]: #Find-and-Replace-Text-in-Word-Documents
[3]: #Use-Regular-Expressions-to-Find-and-Replace-Text
[4]: #Find-and-Replace-Text-using-Meta-Characters
[5]: #Ignore-Text-during-Find-and-Replace
[6]: #Get-Free-License
[7]: https://products.aspose.com/words/cpp
[8]: https://downloads.aspose.com/words/cpp
[9]: https://www.nuget.org/packages/Aspose.Words.cpp
[10]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[11]: https://apireference.aspose.com/words/cpp/class/aspose.words.replacing.find_replace_options/
[12]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a4ba337135cd6c8bed74a268ba60218bd
[13]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[14]: https://apireference.codeporting.com/native/cs2cpp/class/system.text.regular_expressions.regex
[15]: https://apireference.codeporting.com/native/cs2cpp/class/system.text.regular_expressions.regex
[16]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a4ba337135cd6c8bed74a268ba60218bd
[17]: https://apireference.aspose.com/words/cpp/class/aspose.words.replacing.find_replace_options
[18]: https://apireference.aspose.com/words/cpp/class/aspose.words.replacing.find_replace_options#acf22269e0ea135c2328ee5d36bbc2f33
[19]: https://apireference.aspose.com/words/cpp/class/aspose.words.replacing.find_replace_options#a4e77e5fdc05ef2f64d1c479e53575133
[20]: https://apireference.aspose.com/words/cpp/class/aspose.words.replacing.find_replace_options#afd7198fbf4887db570f152224c669edf
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/words/cpp/getting-started/
[23]: https://blog.aspose.com/2021/01/05/protect-or-unprotect-word-documents-using-cpp/





