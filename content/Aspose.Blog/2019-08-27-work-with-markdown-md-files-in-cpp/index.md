---
title: 'Work with Markdown (.md) Files in C++ using Aspose.Words for C++'
date: Tue, 27 Aug 2019 07:55:43 +0000
draft: false
url: /2019/08/27/work-with-markdown-md-files-in-cpp/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Hello guys, let's check out what’s new for you in [Aspose.Words for C++ 19.8][1] release.

## Markdown Features (.md Format)

Markdown is a simple way to format plain text that can easily be converted to HTML. Markdown features currently supported by Aspose.Words are_ {Headings, Block quotes, Horizontal rules, Bold emphasis, Italic emphasis}_. The Markdown feature implementation mostly follows the CommonMark specification in Aspose.Words API and all the features are represented as corresponding styles or direct formatting. Which means that:

*   Bold and Italic are represented as Font.Bold and Font.Italic.
*   Headings are paragraphs with Heading 1 – Heading 6 styles
*   Quotes are paragraphs with “Quote” in style name
*   HorizontalRule is a paragraph with HorizontalRule shape

For more details, please read the following article.  
[Working with Markdown Features][2]

## Load and Convert Encrypted OpenDocument (.odt or .ott format)

The OdtSaveOptions class can now be used to specify additional options when saving a document into the ODT or OTT format. You can initialize a new instance of this class that can be used to save a document in the ODT format encrypted with a password. You can also use [OdtSaveOptions.Password][3] property to get or **set a password to encrypt Word document**. The code sample below shows how to load and save OpenDocument encrypted with a password.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Loading-and-Saving-Load_Options-LoadAndSaveEncryptedODT.cpp" >}}

## Compress Metafiles in Word Document

In MS Word, all the metafiles are compressed by default regardless of their size. However, Aspose.Words used to **compress large metafiles** only and smaller ones were not compressed just because of better performance. Aspose.Words for C++ now provides a property [AlwaysCompressMetafiles][4], to facilitate the users if they want to compress all the metafiles either large or small. Its default value is true which means that all metafiles shall be compressed regardless of their sizes and false means that small metafiles shall not be compressed for performance reason.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Loading-and-Saving-WorkingWithDoc-AlwaysCompressMetafiles.cpp" >}}

## Linked TextBoxes in Word Document

[TextBox class][5] is used to specify how text is displayed inside Shape. It provides a public property [Parent][6]  to get the parent Shape of the TextBox and to allow to find linked Shape from linked TextBox. Please check the following examples for more details:

*   [Create A Link between TextBoxes in Word Document][7]
*   [Check TextBox Sequence][8]
*   [Break a Textbox Link][9]

## Check if Particular DML Text Effect is Applied

Aspose.Words for C++ now provides Font->HasDmlEffect() method to check if particular DML text effect is applied to the Run. This is a boolean type property and returns true if particular DML text effect is applied. The given below code example shows how to use this property.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Programming-Documents-Document-CheckDMLTextEffect-CheckDMLTextEffect.cpp" >}}

## Working with TableStyle

Aspose.Words for C++ now provides a TableStyle class inherited from Style class. The TableStyle facilitates user to apply different styling options such as shading, padding, indentation, CellSpacing and Font etc. For more details, please refer to the following sections:

*   [How to Create a Table Style in Word Document][10]
*   [How to Define Conditional Formatting][11]

## Get Revision Group Details

The Revision.Group property in Revision class can be used to get details if the revision belongs to any group. Its value will be null if the revision does not belong to any group. If revision type is RevisionType.StyleDefinitionChange or if the revision no longer exists in document context (accepted/rejected) then it means that Revision has no group.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Programming-Documents-Document-WorkingWithRevisions-GetRevisionGroupDetails.cpp" >}}

## See Also Useful Links

The resources, you may need to accomplish your tasks:

*   [Aspose.Words for C++ Online Documentation][12] - up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Words for C++ Product Page][13]
*   [Install Aspose.Words for C++ NuGet Package][14]
*   [Aspose.Words for C++ API Reference Guide][15] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][16] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for C++ API by posting your suggestions and concerns in the [Aspose.Words for C++ support forum][17].




[1]: https://downloads.aspose.com/words/cpp/new-releases/aspose.words-for-c---19.8/
[2]: https://docs.aspose.com/display/wordscpp/Working+with+Markdown+Features
[3]: https://apireference.aspose.com/cpp/words/class/aspose.words.saving.odt_save_options/#af6c4e23ded0f36d00f63b1bddbaa643c
[4]: https://apireference.aspose.com/net/words/aspose.words.saving/docsaveoptions/properties/alwayscompressmetafiles
[5]: https://apireference.aspose.com/java/words/com.aspose.words/TextBox
[6]: https://apireference.aspose.com/java/words/com.aspose.words/textbox#Parent
[7]: https://docs.aspose.com/display/wordscpp/Working+with+Linked+TextBoxes#WorkingwithLinkedTextBoxes-CreateALink
[8]: https://docs.aspose.com/display/wordscpp/Working+with+Linked+TextBoxes#WorkingwithLinkedTextBoxes-CheckTextBoxSequence
[9]: https://docs.aspose.com/display/wordscpp/Working+with+Linked+TextBoxes#WorkingwithLinkedTextBoxes-BreakaLink
[10]: https://docs.aspose.com/display/wordscpp/Working+with+TableStyle#WorkingwithTableStyle-CreateaTableStyle
[11]: https://docs.aspose.com/display/wordscpp/Working+with+TableStyle#WorkingwithTableStyle-DefiningConditionalFormatting
[12]: https://docs.aspose.com/display/wordscpp/Home
[13]: https://products.aspose.com/words/cpp
[14]: https://www.nuget.org/packages/Aspose.Words.Cpp/
[15]: https://apireference.aspose.com/cpp/words
[16]: https://github.com/aspose-words/Aspose.words-for-C
[17]: https://forum.aspose.com/c/words




