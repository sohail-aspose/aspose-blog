---
title: 'Protect or Unprotect Word Documents using C++'
seoTitle: "Protect Unprotect Word Documents in C++ | Password Protect DOCX C++"
description: "Protect or unprotect MS Word DOCX documents using C++. Protect Word document with desired protection type. Unprotect a protected document without password."
date: Tue, 05 Jan 2021 18:09:50 +0000
draft: false
url: /2021/01/05/protect-or-unprotect-word-documents-using-cpp/
author: Usman Aziz
summary: "The protection of digital documents has always been a hot topic. As far as Word documents are concerned, MS Word provides several content protection features that limit the user's access to the document. You can protect the document with a password and apply desired restrictions to avoid unauthorized access. In accordance with that, this article covers how to automate Word document protection within C++ applications. Particularly, you will learn **how to protect and unprotect Word documents using C++**."
tags: ['password protect word document cpp', 'protect word document cpp', 'unlock word document without password', 'unprotect word document cpp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Protect-Unprotect-Word-C.png" alt="Protect Unprotect Word C++">}}


The protection of digital documents has always been a hot topic. As far as Word documents are concerned, MS Word provides several content protection features that limit the user's access to the document. You can protect the document with a password and apply desired restrictions to avoid unauthorized access. In accordance with that, this article covers how to automate Word document protection within C++ applications. Particularly, you will learn **how to protect and unprotect Word documents using C++**.

*   [C++ API to Protect/Unprotect Word Documents][1]
*   [Protect Word Documents using C++][2]
*   [Unprotect Word Documents using C++][3]
*   [Get Free License][4]

## C++ API to Protect/Unprotect Word Documents {#C++-API-to-Protect-Unprotect-Word-Documents}

[Aspose.Words for C++][5] is built for creating and manipulating MS Word documents within C++ applications. The API provides basic as well as advanced document manipulation features that also cover protecting and unprotecting Word documents. You can either [download][6] the API package or install it from [NuGet][7].

```
PM> Install-Package Aspose.Words.Cpp
```

## Protect a Word Document using C++ {#Protect-Word-Documents-using-C++}

Aspose.Words for C++ allows you to use the following protection types in order to limit the user's access to the document.

*   **AllowOnlyComments** - Modification of comments in the document is allowed.
*   **AllowOnlyFormFields** - The user can only enter data in the form fields in the document.
*   **AllowOnlyRevisions** - The user can only add revision marks to the document.
*   **ReadOnly** - No changes are allowed to the document (available since Microsoft Word 2003).
*   **NoProtection** - The document is not protected.

The following are the steps to protect a Word document.

*   Load the MS Word document using [Document][8] class by specifying the file's path.
*   Use [Document->Protect(ProtectionType, String)][9] method to protect the document by specifying the protection type and the password.
*   Save the document using [Document->Save(String)][10] method.

The following code sample shows how to protect a Word document using C++.

{{< gist aspose-com-gists 8233bdf649063a776aa32877e4061d14 "protect-word-document.cpp" >}}

## Unprotect Word Document using C++ {#Unprotect-Word-Documents-using-C++}

Aspose.Words for C++ lets you unprotect MS Word documents even if you do not know the password. In order to unprotect a password-protected Word document, you can follow the below steps.

*   Load the MS Word document using [Document][11] class.
*   Use [Document->Unprotect()][12] method to unprotect the Word document.
*   Save the document using [Document->Save(String)][13] method.

{{< gist aspose-com-gists 8233bdf649063a776aa32877e4061d14 "unprotect-word-document.cpp" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][14] in order to try the API without evaluation limitations.

## Conclusion

MS Word document protection has been widely in practice in order to protect the documents from unauthorized users. Keeping an eye on it, this article covered how to protect Word documents as well as unprotect the password-protected documents using C++. You can explore more about the C++ Word API using [documentation][15].

## See Also

*   [Create MS Word Documents using C++][16]




[1]: #C++-API-to-Protect-Unprotect-Word-Documents
[2]: #Protect-Word-Documents-using-C++
[3]: #Unprotect-Word-Documents-using-C++
[4]: #Get-Free-License
[5]: https://products.aspose.com/words/cpp
[6]: https://downloads.aspose.com/words/cpp
[7]: http://nuget.org/packages/Aspose.Words.cpp
[8]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[9]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a1db98c43ec503fdaba623991ff1a32fc
[10]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a4ba337135cd6c8bed74a268ba60218bd
[11]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[12]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a7ab24b0f997f82af1a208ac9d5066059
[13]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a4ba337135cd6c8bed74a268ba60218bd
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/words/cpp/developer-guide/
[16]: https://blog.aspose.com/2020/08/25/create-ms-word-documents-using-cpp/





