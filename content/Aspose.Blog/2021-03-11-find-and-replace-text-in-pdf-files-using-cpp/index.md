---
title: 'Find and Replace Text in PDF Files using C++'
seoTitle: "Find and Replace Text in PDF Files using C++ | Replace Text using Regex"
description: "Find and replace text in PDF documents using C++. Find and replace text in the whole PDF, particular page, or page region. You can also search using Regex."
date: Thu, 11 Mar 2021 09:27:01 +0000
draft: false
url: /2021/03/11/find-and-replace-text-in-pdf-files-using-cpp/
author: Muhammad Ahmad
summary: '[PDF][1] is a popular format that is widely used for sharing documents between organizations and individuals. There might be scenarios where you have to find and replace some text in the PDF documents before sharing. You can do this manually, but that would take more time and be less efficient. The better and faster option would be to do this programmatically. In this article, you will learn **how to find and replace text in PDF files using C++**.'
tags: ['find and replace text in PDF using C++', 'find and replace text in pdf using regex', 'find text in whole PDF document C++']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Find-and-Replace-Text-in-PDF.jpg" alt="Find and Replace Text in PDF using C++">}}


[PDF][2] is a popular format that is widely used for sharing documents between organizations and individuals. There might be scenarios where you have to find and replace some text in the PDF documents before sharing. You can do this manually, but that would take more time and be less efficient. The better and faster option would be to do this programmatically. In this article, you will learn **how to find and replace text in PDF files using [C++][3]**.

*   [C++ API to Find and Replace Text in PDF files][4]
*   [Find and Replace Text in PDF using C++][5]
*   [C++ Find and Replace Text in a Specific PDF Page][6]
*   [Replace Text in PDF Page Region using C++][7]
*   [Find and Replace Text in PDF files using Regular Expressions][8]
*   [Get a Free License][9]

## C++ API to Find and Replace Text in PDF files {#CPP-API-to-Find-and-Replace-Text-in-PDF-files}

[Aspose.PDF for C++][10] is a C++ library for working with PDF files. It provides a bunch of features that help you automate various aspects of your PDF workflows. One such feature is finding and replacing text in PDF files. You can either install the API through [NuGet][11] or download it directly from the [downloads][12] section.

```
PM> Install-Package Aspose.PDF.Cpp
```

## Find and Replace Text in PDF using C++ {#Find-and-Replace-Text-in-PDF-using-CPP}

Aspose.PDF for C++ provides the [TextFragmentAbsorber][13] class for searching text in PDF documents. You initialize this class with the text you want to find and use it to retrieve all the matching text fragments. Once all the fragments are available, you loop over them and replace the text. The following are the steps to find and replace text in PDF files using C++.

*   Load the PDF file using the [Document][14] class.
*   Create an instance of the [TextFragmentAbsorber][15] class and initialize it with the text that you want to find in the PDF file.
*   Accept the [TextFragmentAbsorber][16] for the pages using the [Document->get\_Pages()->Accept (System::SharedPtr<Text::TextFragmentAbsorber> visitor)][17] method.
*   Retrieve all text occurrences using the [TextFragmentAbsorber->get\_TextFragments()][18] method.
*   Loop through the [TextFragmentCollection][19] and update the text using the [TextFragment->set\_Text (System::String value)][20] method.
*   Save the updated PDF file using the [Document->Save (System::String outputFileName)][21] method.

The following is the sample code to find and replace text in the whole PDF file using C++.

{{< gist aspose-com-gists d77cf182b00b4674ec702a7e50e0302a "Find-And-Replace-Text-In-PDF-Files.cpp" >}}

## C++ Find and Replace Text in a Specific PDF Page {#CPP-Find-and-Replace-Text-in-a-Specific-PDF-Page}

There might be situations where you only want to find and replace text on a specific page rather than the whole document. For this, accept the [TextFragmentAbsorber][22] object for the page where you want to replace the text. The following are the steps to find and replace text on a particular page in the PDF document.

*   Load the PDF file using the [Document][23] class.
*   Create an instance of the [TextFragmentAbsorber][24] class and initialize it with the text that you want to find in the PDF file.
*   Accept the [TextFragmentAbsorber][25] for the particular page using the [Document->get\_Pages()->idx\_get (int32\_t index)->Accept (System::SharedPtr<Text::TextFragmentAbsorber> visitor)][26] method.
*   Retrieve all text occurrences using the [TextFragmentAbsorber->get\_TextFragments()][27] method.
*   Loop through the [TextFragmentCollection][28] and update the text using the [TextFragment->set\_Text (System::String value)][29] method.
*   Save the updated PDF file using the [Document->Save (System::String outputFileName)][30] method.

The following is the sample code to find and replace text on a specific PDF page using C++.

{{< gist aspose-com-gists d77cf182b00b4674ec702a7e50e0302a "Find-And-Replace-Text-In-PDF-Page.cpp" >}}

## Replace Text in PDF Page Region using C++ {#Replace-Text-in-PDF-Page-Region-using-CPP}

Instead of searching the whole page, you can specify the region of the page where you want to replace the text. For this, the API provides the [Rectangle][31] class. The following are the steps to find and replace text in a specific part of the PDF page.

*   Load the PDF file using the [Document][32] class.
*   Create an instance of the [TextFragmentAbsorber][33] class and initialize it with the text that you want to find and replace in the PDF file.
*   Set the page region for searching using [TextFragmentAbsorber->get\_TextSearchOptions()->set\_Rectangle (System::SharedPtr< Aspose::Pdf::Rectangle > value)][34] method.
*   Accept the [TextFragmentAbsorber][35] for the particular page using the [Document->get\_Pages()->idx\_get (int32\_t index)->Accept (System::SharedPtr<Text::TextFragmentAbsorber> visitor)][36] method.
*   Retrieve all text occurrences using the [TextFragmentAbsorber->get\_TextFragments()][37] method.
*   Loop through the [TextFragmentCollection][38] and update the text using the [TextFragment->set\_Text (System::String value)][39] method.
*   Save the updated PDF file using the [Document->Save (System::String outputFileName)][40] method.

The following is the sample code to find and replace text in a specific PDF page region.

{{< gist aspose-com-gists d77cf182b00b4674ec702a7e50e0302a "Find-And-Replace-Text-In-PDF-Page-Region.cpp" >}}

## Find and Replace Text in PDF files using Regular Expressions {#Find-and-Replace-Text-in-PDF-files-using-Regular-Expressions}

Aspose.PDF for C++ also provides the ability to search text using regular expressions. With regular expressions, you can find text like email addresses or phone numbers, etc. For this, you have to specify the regular expression instead of the search string and use the [TextSearchOptions][41] class to indicate that you are using a regular expression for searching. The following are the steps to find and replace text in PDF files using a regular expression.

*   Load the PDF file using the [Document][42] class.
*   Create an instance of the [TextFragmentAbsorber][43] class and initialize it with the regular expression you want to use.
*   Initialize the [TextSearchOptions][44] class and pass _true_ to its constructor. It will indicate that you are searching using a regular expression.
*   Assign the [TextSearchOptions][45] object to the [TextFragmentAbsorber][46] class using [TextFragmentAbsorber->set\_TextSearchOptions (System::SharedPtr<Aspose::Pdf::Text::TextSearchOptions> value)][47] method.
*   Accept the [TextFragmentAbsorber][48] for the pages using the [Document->get\_Pages()->Accept (System::SharedPtr<Text::TextFragmentAbsorber> visitor)][49] method.
*   Retrieve all text occurrences using the [TextFragmentAbsorber->get\_TextFragments()][50] method.
*   Loop through the [TextFragmentCollection][51] and update the text using the [TextFragment->set\_Text (System::String value)][52] method.
*   Save the updated PDF file using the [Document->Save (System::String outputFileName)][53] method.

The following is the sample code to find and replace text in PDF files using a regular expression.

{{< gist aspose-com-gists d77cf182b00b4674ec702a7e50e0302a "Find-And-Replace-Text-In-PDF-Regex.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][54].

## Conclusion

In this article, you have learned how to find and replace text in PDF files using C++. You have seen how to replace text in the whole PDF document, a specific PDF page, or a particular region of the page. Furthermore, you have learned how to search and replace text using a regular expression. Aspose.PDF for C++ is a powerful API with many additional features that make working with PDF documents a piece of cake. You can explore the API in detail by using the [official documentation][55]. If you have any questions, please feel free to contact us on the [forum][56].

## See Also

*   [Convert PDF to SVG Format using C++][57]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/programming/cpp/
[4]: #CPP-API-to-Find-and-Replace-Text-in-PDF-files
[5]: #Find-and-Replace-Text-in-PDF-using-CPP
[6]: #CPP-Find-and-Replace-Text-in-a-Specific-PDF-Page
[7]: #Replace-Text-in-PDF-Page-Region-using-CPP
[8]: #Find-and-Replace-Text-in-PDF-files-using-Regular-Expressions
[9]: #Get-a-Free-License
[10]: https://products.aspose.com/pdf/cpp
[11]: https://www.nuget.org/packages/Aspose.Pdf.cpp
[12]: https://downloads.aspose.com/pdf/cpp
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber
[16]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber
[17]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page_collection#aae17f014d368888f824cfed8561c6e84
[18]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber#a430a2bee4faae4b776196b14508a075f
[19]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_collection
[20]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment#a078c57d3649fa893618e193ef1ef3ba2
[21]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[22]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber
[23]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[24]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber
[25]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber
[26]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page#a96ed5a07bf605c8ee58690d3103b5a58
[27]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber#a430a2bee4faae4b776196b14508a075f
[28]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_collection
[29]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment#a078c57d3649fa893618e193ef1ef3ba2
[30]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[31]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.rectangle
[32]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[33]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber
[34]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_search_options#a30fa6199be33a5ad565bc7605bd7f4e4
[35]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber
[36]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page#a96ed5a07bf605c8ee58690d3103b5a58
[37]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber#a430a2bee4faae4b776196b14508a075f
[38]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_collection
[39]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment#a078c57d3649fa893618e193ef1ef3ba2
[40]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[41]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_search_options
[42]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[43]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber
[44]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_search_options
[45]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_search_options
[46]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber
[47]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber#a9444b3216f205fbe55fbfa7216019264
[48]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber
[49]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page_collection#aae17f014d368888f824cfed8561c6e84
[50]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_absorber#a430a2bee4faae4b776196b14508a075f
[51]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_collection
[52]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment#a078c57d3649fa893618e193ef1ef3ba2
[53]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[54]: https://purchase.aspose.com/temporary-license
[55]: https://docs.aspose.com/pdf/cpp/developer-guide/
[56]: https://forum.aspose.com/c/pdf/10
[57]: https://blog.aspose.com/2021/02/01/convert-pdf-to-svg-format-using-cpp/





