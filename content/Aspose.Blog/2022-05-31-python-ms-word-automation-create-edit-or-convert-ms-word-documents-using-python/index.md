---
title: 'Python MS Word Automation – Create, Edit, or Convert Word Documents using Python'
seoTitle: "MS Word Automation in Python | Python MS Word Automation"
description: "Python MS Word Automation. Create Word documents in Python. Edit or modify, parse, and convert Word DOC/DOCX documents using Aspose.Words for Python API."
date: Tue, 31 May 2022 11:50:42 +0000
draft: false
url: /2022/05/31/python-ms-word-automation-create-edit-or-convert-ms-word-documents-using-python/
author: Muzammil Khan
summary: 'As a Python developer, you can automate MS Word to create new Word documents, edit or modify the existing ones, parse or convert them into other formats without using Microsoft Office. In this article, you will learn **how to automate MS Word to create, edit, parse or convert Word documents using Python**.'
tags: ['Automate Word Document with Python', 'Convert Word Document using Python', 'Create Word Document using Python', 'DOCX', 'DOCX Python', 'Edit Word Document in Python', 'Extract Text from DOCX in Python', 'MS Word Automation in Python', 'Parse Word Document in Python', 'Parsing Word Documents with Python', 'Python Convert Word Document', 'Python Create Word Document', 'Python Edit Word Document', 'Python MS Word Automation', 'Python Word', 'Python Word Document Parser', 'Python Word Library']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/python-word-automation-create-edit-or-convert-ms-word-documents-using-python.jpg" alt="Python Word Automation ">}}


We can automate MS Word to create new Word documents ([DOC][1] or [DOCX][2], edit or modify the existing ones, or convert them into other formats without using Microsoft Office. Python MS Word automation allows performing all the actions programmatically that we can perform through the user interface of MS Word. In this article, we will learn **how to automate MS Word to create, edit, or convert Word documents using Python**.

This article covers all the basic features required for generating and manipulating Word documents programmatically using Python. This article includes the following topics:

*   [Python MS Word Automation API to Create, Edit, or Convert Word Documents][3]
*   [Create Word Documents][4]
*   [Edit or Modify Word Documents][5]
*   [Find and Replace Text in Word Documents][6]
*   [Convert Word Documents][7]
*   [Parse Word Documents][8]

## Python MS Word Automation API to Create, Edit, or Convert Word Documents {#Python-MS-Word-Automation-API-to-Create-Edit-or-Convert-Word-Documents}

For automating Word, we will be using [Aspose.Words for Python][9] API. It is a complete and feature-rich Word automation solution to create, edit, or analyze Word documents programmatically. The _Document_ class of the API represents a Word document. The API provides the _DocumentBuilder_ class that offers various methods to insert text, images, and other content in the document. This class also allows specifying the font, paragraph, and section formatting. The _Run_ class of the API represents a run of characters with the same font formatting. Please install the library in your Python application from [PyPI][10] using the following pip command.

```
pip install aspose-words
```

## Create Word Documents using Python {#Create-Word-Documents-using-Python}

We can create Word documents programmatically by following the steps given below:

*   Firstly, create an instance of the **_Document_** class.
*   Next, create an instance of the **_DocumentBuilder_** class with the Document object as an argument.
*   After that, insert/write elements to add some text, paragraphs, tables, or images using the **_DocumentBuilder_** object.
*   Finally, call the **_save()_** method with the output file path as an argument to save the created file.

The following code sample shows **how to create a Word document (DOCX) using Python**.

{{< gist aspose-com-gists bcb11fd8e7050e31f052037012c38864 "Python-MS-Word-Automation_Create.py" >}}



{{< figure align=center src="images/Create-Word-Documents-using-Python.jpg" alt="Create Word Documents" caption="Create Word Documents using Python.">}}


## Edit or Modify Word Documents using Python {#Edit-or-Modify-Word-Documents-using-Python}

In the previous section, we created a Word document. Now, let’s edit it and change the content of the document. We can edit Word documents by following the steps given below:

*   Firstly, load an existing Word document using the **_Document_** class.
*   Next, access the specific section by its index.
*   Then, access the first paragraph content as an object of the **_Run_** class.
*   After that, set the text to update for the accessed paragraph.
*   Finally, call the **_save()_** method with the output file path to save the updated file.

The following code sample shows **how to edit a Word document (DOCX) using Python**.

{{< gist aspose-com-gists bcb11fd8e7050e31f052037012c38864 "Python-MS-Word-Automation_Edit.py" >}}



{{< figure align=center src="images/Edit-or-Modify-Word-Documents-using-Python-1024x576.jpg" alt="Edit or Modify Word Documents " caption="Edit or Modify Word Documents using Python.">}}


## Find and Replace Text in Word Documents using Python {#Find-and-Replace-Text-in-Word-Documents-using-Python}

We can also find any text and replace it with a new text by following the steps given below:

*   Firstly, load a Word document using the **_Document_** class.
*   Next, create an instance of the **_FindReplaceOptions_** class.
*   After that, call the **_replace()_** method. It takes the search string, the replace string, and the **_FindReplaceOptions_** object as arguments.
*   Finally, call the **_save()_** method with the output file path to save the updated file.

The following code sample shows **how to find and replace specific text in a Word document (DOCX) using Python**.

{{< gist aspose-com-gists bcb11fd8e7050e31f052037012c38864 "Python-MS-Word-Automation_FindReplace.py" >}}



{{< figure align=center src="images/Find-and-Replace-Text-in-Word-Documents-using-Python-1024x576.jpg" alt="Find and Replace Text in Word Documents" caption="Find and Replace Text in Word Documents.">}}


## Convert Word Documents using Python {#Convert-Word-Documents-using-Python}

We can convert Word documents to other formats such as PDF, XPS, EPUB, HTML, JPG, PNG, etc. Please follow the steps given below to convert a Word document to an HTML web page:

*   Firstly, load a Word document using the **_Document_** class.
*   Next, create an instance of the **_HtmlSaveOptions_** class with the _Document _object as an argument.
*   After that, specify the css\_style\_sheet\_type, export\_font\_resources, resource\_folder, and alias properties.
*   Finally, call the **_save()_** method with the output file path and **_**_HtmlSaveOptions_**_** object as arguments to save the converted HTML file.

The following code sample shows **how to convert a Word document (DOCX) to HTML using Python**.

{{< gist aspose-com-gists bcb11fd8e7050e31f052037012c38864 "Python-MS-Word-Automation_Convert.py" >}}



{{< figure align=center src="images/Convert-Word-Documents-using-Python-1-1024x576.jpg" alt="" caption="Convert Word Documents using Python.">}}


Similarly, we can also convert Word documents to other supported formats. Please read more about how to convert [Word to EPUB][11], [Word to PDF][12], [Word document to Markdown][13], [Word to JPG, or PNG images][14] in the documentation.

## Parse Word Documents using Python {#Parse-Word-Documents-using-Python}

We can parse Word documents and extract the content as plain text by following the steps given below:

*   Firstly, load a Word document using the **_Document_** class.
*   Next, extract and print the text.
*   Finally, call the **_save()_** method to save the Word document as a text file. This method takes the path of the output file as an argument.

The following code sample shows **how to parse a Word document (DOCX) using Python**.

{{< gist aspose-com-gists bcb11fd8e7050e31f052037012c38864 "Python-MS-Word-Automation_Parse.py" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][15] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   automate MS Word using Python;
*   create and edit Word documents programmatically;
*   parse or convert DOCX files;
*   find and replace text in Word documents using Python.

Besides, you can learn more about **_Aspose.Words for Python_** API using the [documentation][16]. In case of any ambiguity, please feel free to contact us on the [forum][17].

## See Also

*   [Extract Text from Word DOCX DOC in Python][18]
*   [Create Table in Word DOCX in Python][19]
*   [Extract Images from Word Documents in Python][20]
*   [Convert a Word Document to EPUB in Python][21]
*   [Split a Word DOCX DOC in Python][22]
*   [Automate MS Word Mail Merge in Python][23]
*   [Combine Word Documents using Python][24]




[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/word-processing/docx/)
[3]: #Python-MS-Word-Automation-API-to-Create-Edit-or-Convert-Word-Documents
[4]: #Create-Word-Documents-using-Python
[5]: #Edit-or-Modify-Word-Documents-using-Python
[6]: #Find-and-Replace-Text-in-Word-Documents-using-Python
[7]: #Convert-Word-Documents-using-Python
[8]: #Parse-Word-Documents-using-Python
[9]: https://products.aspose.com/words/python-net/
[10]: https://pypi.org/project/aspose-words/
[11]: https://docs.aspose.com/words/python-net/convert-a-document-to-html-mhtml-or-epub/
[12]: https://docs.aspose.com/words/python-net/convert-a-document-to-pdf/
[13]: https://docs.aspose.com/words/python-net/convert-a-document-to-markdown/
[14]: https://docs.aspose.com/words/python-net/convert-a-document-to-an-image/
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/words/net/
[17]: https://forum.aspose.com/c/words
[18]: https://blog.aspose.com/2021/11/25/extract-text-from-word-docx-in-python/
[19]: https://blog.aspose.com/2021/11/22/create-table-in-word-using-python/
[20]: https://blog.aspose.com/2021/11/19/extract-images-from-word-in-python/
[21]: https://blog.aspose.com/2021/11/19/convert-word-to-epub-in-python/
[22]: https://blog.aspose.com/2021/11/18/split-a-word-document-in-python/
[23]: https://blog.aspose.com/2021/11/17/automate-ms-word-mail-merge-in-python/
[24]: https://blog.aspose.com/2021/11/12/combine-word-documents-using-python/




