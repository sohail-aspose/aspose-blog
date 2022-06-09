---
title: 'Work with VBA Macros in Word Documents using Python'
seoTitle: "Python: Create, Modify, Clone VBA Macro in Word Documents"
description: "Use Python Word library to create VBA macro in Word documents in Python. Modify and clone VBA modules or projects in Word documents dynamically."
date: Tue, 23 Nov 2021 15:52:15 +0000
draft: false
url: /2021/11/23/work-with-vba-macro-in-word-using-python/
author: Usman Aziz
summary: '[Visual Basic for Applications (VBA)][1] is a powerful programming language that lets you automate tasks in Word documents. Moreover, you can perform repetitive tasks with VBA macros quite easily. In this article, you will learn how to work with VBA projects and modules in MS Word documents. Particularly, the article will cover **how to create, modify and clone VBA macros programmatically in Python**.'
tags: ['clone vba macro in word using python', 'create vba macro in word using python', 'manipulate vba macro in word using python', 'modify vba macro in word using python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/work-with-VBA-macro-in-Word-documents.jpg" alt="Work with VBA Macros in Word Documents using Python">}}


[Visual Basic for Applications (VBA)][2] is a powerful programming language that lets you automate tasks in Word documents. Moreover, you can perform repetitive tasks with VBA macros quite easily. In this article, you will learn how to work with VBA projects and modules in MS Word documents. Particularly, the article will cover **how to create, modify and clone VBA macros programmatically in Python**.

*   [Python Library to Work with MS Word VBA Macros][3]
*   [Create VBA Macro in an MS Word Document][4]
*   [Modify VBA Macro in a Word Document][5]
*   [Clone VBA Macro in a Word Document][6]

**Info**: If you ever need to get a Word document from a PowerPoint presentation, you can use Aspose [Presentation to Word Document][7] converter.

## Python Library to Work with MS Word VBA Macros {#Python-Library-to-Work-with-MS-Word-VBA-Macros}

To work with VBA Macros in Word files, we will use [Aspose.Words for Python][8]. It is a powerful library for creating and manipulating Word documents from within Python applications. You can install the library in your application from [PyPI][9] using the following pip command.

```
pip install aspose-words
```

## Create VBA Macro in an MS Word Document in Python {#Create-VBA-Macro-in-MS-Word-Document}

The following are the steps to create a VBA macro in an MS Word DOCM file using Python.

*   Load the Word document or create a new one using _Document_ class.
*   Create an object of _VbaProject_ class.
*   Set name of the project using _VbaProject.name_ property.
*   Assign project to _Document.vba\_project_ property.
*   Create an object of _VbaModule_ class.
*   Set name and type of module using _VbaModule.name_ and _VbaModule.type_ properties, respectively.
*   Set source code using _VbaModule.source\_code_ property.
*   Add module to the VBA project of the document using _Document.vba\_project.modules.add(VbaModule)_ method.
*   Save the document using _Document.save()_ method.

The following code sample shows how to create a VBA macro in a DOCM document using Python.

{{< gist aspose-com-gists 2322b84d38b01cbc8f3b7f57bf2a2a7f "create-vba-macro-in-word.py" >}}

## Modify VBA Macro in a Word Document in Python {#Modify-VBA-Macro-in-a-Word-Document}

You can also access and modify the existing VBA macros in Word documents seamlessly. The following steps demonstrate how to achieve this using Aspose.Words for Python.

*   Load the Word document using _Document_ class.
*   Get reference of the _VbaProject_ into an object using _Document.vba\_project_ property.
*   Access the desired VBA module using index and update its source code using _VbaProject.modules\[int\].source\_code_ property.
*   Save the document using _Document.save()_ method.

The following code sample shows how to modify an existing MS Word VBA macro using Python.

{{< gist aspose-com-gists 2322b84d38b01cbc8f3b7f57bf2a2a7f "modify-vba-macro-in-word.py" >}}

## Clone VBA Macro in a Word Document using Python {#Clone-VBA-Macro-in-a-Word-Document}

In certain cases, you may need to clone a VBA module or the whole VBA project from one Word document to another. To achieve this, Aspose.Words for Python allows you to create clones quite easily. The following sections cover how to clone a VBA module or a VBA project.

### Clone a VBA Module

The following are the steps to create a clone of a VBA module from one DOCM document to another using Python.

*   Load the source Word document using _Document_ class.
*   Load the destination Word document using _Document_ class.
*   Create a _VbaProject_ for destination Word document.
*   Get clone of VBA module from source Word document into an object using _Document.vba\_project.modules.get\_by\_name(string).clone()_ method.
*   Add the cloned module into destination document using _Document.vba\_project.modules.add(VbaModule)_ method.
*   Save the destination document using _Document.save()_ method.

The following code sample shows how to clone an MS Word VBA module in Python.

{{< gist aspose-com-gists 2322b84d38b01cbc8f3b7f57bf2a2a7f "clone-vba-module-in-word.py" >}}

### Clone a VBA Project

The following are the steps to clone an MS Word VBA project in Python.

*   Load the source Word document using _Document_ class.
*   Load the destination Word document using _Document_ class.
*   Get clone of VBA project from source document using _Document.vba\_project.clone()_ method and add it to destination document using _Document.vba\_project_ property.
*   Save the destination document using _Document.save()_ method.

The following code sample shows how to clone a VBA project from one Word document to another in Python.

{{< gist aspose-com-gists 2322b84d38b01cbc8f3b7f57bf2a2a7f "clone-vba-project-in-word.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [temporary license][10] to use Aspose.Words for Python without evaluation limitations.

## Conclusion

In this article, you have learned how to create VBA macros in MS Word documents using Python. Moreover, you have seen how to modify or clone existing VBA modules or projects programmatically. In addition, you can explore other features of Aspose.Words for Python using the [documentation][11]. In case you would have any questions, feel free to let us know via our [forum][12].

## See Also

*   [Create MS Word Documents using Python][13]
*   [Convert Word Document to HTML using Python][14]
*   [Convert Word Documents to PNG, JPEG, or BMP in Python][15]
*   [Word Documents to Markdown using Python][16]
*   [Compare Two Word Documents in Python][17]




[1]: https://en.wikipedia.org/wiki/Visual_Basic_for_Applications
[2]: https://en.wikipedia.org/wiki/Visual_Basic_for_Applications
[3]: #Python-Library-to-Work-with-MS-Word-VBA-Macros
[4]: #Create-VBA-Macro-in-MS-Word-Document
[5]: #Modify-VBA-Macro-in-a-Word-Document
[6]: #Clone-VBA-Macro-in-a-Word-Document
[7]: https://products.aspose.app/slides/conversion/ppt-to-word
[8]: https://products.aspose.com/words/python/
[9]: https://pypi.org/project/aspose-words/
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/words/python/product-overview/
[12]: https://forum.aspose.com/
[13]: https://blog.aspose.com/2021/10/28/create-word-documents-using-python/
[14]: https://blog.aspose.com/2021/11/01/convert-word-to-html-in-python/
[15]: https://blog.aspose.com/2021/11/04/convert-word-to-png-jpg-bmp-in-python/
[16]: https://blog.aspose.com/2021/11/05/convert-word-to-markdown-using-python/
[17]: https://blog.aspose.com/2021/11/11/compare-two-word-documents-in-python/




