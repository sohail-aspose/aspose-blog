---
title: 'Insert Table in Word Documents (DOC/DOCX) using C++'
seoTitle: ""
description: ""
date: Sun, 20 Sep 2020 23:27:06 +0000
draft: false
url: /2020/09/20/insert-table-in-word-documents-programmatically-using-cpp/
author: Farhan Raza
summary: 'Using Aspose.Words for C++ API, you can insert tables in a word document. You can configure the API by downloading it from New Releases or via the NuGet gallery. Once configured properly, you can simply utilize the methods, properties, and classes exposed by the API so that a few simple API calls can be used to create, edit or manipulate Microsoft Word documents, like DOCX or DOC files.'
tags: ['insert table in docx', 'insert table in word', 'insert table in word document', 'insert table in word document cpp', 'nested table in word']
categories: ['Aspose.Words Product Family']
---

Tables are helpful to organize information and figures. We often insert tables in word documents ([DOCX][1]/[DOC][2] to show information. In a word processing application, you can easily create tables using C++. You can go through the following examples to learn working with Tables in Word documents:

*   [Insert Tables in Word Documents API][3]
*   [Insert a Table in Word Documents using C++][4]
*   [Insert Table from HTML in Word Documents using C++][5]
*   [Insert Table in DOCX Using Document Builder in C++][6]
    1.  [Insert Simple Table in DOCX with Document Builder using C++][7]
    2.  [Insert Formatted Table in DOCX with Document Builder using C++][8]
    3.  [Insert Nested Table in DOCX with Document Builder using C++][9]

Let us move on to explore all these topics in detail:

## Insert Tables in Word Documents API {#section1}

Firstly, please note that you will be using [Aspose.Words for C++][10] API to insert tables in a word document. You can configure the API by downloading it from [New Releases][11] or via the [NuGet][12] gallery. Once configured properly, you can simply utilize the methods, properties, and classes exposed by the API so that a few simple API calls can be used to create, edit or manipulate Microsoft Word documents, like DOCX or DOC files.

## Insert a Table in Word Documents using C++ {#section2}

You can insert a table in word documents with a few simple steps. However, it is important to note here that you must pass the document object to the constructor of each node so that all child nodes belong to the same object. You need to follow the steps listed below:

1.  Initialize object of [Document][13] class
2.  Create [Table][14] object
3.  Add the Table to Document
4.  Create Rows and Columns
5.  Apply [AutoFit][15] on Table Cells
6.  Save output Word Document

The code snippet below shows how to insert a Table in Word document (DOCX/DOC) using C++:

{{< gist aspose-com-gists a1f0027243154dace264e8733fda2345 "InsertTable.cpp" >}}

## Insert Table from HTML in Word Documents using C++ {#section3}

It is possible that an HTML file contains Table that you need to insert into your word documents like DOCX, DOC, etc. Or you may need to copy a table from a website. So instead of creating and designing the table from scratch, you can easily parse HTML markup as a table into word document. For example, you can add a table into word document using the following HTML string:

```
<table><tr><td>Row 1, Cell 1</td><td>Row 1, Cell 2</td></tr><tr><td>Row 2, Cell 1</td><td>Row 2, Cell 2</td></tr></table>
```

We have kept the contents simple so that the support for table tag can be demonstrated with basic yet important use case. Moreover, it is important to note here that AutoFit can not be applied on tables which are created from HTML.

Let us follow the steps below for inserting HTML table in Word document:

1.  Initialize an instance of [Document][16] class
2.  Pass the HTML markup with [InsertHtml][17] method
3.  Save output DOCX word file

Below code follows these steps and shows how to create table in Word document with HTML using C++:

{{< gist aspose-com-gists a1f0027243154dace264e8733fda2345 "InsertTableHTML.cpp" >}}

You can notice this method is a bit simpler than the approach we have explored above. The reason being, you do not need to add each node one by one for the rows, columns, or cells because the Table tag in the HTML string contains all information. Following is a screenshot of this simple HTML table added into the Word document:



{{< figure align=center src="images/Insert-Table-Word-cpp.png" alt="Insert Table in Word">}}


## Insert Table Using Document Builder in C++ {#section4}

The best thing about Aspose.Words for C++ API is that it offers a variety of features that become a competitive edge for the API and make it stand out among other options. Likewise, the feature of the inserting table using a document builder is another approach of adding tables in word documents (DOC/DOCX). So let us explore the details from three different perspectives:

### 1) Insert Simple Table in DOCX with Document Builder using C++ {#section5}

For adding a simple table in word document with Document builder, you need to follow the steps below:

1.  Create [Document][18] Object
2.  Call [StartTable()][19] method and insert cells
3.  Add the Row and Cells
4.  Save output DOCX file

Moreover, the code snippet below shows how to insert simple table in DOCX file with C++:

{{< gist aspose-com-gists a1f0027243154dace264e8733fda2345 "SimpleTableBuilder.cpp" >}}

### 2) Insert Formatted Table in DOCX with Document Builder using C++ {#section6}

You can insert a formatted table into a word document with the steps below:

1.  Initialize an instance of [Document][20] class
2.  Make Header Row
3.  Set indents and features for the formatting
4.  Reset Font formatting
5.  Save output Word DOCX file

Below code snippet creates formatted table in DOCX file using C++:

{{< gist aspose-com-gists a1f0027243154dace264e8733fda2345 "FormattedTableBuilder.cpp" >}}

### 3) Insert Nested Table in DOCX with Document Builder using C++ {#section7}

Sometimes we need another table inside an existing table. For instance, a cell in some row or column of a table can contain a sub-table for a sub-category or some other field. In such scenarios, Nested tables are helpful which can be added by following the steps below:

1.  Build outer [Table][21] and then call [EndTable][22] method
2.  Build inner Table inside a cell of outer table
3.  Save output word document

The following code snippet shows how to insert nested table in Word document using C++:

{{< gist aspose-com-gists a1f0027243154dace264e8733fda2345 "NestedTableBuilder.cpp" >}}

## Conclusion

To sum up, we have learned how to insert different tables in Word documents using different approaches. You can insert simple table or with HTML string as well as the formatted and nested tables into the word documents (DOC/DOCX). However, in case of any confusion or query, you can reach out to us at [Free Support Forums][23]. Moreover, you can also refer to [API References][24] and [Product Documentation][25] for your kind reference.

## See Also

[Add or Remove Header and Footer in Word Documents using Java][26]




[1]: https://docs.fileformat.com/word-processing/docx/
[2]: https://docs.fileformat.com/word-processing/doc/)
[3]: #section1
[4]: #section2
[5]: #section3
[6]: #section4
[7]: #section5
[8]: #section6
[9]: #section7
[10]: https://products.aspose.com/words/cpp
[11]: https://releases.aspose.com/
[12]: https://www.nuget.org/packages/Aspose.Words.Cpp/
[13]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[14]: https://apireference.aspose.com/words/cpp/class/aspose.words.tables.table
[15]: https://apireference.aspose.com/words/cpp/class/aspose.words.tables.table#a62836eef672e87165cfa56fe8463782e
[16]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[17]: https://apireference.aspose.com/words/cpp/class/aspose.words.document_builder#a72276df1da6f0ecae7b1ec3ff09df0b0
[18]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[19]: https://apireference.aspose.com/words/net/aspose.words/documentbuilder/methods/starttable
[20]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[21]: https://apireference.aspose.com/words/cpp/class/aspose.words.tables.table
[22]: https://apireference.aspose.com/words/net/aspose.words/documentbuilder/methods/endtable
[23]: https://forum.aspose.com/c/words/8
[24]: https://apireference.aspose.com/words/cpp
[25]: https://docs.aspose.com/words/cpp/
[26]: https://blog.aspose.com/2020/09/01/add-remove-header-footer-in-word-java/





