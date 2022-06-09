---
title: 'Make Fillable Form in Word | Insert, Delete Check Boxes &amp; Fields in C#'
seoTitle: ""
description: ""
date: Wed, 05 Aug 2020 12:02:18 +0000
draft: false
url: /2020/08/05/make-fillable-form-in-word-insert-delete-check-boxes-fields-in-c/
author: Farhan Raza
summary: ''
tags: ['Insert check box in DOCX', 'Insert text box in DOCX csharp', 'fillable form fields in DOCX', 'fillable form in word', 'fillable form in word csharp']
categories: ['Aspose.Words Product Family']
---

Fillable Forms are frequently used in Microsoft Word Documents like [DOC][1], [DOCX][2], and other file formats. In this article, we will create a fillable form in Word document programmatically using C# with [Aspose.Words for .NET][3] API. Moreover, we will also cover removing or deleting fillable form fields.

## Installation

You can configure Aspose.Words for .NET API in your .NET application and subsequently use it with C# or VB.NET. You can either download the DLL from the [New Releases][4] section or configure it using following NuGet command.

_PM> Install-Package Aspose.Words -Version 20.8.0_

Moreover, you can also install the API using NuGet Manager for Solution tool in Visual Studio, as shown in the screenshot below:



{{< figure align=center src="images/Fillable-Form.png" alt="Make fillable form in word">}}


So the API has been configured at this step. Let us proceed to learn the following use cases:

*   [Create fillable form fields with Check box, Text box in Word using C#][5]
*   [Delete a fillable form field from a Word Document using C#][6]

## Create Fillable Form Fields with Check box, Text box in Word using C# {#section1}

You can create or insert check boxes in word document easily with few basic steps. In addition to the check box, we will also explore how to add text box and combo box. Following are the steps for inserting or adding check box, text box, and combo box in a DOCX file.

1.  Initialize a new Word document
2.  Insert Text form field with [InsertTextInput][7] method
3.  Insert check box field using [InsertCheckBox][8] method
4.  Insert combo box field with [InsertComboBox][9] method
5.  Save output word file

The code snippet below shows how to insert fillable field like check box, text box, and combo box in Word files (DOC/DOCX) in C#:

{{< gist aspose-com-gists 24247a0021776683e8ccd22ddb0ea53c "check-boxes-in-word.cs" >}}

Furthermore, Aspose.Words for .NET API is a feature-rich API that lets you set many properties of the form fields. For example, FormField class can be used to set size, default value, entry and exit macros, etc.

## Delete a Fillable Form Field in a Word Document using C# {#section2}

Adding a fillable form field and deleting a fillable form field are the most important and frequently used features with reference to forms in word files. Now, let us take a look at how a fillable form field can be deleted using C# in your .NET applications. You can follow the following steps to delete a field:

1.  Load input word file using [Document][10] class
2.  Get specific fillable form field by its name
3.  Call [Remove][11] method
4.  Save output word file

The following code snippet is based on these steps which shows how to delete a fillable form field from word document with C#:

{{< gist aspose-com-gists 24247a0021776683e8ccd22ddb0ea53c "delete-fillable-form-field.cs" >}}

## Conclusion

Concludingly, we have learned how to make or create fillable form fields in DOCX, or ord files. Moreover, we have also checked out how to delete or remove a form field from a word document. In case of any confusion, doubt, or query, you please write to us at [Free Support Forum][12]. We would love to assist you!

## See Also

[Word Document (DOC/DOCX) to HTML Conversion][13]




[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: https://products.aspose.com/words/net
[4]: https://releases.aspose.com/
[5]: #section1
[6]: #section2
[7]: https://apireference.aspose.com/words/net/aspose.words/documentbuilder/methods/inserttextinput
[8]: https://apireference.aspose.com/words/net/aspose.words/documentbuilder/methods/insertcheckbox/index
[9]: https://apireference.aspose.com/words/net/aspose.words/documentbuilder/methods/insertcombobox
[10]: https://apireference.aspose.com/words/net/aspose.words/document
[11]: https://apireference.aspose.com/words/net/aspose.words/node/methods/remove
[12]: https://forum.aspose.com/c/words
[13]: https://blog.aspose.com/2020/07/15/word-document-doc-docx-to-html-conversion-using-java/





