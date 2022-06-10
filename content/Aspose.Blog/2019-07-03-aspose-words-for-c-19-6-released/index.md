---
title: 'Compare Two Word Documents using C++'
date: Wed, 03 Jul 2019 13:11:09 +0000
draft: false
url: /2019/07/03/aspose-words-for-c-19-6-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

In this post, we will see how to compare two Word Documents by using C++ with [Aspose.Words for C++ 19.6][1] API.

## C++ MS Word Document Comparison

You can use [Document.Compare][2] method to compare two Word documents to see the difference between them. This method mimics Microsoft Word's Compare feature and produces document difference as a number of edit and format revisions. The main idea is that if we reject all revisions then we get a document that is equal to the original document. On the contrary, if we accept all revisions then we get the final (comparison target) document.

## Compare Word Documents using C++

The following example shows a normal comparison case.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Programming-Documents-Document-CompareDocument-NormalComparison.cpp" >}}

## C++ MS Word Comparison - Check If Documents are Same

The below example shows how to test that Word Documents are "Equal".

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Programming-Documents-Document-CompareDocument-CompareForEqual.cpp" >}}

### Limitations

There are a few general limitations:

*   The document being compared must not have revisions before this method is called.
*   Markup - is limited to SmartTag only. Other markups are ignored completely.
*   DML- Fallback shapes are compared instead of actual DML comparison.

> There is an important note regarding "equal". Actually "equality" means here that the comparison method is not able to represent changes as revisions. In general, it means that both document text and text formatting are the same. But there can be other difference between documents. For example, Word supports only format revisions for styles and we can't represent style insertion/deletion. So documents can have a different set of styles and the Compare method still produces no revisions.

## See Also Useful Links

The resources, you may need to accomplish your tasks:

*   [Aspose.Words for C++ Online Documentation][3] - up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Words for C++ Product Page][4]
*   [Install Aspose.Words for C++ NuGet Package][5]
*   [Aspose.Words for C++ API Reference Guide][6] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][7] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for C++ API by posting your suggestions and concerns in the [Aspose.Words for C++ support forum][8].




[1]: https://downloads.aspose.com/words/cpp/new-releases/aspose.words-for-c---19.6/
[2]: https://apireference.aspose.com/cpp/words/class/aspose.words.document/#ac7197138e35891d449cd3c1c9cc457a9
[3]: https://docs.aspose.com/display/wordscpp/Home
[4]: https://products.aspose.com/words/cpp
[5]: https://www.nuget.org/packages/Aspose.Words.Cpp/
[6]: https://apireference.aspose.com/cpp/words
[7]: https://github.com/aspose-words/Aspose.words-for-C
[8]: https://forum.aspose.com/c/words




