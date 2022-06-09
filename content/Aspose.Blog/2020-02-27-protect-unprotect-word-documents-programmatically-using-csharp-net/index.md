---
title: 'Protect or Unprotect Word Documents Programmatically using C#'
seoTitle: ""
description: ""
date: Thu, 27 Feb 2020 02:41:32 +0000
draft: false
url: /2020/02/27/protect-unprotect-word-documents-programmatically-using-csharp-net/
author: Usman Aziz
summary: ''
tags: ['make word document read only', 'protect word document in csharp', 'unprotect word document without password']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Protect-Unprotect-Word-C.png" alt="">}}


**Microsoft Word** supports a variety of protection features to protect the whole Word document or some parts of the document. **Document protection** comes into practice when you need to share the document with another person or party. In such cases, you may want to limit the third party's access or permissions. On the other hand, you can also specify a password to avoid unauthorized access to the document. This article is also comprised of some easy ways to **protect Word documents programmatically**. Furthermore, you'll also learn how to **unprotect Word documents** without a password. In the subsequent sections, you'll learn how to:

*   protect Word documents using C#,
*   protect Word documents with a password in C#, and
*   unprotect Word documents without a password in C#.

## .NET API to Protect/Unprotect Word Documents

[Aspose.Words for .NET][1] is an API to manipulate Word documents programmatically in the .NET applications. Along with other document manipulation features, the API provides easy yet powerful features to protect and unprotect Word documents. You can [download][2] _Aspose.Words for .NET_ DLL or install it in your project using the following ways in Visual Studio:

### NuGet Package Manager



{{< figure align=center src="images/Aspose.Words-NuGet.png" alt="protect or unprotect Word document">}}


### Package Manager Console```
PM> Install-Package Aspose.Words
```

## Protect Word Documents using C#

Aspose.Words for .NET provides the following protection types to secure a Word document:

*   **AllowOnlyComments** \- To allow modification of comments only.
*   **AllowOnlyFormFields** \- To allow data entry into the form fields only.
*   **AllowOnlyRevisions** \- To allow adding revision marks only.
*   **ReadOnly** \- Completely read-only (no changes are allowed to the document).
*   **NoProtection** \- No protection at all.

The following are the steps to apply protection to a Word document:

*   Create an instance of [Document][3] class and initialize it with the Word document's path.
*   Call [Document.Protect(ProtectionType)][4] method by providing desired [ProtectionType][5] value.
*   Call [Document.Save(String)][6] method to save the protected Word document.

The following code sample shows how to protect a Word document in C#.

{{< gist aspose-com-gists b119c2cc8610cb2f3a0d6f76ab4b8108 "protect-word-document.cs" >}}

## Protect Word Documents with Password in C#

The following are the steps to protect a Word document with a password:

*   Create an instance of [Document][7] class and initialize it with the Word document's path.
*   Call [Document.Protect(ProtectionType, String)][8] method by providing the [ProtectionType][9] value and a password.
*   Call [Document.Save(String)][10] method to save the protected Word document.

The following code sample shows how to protect a Word document using a password in C#.

{{< gist aspose-com-gists b119c2cc8610cb2f3a0d6f76ab4b8108 "protect-word-document-with-password.cs" >}}

## Unprotect Word Documents without a Password in C#

_Aspose.Words for .NET_ has the ability to unprotect a Word document even if you don't have the password. The following are the steps to unprotect a Word document:

*   Create an instance of [Document][11] class and initialize it with the Word document's path.
*   Call [Document.Unprotect()][12] method.
*   Call [Document.Save(String)][13] method to save the unprotected Word document.

The following code sample shows how to unprotect a Word document without a password in C#.

{{< gist aspose-com-gists b119c2cc8610cb2f3a0d6f76ab4b8108 "unprotect-word-document.cs" >}}

## Try Aspose.Words for .NET for Free

You can get a [temporary license][14] to try and use _Aspose.Words for .NET_ for free.




[1]: https://products.aspose.com/words/net
[2]: https://downloads.aspose.com/
[3]: https://apireference.aspose.com/net/words/aspose.words/document
[4]: https://apireference.aspose.com/net/words/aspose.words/document/methods/protect
[5]: https://apireference.aspose.com/net/words/aspose.words/protectiontype
[6]: https://apireference.aspose.com/net/words/aspose.words.document/save/methods/2
[7]: https://apireference.aspose.com/net/words/aspose.words/document
[8]: https://apireference.aspose.com/net/words/aspose.words.document/protect/methods/1
[9]: https://apireference.aspose.com/net/words/aspose.words/protectiontype
[10]: https://apireference.aspose.com/net/words/aspose.words.document/save/methods/2
[11]: https://apireference.aspose.com/net/words/aspose.words/document
[12]: https://apireference.aspose.com/net/words/aspose.words/document/methods/unprotect
[13]: https://apireference.aspose.com/net/words/aspose.words.document/save/methods/2
[14]: https://purchase.aspose.com/temporary-license





