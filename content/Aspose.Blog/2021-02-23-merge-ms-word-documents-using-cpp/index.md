---
title: 'Merge MS Word Documents using C++'
seoTitle: "Merge MS Word Documents using C++ | Merge DOCX Files"
description: "Merge MS Word (DOC/DOCX) documents programmatically using C++. Merge multiple Word documents using additional options within your C++ applications."
date: Tue, 23 Feb 2021 10:59:08 +0000
draft: false
url: /2021/02/23/merge-ms-word-documents-using-cpp/
author: Muhammad Ahmad
summary: 'MS Word is a powerful tool that allows you to customize and format your professional documents with a fantastic set of features. You may find yourself in situations where you want to merge multiple Word documents, such as combining all the receipts in a single file or combining the different software requirement documents for easier management. Furthermore, combining the files simplifies the process of sharing them. In this article, you will learn **how to merge multiple MS Word documents using C++**.'
tags: ['C++ merge DOCX files', 'C++ merge word documents', 'merge multiple word documents using C++', 'merge two word documents using C++']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Merge-Word-Documents.jpg" alt="Merge Word Documents">}}


MS Word is a powerful tool that allows you to customize and format your professional documents with a fantastic set of features. You may find yourself in situations where you want to merge multiple Word documents, such as combining all the receipts in a single file or combining the different software requirement documents for easier management. Furthermore, combining the files simplifies the process of sharing them. In this article, you will learn **how to merge multiple MS Word documents using C++**.

*   [C++ API to Merge Word Documents][1]
*   [Combine Word Documents using C++][2]
*   [Merge Word Documents with Additional Options][3]
*   [Get a Free License][4]

## C++ API to Merge Word Documents {#CPP-API-to-Merge-Word-Documents}

[Aspose.Words for C++][5] is a native C++ library that allows you to create, change and convert Microsoft Word documents. In addition, it also supports combining multiple Word documents into a single file. You can either install the API through??[NuGet][6]??or download it directly from the??[Downloads][7]??section.

```
PM> Install-Package Aspose.Words.Cpp
```

## Merge Word Documents using C++ {#Merge-Word-Documents-using-CPP}

Merging Word documents with Aspose.Words for C++ API is a breeze. You can load and merge them with just a few lines of code. The following is the image showing the two sample Word files that we will combine in this article.



{{< figure align=center src="images/Sample1And2-1024x484.png" alt="Word documents to merge">}}


The following are the steps for merging Word documents using C++.

*   Load the destination document using the [Document][8] class.
*   Load the source document using the [Document][9] class.
*   Use the [Document->AppendDocument (System::SharedPtr<Aspose::Words::Document> srcDoc, Aspose::Words::ImportFormatMode importFormatMode)][10] method of the destination document instance to merge both documents.
*   Set the styling preference for importing the source document using the [ImportFormatMode][11] enum.
*   Save the merged Word document using [Document->Save (System::String fileName, Aspose::Words::SaveFormat saveFormat)][12] method.

The following is the sample code to merge Word documents.

{{< gist aspose-com-gists 869e1d9d88b432784acc2e7283fcb42b "Merge-Word-Documents.cpp" >}}

The following images compare the merged documents generated by using [](https://apireference.aspose.com/words/cpp/namespace/aspose.words#aafaa52cbf0baa49c3225787c23a8c949)[][13][ImportFormatMode][14]::KeepSourceFormatting and [](https://apireference.aspose.com/words/cpp/namespace/aspose.words#aafaa52cbf0baa49c3225787c23a8c949)[][15][ImportFormatMode][16]::UseDestinationStyles modes.



{{< figure align=center src="images/KeepSourceFormatting-1024x715.png" alt="Merged Word document generated using ImportFormatOptions::KeepSourceFormatting" caption="Output generated using **ImportFormatMode::KeepSourceFormatting**">}}




{{< figure align=center src="images/UseDestinationStyles-1024x718.png" alt="Merged Word document generated using ImportFormatOptions::UseDestinationStyles" caption="Output generated using **ImportFormatMode::UseDestinationStyles**">}}


## Merge Word Documents with Additional Options {#Merge-Word-Documents-with-Additional-Options}

Aspose.Words for C++ API provides the [ImportFormatOptions][17] class for customizing the merging of Word files. The following are the options provided by the [ImportFormatOptions][18] class.

*   **[IgnoreHeaderFooter][19]**: Specifies whether to ignore the formatting of headers/footers content when the??[](https://apireference.aspose.com/words/cpp/namespace/aspose.words#aafaa52cbf0baa49c3225787c23a8c949)[ImportFormatMode][20]::KeepSourceFormatting mode is used.
*   [**IgnoreTextBoxes**][21]: Specifies whether to ignore the source formatting of textboxes when the??[](https://apireference.aspose.com/words/cpp/namespace/aspose.words#aafaa52cbf0baa49c3225787c23a8c949)[ImportFormatMode][22]::KeepSourceFormatting mode is used.
*   [**KeepSourceNumbering**][23]: Specifies how to import the numbering when it conflicts in source and destination documents.
*   [**SmartStyleBehavior**][24]: Specifies how to import styles when they have the same names in source and destination documents.

The following are the steps to merge multiple Word documents with additional options:

*   Load the destination document using the [Document][25] class.
*   Load the source document using the [Document][26] class.
*   Create an instance of the [ImportFormatOptions][27] class and set the desired options.
*   Merge the documents using [Document->AppendDocument ( System::SharedPtr<Aspose::Words::Document> srcDoc, Aspose::Words::ImportFormatMode importFormatMode, System::SharedPtr<Aspose::Words::ImportFormatOptions> importFormatOptions)][28] method.
*   Save the destination Word document using [Document->Save (System::String fileName, Aspose::Words::SaveFormat saveFormat)][29] method.

The following is the sample code to merge Word documents with additional options.

{{< gist aspose-com-gists 869e1d9d88b432784acc2e7283fcb42b "Merge-Word-Documents-Customized.cpp" >}}

The following images compare the merged documents generated by setting the [IgnoreHeaderFooter][30] option to **true** and **false**.



{{< figure align=center src="images/IgnoreHeaderTrue-1024x720.png" alt="Merged Word document generated by setting the IgnoreHeaderFooter option to true" caption="Output generated by setting the **IgnoreHeaderFooter</strong> option to <strong>true**">}}




{{< figure align=center src="images/IgnoreHeaderFalse-1024x718.png" alt="Merged Word document generated by setting the IgnoreHeaderFooter option to false" caption="Output generated by setting the **IgnoreHeaderFooter</strong> option to <strong>false**">}}


## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting??[a free temporary license][31].

## Conclusion

In this article, you have learned how to merge multiple Word documents using C++. Furthermore, you have learned how to use additional options for customizing the merging of Word Files. Aspose.Words for C++ API provides a bunch of features for working with Word files. You can explore the API in detail by using the [official documentation][32]. If you have any questions, please feel free to contact us on the [forum][33].

## See Also

*   [Find and Replace Text in Word Documents using C++][34].




[1]: #CPP-API-to-Merge-Word-Documents
[2]: #Merge-Word-Documents-using-CPP
[3]: #Merge-Word-Documents-with-Additional-Options
[4]: #Get-a-Free-License
[5]: https://products.aspose.com/words/cpp
[6]: https://www.nuget.org/packages/Aspose.Words.Cpp
[7]: https://downloads.aspose.com/words/cpp
[8]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[9]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[10]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#aeb1c57b21244b7c3b4426c0ff6ca5e34
[11]: https://apireference.aspose.com/words/cpp/namespace/aspose.words#aafaa52cbf0baa49c3225787c23a8c949
[12]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a1355bc15bd6da23c7bf65f3fcf0fb050
[13]: https://apireference.aspose.com/words/cpp/namespace/aspose.words#aafaa52cbf0baa49c3225787c23a8c949a4cf454c612a2ed0c3ee75ac5175497c3
[14]: https://apireference.aspose.com/words/cpp/namespace/aspose.words#aafaa52cbf0baa49c3225787c23a8c949
[15]: https://apireference.aspose.com/words/cpp/namespace/aspose.words#aafaa52cbf0baa49c3225787c23a8c949a4cf454c612a2ed0c3ee75ac5175497c3
[16]: https://apireference.aspose.com/words/cpp/namespace/aspose.words#aafaa52cbf0baa49c3225787c23a8c949
[17]: https://apireference.aspose.com/words/cpp/class/aspose.words.import_format_options
[18]: https://apireference.aspose.com/words/cpp/class/aspose.words.import_format_options
[19]: https://apireference.aspose.com/words/cpp/class/aspose.words.import_format_options#a4310f7f3e1d5cee6e0327b699f3f3fa6
[20]: https://apireference.aspose.com/words/cpp/namespace/aspose.words#aafaa52cbf0baa49c3225787c23a8c949
[21]: https://apireference.aspose.com/words/cpp/class/aspose.words.import_format_options#a5d7712f203541e78dba2dedc350d27b1
[22]: https://apireference.aspose.com/words/cpp/namespace/aspose.words#aafaa52cbf0baa49c3225787c23a8c949
[23]: https://apireference.aspose.com/words/cpp/class/aspose.words.import_format_options#ac12ec2b07306b8d9aa3d3ee1983096cf
[24]: https://apireference.aspose.com/words/cpp/class/aspose.words.import_format_options#a1eef86cf3e6a8fdbbd33f6fafcc23e73
[25]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[26]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[27]: https://apireference.aspose.com/words/cpp/class/aspose.words.import_format_options
[28]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a7b09f54d466b74ee498156e848b9ba86
[29]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a1355bc15bd6da23c7bf65f3fcf0fb050
[30]: https://apireference.aspose.com/words/cpp/class/aspose.words.import_format_options#a4310f7f3e1d5cee6e0327b699f3f3fa6
[31]: https://purchase.aspose.com/temporary-license
[32]: https://docs.aspose.com/words/cpp/
[33]: https://forum.aspose.com/c/words/8
[34]: https://blog.aspose.com/2021/01/12/Find-and-Replace-Text-in-Word-Documents-using-CPP/





