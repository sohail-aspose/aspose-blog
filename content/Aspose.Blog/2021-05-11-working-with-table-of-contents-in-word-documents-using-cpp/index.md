---
title: 'Working with Table of Contents in Word Documents using C++'
seoTitle: "Working with Table of Contents in Word Documents using C++"
description: "Working with table of contents in Word files using C++. Learn how to add, read, update and remove the table of contents from Word files using C++."
date: Tue, 11 May 2021 02:12:21 +0000
draft: false
url: /2021/05/11/working-with-table-of-contents-in-word-documents-using-cpp/
author: Muhammad Ahmad
summary: "Table of Contents (TOC) is an important part of a Word Document. It provides an overview of the document's content and allows you to navigate to your desired section quickly. You might find yourself in scenarios where you need to add, extract, update or remove the table of contents from Word documents programmatically. To that end, this article will teach you **how to work with the table of contents in Word files using C++**."
tags: ['Add Table of Contents in a Word Document C++', 'Extract Table of Contents from a Word Document C++', 'Remove Table of Contents from a Word Document C++', 'Update Table of Contents in a Word Document C++']
categories: ['Aspose.Words Product Family']
---

Table of Contents (TOC) is an important part of a Word Document. It provides an overview of the document's content and allows you to navigate to your desired section quickly. You might find yourself in scenarios where you need to add, extract, update or remove the table of contents from Word documents programmatically. To that end, this article will teach you **how to work with the table of contents in Word files using C++**.

*   [C++ API for Working with Table of Contents in Word Documents][1]
*   [Add the Table of Contents in a Word Document][2]
*   [Extract the Table of Contents from a Word Document][3]
*   [Update the Table of Contents in a Word Document][4]
*   [Remove the Table of Contents from a Word Document][5]

## C++ API for Working with Table of Contents in Word Documents {#CPP-API-for-Working-with-Table-of-Contents-in-Word-Documents}

[Aspose.Words for C++][6] is a native C++ library that allows you to create, read, modify and convert Microsoft Word documents. In addition, it also supports working with the table of contents in Word files. You can either install the API through [NuGet][7] or download it directly from the [Downloads][8] section.

```
PM> Install-Package Aspose.Words.Cpp
```

## **Add the Table of Contents in a Word Document** {#Add-the-Table-of-Contents-in-a-Word-Document}

The following are the steps to add a table of contents in a Word document.

*   Load the Word file using the [Document][9] class.
*   Create an instance of the [DocumentBuilder][10] class using the [Document][11] object created previously.
*   Insert the table of contents using the [DocumentBuilder->InsertTableOfContents(System::String switches)][12] method.
*   Populate the table of contents using the [Document->UpdateFields()][13] method.
*   Save the Word document using the [Document->Save(System::String fileName)][14] method.

The following sample code shows how to add a table of contents in a Word document using C++.

{{< gist aspose-com-gists 74023eecde943738bd5d1a406c64e638 "Add-Table-Of-Contents.cpp" >}}



{{< figure align=center src="images/AddTableOfContentsInWordCpp.png" alt="Output Word file containing the Table of Contents" caption="Output Word file containing the Table of Contents">}}


## Extract the Table of Contents from a Word Document {#Extract-the-Table-of-Contents-from-a-Word-Document}

The following are the steps to extract the table of contents from a Word document.

*   Load the Word file using the [Document][15] class.
*   Retrieve the fields using [Document->get\_Range()->get\_Fields()][16] method and loop over them.
*   Check whether the field is of the type [FieldType::FieldHyperlink][17].
*   Check if the field belongs to the table of contents.
*   Retrieve and print the field information.

The following sample code demonstrates how to extract the table of contents from a Word document using C++.

{{< gist aspose-com-gists 74023eecde943738bd5d1a406c64e638 "Extract-Table-Of-Contents.cpp" >}}

## Update the Table of Contents in a Word Document {#Update-the-Table-of-Contents-in-a-Word-Document}

If the document's content has been updated, and you need to reflect those changes in the table of contents, you simply need to load the Word file and call the [Document->UpdateFields()][18] method. This method will update the table of contents according to the modified content. After this, save the updated Word document.

## Remove the Table of Contents from a Word Document {#Remove-the-Table-of-Contents-from-a-Word-Document}

The following are the steps to remove the table of contents from a Word document.

*   Load the Word file using the [Document][19] class.
*   Retrieve and store a list of the [FieldStart][20] nodes.
*   Loop through the nodes until you reach the node of the type [NodeType::FieldEnd][21] that designates the end of the table of contents.
*   Remove the table of contents using the [Node->Remove()][22] method.
*   Save the Word document using the [Document->Save(System::String fileName)][23] method.

The following sample code shows how to remove the table of contents from a Word Document using C++.

{{< gist aspose-com-gists 74023eecde943738bd5d1a406c64e638 "Remove-Table-Of-Contents.cpp" >}}

## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][24].

## Conclusion

In this article, you have learned how to work with the table of contents in Word documents using C++. You have seen the steps and the sample code required to add, extract, update and remove the table of contents from Word documents. Aspose.Words for C++ provides many additional features for working with Word files. You can explore the API in detail by visiting the [official documentation][25]. In case of any questions, please feel free to reach us on our [free support forum][26].

## See Also

*   [Working with Comments in Word Documents using C++][27]
*   [Convert RTF Documents to PDF using C++][28]




[1]: #CPP-API-for-Working-with-Table-of-Contents-in-Word-Documents
[2]: #Add-the-Table-of-Contents-in-a-Word-Document
[3]: #Extract-the-Table-of-Contents-from-a-Word-Document
[4]: #Update-the-Table-of-Contents-in-a-Word-Document
[5]: #Remove-the-Table-of-Contents-from-a-Word-Document
[6]: https://products.aspose.com/words/cpp
[7]: https://www.nuget.org/packages/Aspose.Words.Cpp
[8]: https://downloads.aspose.com/words/cpp
[9]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[10]: https://apireference.aspose.com/words/cpp/class/aspose.words.document_builder
[11]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[12]: https://apireference.aspose.com/words/cpp/class/aspose.words.document_builder#a8f381559792fd8c84f9bf316a71eb17a
[13]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a9c2187d845fae7a8dd8a6a5241d69d25
[14]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a4ba337135cd6c8bed74a268ba60218bd
[15]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[16]: https://apireference.aspose.com/words/cpp/class/aspose.words.range#a198a629ae4d9d113740df7569c13fd39
[17]: https://apireference.aspose.com/words/cpp/namespace/aspose.words.fields#a07fe44a4500c375e409bae0f72c9edec
[18]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a9c2187d845fae7a8dd8a6a5241d69d25
[19]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[20]: https://apireference.aspose.com/words/cpp/class/aspose.words.fields.field_start
[21]: https://apireference.aspose.com/words/cpp/namespace/aspose.words#a344de11ed54cf046eea1f8954a396379
[22]: https://apireference.aspose.com/words/cpp/class/aspose.words.node#a75a9cc0fda5ec9c8aaa1c4910af8f28c
[23]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a4ba337135cd6c8bed74a268ba60218bd
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/words/cpp/
[26]: https://forum.aspose.com/c/words/8
[27]: https://blog.aspose.com/2021/05/05/working-with-comments-in-word-documents-using-cpp/
[28]: https://blog.aspose.com/2021/02/17/convert-rtf-documents-to-pdf-using-cpp/





