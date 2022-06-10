---
title: 'Copy Macros from One Word Document to Other in Java'
date: Fri, 27 Dec 2019 16:46:18 +0000
draft: false
url: /2019/12/27/copy-word-macro-from-one-document-to-other-aspose-words-for-java/
author: Usman Aziz
summary: ''
tags: ['Aspose.Words for Java', 'Copy VBA Macro', 'Copy VBA Macro in Java', 'Copy VBA Module', 'Copy VBA Project', 'Copy Word Macro', 'Copy Word Macro in Java', 'VBA Macro', 'VBA Macro in Word', 'Word Macro']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-Java.png" alt="Copy Word macros in Java using Aspose.Words">}}


Another month, another feature-rich release! [Aspose.Words for Java 19.12][1] has been rolled out with a bunch of useful features, enhancements and bug fixes. Using the latest release you will be able to copy Word macros from one document to another by cloning the VBA module or the VBA project in Java. Furthermore, we have added the support of PDF 1.7 Standard for Word to PDF conversion. Also, the latest release of _Aspose.Words for Java_ is capable of scanning user-installed fonts in Windows 10 for the font source. So let's go through these useful features in more detail.

## Copy VBA Macros from One Word Document to Other in Java

Macros in a Word document are written in VBA (Visual Basic for Applications) to automate the frequently used tasks. MS Word macros contain a set of code statements that are executed when a particular button in the toolbar is clicked or a combination of keys is pressed.

In the [previous release][2] of _Aspose.Words for Java_, we introduced the feature of adding macros to VBA project or VBA modules in the Word documents. However, there could be the case when you need to clone VBA modules or the whole VBA project to copy Word macros from one document to another programmatically. In order to make it possible, we have added _deepClone()_ method to [VABModule][3] and [VBAProject][4] classes to copy Word macros from a particular VBA module or project.

Let's now check out how to copy Word macros from one document to another in Java using _Aspose.Words for Java_.

### Cloning VBA Module

The following Java code sample shows how to copy macros by cloning a particular VBA module in Word document.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithVbaMacros-CloneVbaModule.java" >}}

### Cloning VBA Project

The following Java code sample shows how to copy macros by cloning a complete VBA project in Word document.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithVbaMacros-CloneVbaProject.java" >}}

## Convert Word to PDF 1.7 Standard in Java

A PDF document may compliant with various standards or editions of PDF specifications. PDF 1.7 was the sixth edition of the PDF specification and it included some proprietary technologies which are defined only by Adobe. _Aspose.Words for Java_ already supports [Word to PDF conversion][5], however, we have extended this support and now you can convert a Word document to PDF 1.7. For this, we have added the [PDF\_17][6] option to the [PdfCompliance][7] enum.

The following Java code sample shows how to convert Word to PDF by specifying _PdfCompliance_.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-rendering_printing-WorkingWithPdfSaveOptions-ConversionToPDF17.java" >}}

## Using User-Installed Fonts for SystemFontSource on Windows 10

In the previous versions of the _Aspose.Words for Java_, the API used to scan only the system-installed fonts for [SystemFontSource][8]. This approach didn't fit well in Windows 10 where the fonts may be installed either into the system folder "_%windir%\\fonts_" for all users or into the user folder "_%userprofile%\\AppData\\Local\\Microsoft\\Windows\\Fonts_" for the current user. We have enhanced this feature and now _Aspose.Words for Java_ has the ability to scan the user-installed fonts as well.

## New Find and Replace Option {#Aspose.WordsforJava19.12ReleaseNotes-AddedanewFindReplaceOptions.UseLegacyOrderoption}

_Aspose.Words for Java_ provides [Find and Replace][9] option to replace the desired words or phrases in the Word documents. In the previous versions of the API, the find/replace feature used to analyze the text boxes separately from the content of the document. This behavior was designed in accordance with the MS Word's behavior, however, there could be the case when you may need to find and replace content sequentially including the text in the text boxes. For such a scenario, we have introduced a new option in [FindReplaceOptions][10] class as _UseLegacyOrder_. The following Java code sample shows how to use this option when finding and replacing text in a Word document.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-find_replace-UsingLegacyOrder-FineReplaceUsingLegacyOrder.java" >}}

Well, this was a brief overview of some of the important features we have added to the latest release. You can have a look at the complete list of features and bug fixes in the [release notes][11]. You can [download][12] the latest release and evaluate the new features by yourself. For more details about any feature, you may consult the [documentation][13] of the API as well as contact us via our [forum][14].




[1]: https://downloads.aspose.com/words/java
[2]: https://blog.aspose.com/2019/11/16/aspose-words-for-java-19-11-released/
[3]: https://apireference.aspose.com/java/words/com.aspose.words/vbamodule
[4]: https://apireference.aspose.com/java/words/com.aspose.words/vbaproject
[5]: https://docs.aspose.com/display/wordsjava/Converting+a+Microsoft+Word+document+using+save+Method#ConvertingaMicrosoftWorddocumentusingsaveMethod-ConvertaDocumenttoPDF
[6]: https://apireference.aspose.com/java/words/com.aspose.words/pdfcompliance#PDF_17
[7]: https://apireference.aspose.com/java/words/com.aspose.words/pdfcompliance
[8]: https://apireference.aspose.com/java/words/com.aspose.words/SystemFontSource
[9]: https://docs.aspose.com/display/wordsjava/Find+and+Replace
[10]: https://apireference.aspose.com/java/words/com.aspose.words/FindReplaceOptions
[11]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+19.12+Release+Notes
[12]: https://downloads.aspose.com/words/java
[13]: https://docs.aspose.com/display/wordsjava/Getting+Started
[14]: https://forum.aspose.com/c/words




