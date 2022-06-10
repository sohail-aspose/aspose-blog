---
title: 'Read or Write Markdown Text in Java using Aspose.Words for Java 19.7'
date: Fri, 19 Jul 2019 10:17:14 +0000
draft: false
url: /2019/07/19/create-read-or-write-markdown-md-files-in-java/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Hello guys, let's check out what’s new for you in [Aspose.Words for Java 19.7][1]  release.

## Support for Markdown Features

Markdown is a simple way to format plain text that can easily be converted to HTML. Markdown features currently supported by Aspose.Words are _{Headings, Block quotes, Horizontal rules, Bold emphasis, Italic emphasis}_. The Markdown feature implementation mostly follows the CommonMark specification in Aspose.Words API and all the features are represented as corresponding styles or direct formatting. Which means that:

*   Bold and Italic are represented as Font.Bold and Font.Italic.
*   Headings are paragraphs with Heading 1 - Heading 6 styles
*   Quotes are paragraphs with "Quote" in style name
*   HorizontalRule is a paragraph with HorizontalRule shape

For more details, please read the following article.

*   [Working with Markdown Features][2]

## Linked TextBoxes in Word Document

[TextBox class][3] is used to specify how text is displayed inside Shape. It provides a public property [Parent][4] to get the parent Shape of the TextBox and to allow to find linked Shape from linked TextBox. Please check the following examples for more details:

*   [Create A Link between TextBoxes in Word Document][5]
*   [Check TextBox Sequence][6]
*   [Break a Textbox Link][7]

## Restart List Numbering Dynamically using LINQ Reporting

You can restart list numbering within your documents dynamically using restartNum tags. In particular, this feature is useful when working with a nested numbered list within a data band. Continue reading [Restarting List Numbering Dynamically][8].

## Detect SmartArt Shape in Word Document

Starting from this release, you can detect SmartArt shape in Word document. You need to simply use the [Shape.HasSmartArt][9] property. This property returns true if this Shape has a SmartArt object. Continue reading [Detect SmartArt Shape][10].

## Get Revision Group Details

The [Revision.Group][11] property in Revision class can be used to get details if the revision belongs to any group. Its value will be null if the revision does not belong to any group. If the revision type is _RevisionType.StyleDefinitionChange_ or if the revision no longer exists in document context (accepted/rejected) then it means that Revision has no group.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-TrackChanges-GetRevisionGroupDetails.java" >}}

## See also Useful Links

*   [Aspose.Words for Java Online Documentation][12] - up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Words for Java Product Page][13]
*   [Install Aspose.Words for Java from Maven][14]
*   [Aspose.Words for Java API Reference Guide][15] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][16] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for Java API by posting your suggestions and concerns in the [Aspose.Words for Java Support Forum][17].




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-19.7/
[2]: https://docs.aspose.com/display/wordsjava/Working+with+Markdown+Features
[3]: https://apireference.aspose.com/java/words/com.aspose.words/TextBox
[4]: https://apireference.aspose.com/java/words/com.aspose.words/textbox#Parent
[5]: https://docs.aspose.com/display/wordsjava/Working+with+Linked+TextBoxes#WorkingwithLinkedTextBoxes-CreateALink
[6]: https://docs.aspose.com/display/wordsjava/Working+with+Linked+TextBoxes#WorkingwithLinkedTextBoxes-CheckTextBoxSequence
[7]: https://docs.aspose.com/display/wordsjava/Working+with+Linked+TextBoxes#WorkingwithLinkedTextBoxes-BreakaLink
[8]: https://docs.aspose.com/display/wordsjava/Restarting+List+Numbering+Dynamically
[9]: https://apireference.aspose.com/java/words/com.aspose.words/shape#HasSmartArt
[10]: https://docs.aspose.com/display/wordsjava/Working+with+Shapes#WorkingwithShapes-DetectSmartArtShape
[11]: https://apireference.aspose.com/java/words/com.aspose.words/revision#Group
[12]: https://docs.aspose.com/display/wordsjava/Home
[13]: https://products.aspose.com/words/java
[14]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[15]: https://apireference.aspose.com/java/words
[16]: https://github.com/aspose-words/Aspose.Words-for-Java
[17]: https://forum.aspose.com/c/words




