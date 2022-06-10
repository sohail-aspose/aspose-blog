---
title: 'Web Extensions - Office Add-ins Task Panes in Java Word API'
date: Sat, 16 Nov 2019 08:46:30 +0000
draft: false
url: /2019/11/16/office-add-ins-task-panes-using-java-word-api/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Its great pleasure to share that we have achieved another milestone by publishing new release of Aspose.Words for Java i.e. 19.11 that **supports Harfbuzz Shaper plugin on Unix-based operating systems** and will enable developers to work with **Web Extensions**, customize the formatting of the **horizontal rule shape** etc. Details of all the new features, enhancements and bugs resolution can be seen in the [release notes][1]. This latest release [Aspose.Words for Java v19.11][2] can be downloaded from the download section. Let us have a brief look at the salient features of this exciting release.  

## Work with Web Extensions and Task Panes

Aspose.Words API provides the **WebExtensions** namespace that provides various classes to customize elements and attributes extending the XML vocabulary for representing **Office Add-ins**. You can now use Aspose.Words for Java to [work with Task Panes in Office Add-ins and Web Extensions][3]. For this purpose, it provides new _TaskPane class_, _TaskPaneCollection class_, _TaskPaneDockState enumeration_, _Document.WebExtensionTaskPanes property_ etc.

The following code example demonstrates how to create task panes and add to web extension task panes with basic properties.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-WebExtension-WorkingWithWebExtension-UsingWebExtensionTaskPanes.java" >}}

## Customize Formatting of Horizontal Rule Shape

Aspose.Words for Java API now provides _Shape.HorizontalRuleFormat property_ to access the properties of the **horizontal rule shape**. The _HorizontalRuleFormat class_ exposes basic properties like _Height_, _Color_, _NoShade_ etc. The following code example demonstrates [how to set HorizontalRuleFormat to format a horizontal rule][4].

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-Shapes-WorkingWithShapes-ShapeHorizontalRuleFormat.java" >}}

## Macros Support Improved

Aspose.Words for Java API provides _Dcoument.VbaProject property_ to get or set _VbaProject_ in the document. The following code example demonstrates [how to create a VBA project and VBA Module][5] along with basic properties e.g. _Name_ and _Type_.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithVbaMacros-CreateVbaProject.java" >}}

## See also Useful Links

*   [Aspose.Words for Java Online Documentation][6] - up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Words for Java Product Page][7]
*   [Install Aspose.Words for Java from Maven][8]
*   [Aspose.Words for Java API Reference Guide][9] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][10] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for Java API by posting your suggestions and concerns in the [Aspose.Words for Java Support Forum][11].




[1]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+19.11+Release+Notes
[2]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-19.11/
[3]: https://docs.aspose.com/display/wordsjava/Working+with+Web+Extensions
[4]: https://docs.aspose.com/display/wordsjava/Working+with+Shapes#WorkingwithShapes-HorizontalRuleFormat
[5]: https://docs.aspose.com/display/wordsjava/Working+with+VBA+Macros#WorkingwithVBAMacros-CreatingaVBAProject
[6]: https://docs.aspose.com/display/wordsjava/Home
[7]: https://products.aspose.com/words/java
[8]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[9]: https://apireference.aspose.com/java/words
[10]: https://github.com/aspose-words/Aspose.Words-for-Java
[11]: https://forum.aspose.com/c/words




