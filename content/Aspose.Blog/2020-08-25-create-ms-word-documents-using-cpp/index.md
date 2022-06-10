---
title: 'Create MS Word Documents (DOC/DOCX) using C++'
seoTitle: "Create MS Word Documents in C++ | Add Text, Image, Table, List in Docs"
description: "C++ Word Processing API to create MS Word DOC/DOCX documents using C++. Insert text, tables, images, lists, and other elements in Word documents."
date: Tue, 25 Aug 2020 04:17:31 +0000
draft: false
url: /2020/08/25/create-ms-word-documents-using-cpp/
author: Usman Aziz
summary: '![Create Word Documents in C++][1]

[Aspose.Words][2] is a feature-rich collection of APIs that lets you create, edit, and convert MS Word documents programmatically. It provides a wide range of basic as well as advanced features for manipulating word processing documents. In this article, you will learn how to use [Aspose.Words for C++][3] and **create MS Word documents from scratch using C++**. The step by step guide as well as code samples will let you know how to insert text, images, tables, lists, and other elements in Word documents.'
tags: ['create doc using cpp', 'create word document cpp', 'insert image in Word document cpp', 'insert list in word document cpp', 'insert table in word document cpp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Create-Word-Document-in-C.jpg" alt="Create Word Documents in C++">}}


[Aspose.Words][4] is a feature-rich collection of APIs that lets you create, edit, and convert MS Word documents programmatically. It provides a wide range of basic as well as advanced features for manipulating word processing documents. In this article, you will learn how to use [Aspose.Words for C++][5] and **create MS Word documents from scratch using C++**. The step by step guide as well as code samples will let you know how to insert text, images, tables, lists, and other elements in Word documents.

*   [C++ Word Processing API][6]
*   [Create MS Word Documents using C++][7]
*   [Edit or Update Existing MS Word DOC/DOCX using C++][8]
*   [Insert Images in Word Documents using C++][9]
*   [Insert Table in Word Documents using C++][10]
*   [Add Lists in Word Documents using C++][11]

## C++ API to Create MS Word Documents {#C++-API-to-Create-Word-Documents}

[Aspose.Words for C++][12] lets you generate and manipulate the word processing documents within C++ applications without MS Word. You can [download][13] the API or install it within your C++ applications using [NuGet][14] with the following command.

```
PM> Install-Package Aspose.Words.Cpp
```

## Create MS Word Documents using C++ {#Create-MS-Word-Documents-using-C++}

Let's first create a simple Word document and save it as a _.doc_ or _.docx_ file. For this, you need to follow the below steps:

*   Create a blank Word document using [Document][15] class.
*   Create an object of [DocumentBuilder][16] class to add content to the document.
*   Add text using [DocumentBuilder->Writeln()][17] method.
*   Save the document as _.doc_ or _.docx_ file using [Document->Save()][18] method.

The following code sample shows how to create a Word DOCX document using C++.

{{< gist aspose-com-gists 6d4a3300f974c38f3d5f775c35d649e5 "create-word-document.cpp" >}}

## Edit or Update Existing Word DOC/DOCX using C++ {#Edit-or-Update-Existing-MS-Word-DOC-DOCX-using-C++}

You may also edit the existing Word documents using Aspose.Words for C++. For this, the API uses the Document Object Model (DOM) for the in-memory representation of a document. The DOM lets you access the elements of a Word document such as header/footer, paragraphs, tables, and etc. Read more about the DOM [here][19].

For updating a Word document, simply load it using [Document][20] class and process it as desired. The following are the steps to edit and update an existing Word document.

*   Load the Word document using [Document][21] class.
*   Create an object of [DocumentBuilder][22] class to access the content.
*   Access the desired paragraph (or any other element) and update the content.
*   Save the updated document using [Document->Save()][23] method.

The following code sample shows how to update the text of a paragraph in a Word document using C++.

{{< gist aspose-com-gists 6d4a3300f974c38f3d5f775c35d649e5 "update-word-document.cpp" >}}

## Insert Images in Word Document using C++ {#Insert-Images-in-Word-DOC-DOCX-using-C++}

The following are the steps to insert an image within MS Word documents using C++.

*   Create a new Word document or load an existing one using [Document][24] class.
*   Create a [DocumentBuilder][25] object and initialize it with the _Document_ object.
*   Insert image using [DocumentBuilder->InsertImage(String fileName, RelativeHorizontalPosition horzPos, double left, RelativeVerticalPosition vertPos, double top, double width, double height, WrapType wrapType)][26] method.
*   Save the document as a Word file.

The following code sample shows how to insert an image into a Word document using C++.

{{< gist aspose-com-gists 6d4a3300f974c38f3d5f775c35d649e5 "create-word-document-image.cpp" >}}

## Insert Table in Word Documents using C++ {#Insert-Table-in-Word-Documents-using-C++}

The table is an important element of the Word documents to keep the data in the form of rows and columns. In order to generate a table within the Word documents, follow the below steps.

*   Create a new Word document using [Document][27] class.
*   Create an object of [Table][28] class.
*   Insert table into the document using _Document->get\_FirstSection()->get\_Body()->AppendChild()_ method.
*   Create a new row using the [Row][29] class.
*   Insert row into the table using _Table->AppendChild(row)_ method.
*   Create and new [Cell][30] and insert text into it using [Cell->get\_FirstParagraph()->AppendChild()][31] method.
*   Insert cell into the row using _Row->AppendChild()_ method.
*   Repeat the process for adding multiple rows.
*   Save the document using [Document->Save()][32] method.

The following code sample shows how to insert a table in Word document using C++.

{{< gist aspose-com-gists 6d4a3300f974c38f3d5f775c35d649e5 "create-word-document-table.cpp" >}}

## Add Lists in Word Documents using C++ {#Add-Lists-in-Word-Documents-using-C++}

Last but not the least, creating a list in the Word documents. The following are the steps to create a bullet list.

*   Create a new Word document or load an existing one using [Document][33] class.
*   Define a new [DocumentBuilder][34] object and initialize it with the _Document_ object.
*   Create list using _DocumentBuilder->get\_ListFormat()->set\_List(Document->get\_Lists()->Add(ListTemplate::NumberArabicDot))_ method.
*   Populate the list and set the list level.
*   Save the document as a file.

The following code sample shows how to create a list in a Word document using C++.

{{< gist aspose-com-gists 6d4a3300f974c38f3d5f775c35d649e5 "create-word-document-list.cpp" >}}

## Conclusion

In this article, you have seen how to create MS Word documents from scratch using C++. Furthermore, you have learned how to insert elements such as text, images, tables, and lists in new or existing Word documents. You can explore more about the advanced features of the API using the [documentation][35].

## See Also

*   [Convert Word Documents to PDF using C++][36]




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2020/08/Create-Word-Document-in-C.jpg
[2]: https://products.aspose.com/words
[3]: https://products.aspose.com/words/cpp
[4]: https://products.aspose.com/words
[5]: https://products.aspose.com/words/cpp
[6]: #C++-API-to-Create-Word-Documents
[7]: #Create-MS-Word-Documents-using-C++
[8]: #Edit-or-Update-Existing-MS-Word-DOC-DOCX-using-C++
[9]: #Insert-Images-in-Word-DOC-DOCX-using-C++
[10]: #Insert-Table-in-Word-Documents-using-C++
[11]: #Add-Lists-in-Word-Documents-using-C++
[12]: https://products.aspose.com/words/cpp
[13]: https://downloads.aspose.com/words/cpp
[14]: https://www.nuget.org/packages/Aspose.Words.Cpp
[15]: https://apireference.aspose.com/words/cpp/class/aspose.words.document/
[16]: https://apireference.aspose.com/words/cpp/class/aspose.words.document_builder/
[17]: https://apireference.aspose.com/words/cpp/class/aspose.words.document_builder#a6d739b4d8b7260bdabb0e38967247f57
[18]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a4ba337135cd6c8bed74a268ba60218bd
[19]: https://docs.aspose.com/words/cpp/aspose-words-document-object-model/
[20]: https://apireference.aspose.com/words/cpp/class/aspose.words.document/
[21]: https://apireference.aspose.com/words/cpp/class/aspose.words.document/
[22]: https://apireference.aspose.com/words/cpp/class/aspose.words.document_builder/
[23]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a4ba337135cd6c8bed74a268ba60218bd
[24]: https://apireference.aspose.com/words/cpp/class/aspose.words.document/
[25]: https://apireference.aspose.com/words/cpp/class/aspose.words.document_builder/
[26]: https://apireference.aspose.com/words/cpp/class/aspose.words.document_builder#a453a3318c31c6b6fdc24a66ff925b711
[27]: https://apireference.aspose.com/words/cpp/class/aspose.words.document/
[28]: https://apireference.aspose.com/words/cpp/class/aspose.words.tables.table/
[29]: https://apireference.aspose.com/words/cpp/class/aspose.words.tables.row/
[30]: https://apireference.aspose.com/words/cpp/class/aspose.words.tables.cell/
[31]: https://apireference.aspose.com/words/cpp/class/aspose.words.tables.cell#a03648eef87125673be8882e8f4e053a9
[32]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a4ba337135cd6c8bed74a268ba60218bd
[33]: https://apireference.aspose.com/words/cpp/class/aspose.words.document/
[34]: https://apireference.aspose.com/words/cpp/class/aspose.words.document_builder/
[35]: https://docs.aspose.com/words/cpp/getting-started/
[36]: https://blog.aspose.com/2020/04/10/convert-word-doc-or-docx-to-pdf-in-cpp/





