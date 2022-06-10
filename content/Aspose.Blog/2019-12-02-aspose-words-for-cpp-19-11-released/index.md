---
title: 'Customize Formatting of Horizontal Rule Shape in Word Documents using C++'
date: Mon, 02 Dec 2019 08:24:54 +0000
draft: false
url: /2019/12/02/aspose-words-for-cpp-19-11-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

It is our great pleasure to share with you that we have published yet another new release and you can now [download Aspose.Words for C++ 19.11][1] API from the downloads section. Following list highlights the major features and you will also learn how you can use Aspose.Words for C++ 19.11 to:

*   Work with **Web Extensions** and **Task Panes**
*   Customize Formatting of **Horizontal Rule Shape**
*   Aspose.Words for C++ has now improved character spacing calculation when 'use printer metrics' option is set
*   **Macros** support is improved in this release

## Work with Web Extensions and Task Panes  

Different classes for representing **Office Add-ins** are now part of the [WebExtensions namespace][2] of Aspose.Words for C++. You can now use Aspose.Words for C++ to work with Web Extensions and Task Panes in Office Add-ins. For example, the API now provides new TaskPane class, TaskPaneCollection class, TaskPaneDockState enumeration, Document.WebExtensionTaskPanes property etc.

The following code example can be used to [create task panes and add to web extension task panes][3] with basic properties.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Programming-Documents-Document-WorkingWithWebExtension-UsingWebExtensionTaskPanes.cpp" >}}

## Customize Formatting of Horizontal Rule Shape

The [Shape.HorizontalRuleFormat][4] property is now available in the Aspose.Words for C++ API for accessing the properties of the **horizontal rule shape**. Basic properties like Height, Color, NoShade, etc are now available in the HorizontalRuleFormat class. For example, you can use the following code to [set HorizontalRuleFormat to format a horizontal rule shape][5].

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Programming-Documents-Shapes-WorkingWithShapes-DocumentBuilderInsertHorizontalRule.cpp" >}}

## VBA Macros Support Improved

Aspose.Words for C++ API now provides [Dcoument.VbaProject][6] property to get or set [VbaProject][7] in the Word document. The following code example demonstrates [how to create a VBA project and VBA Module][8] along with basic properties e.g. Name and Type.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Loading-and-Saving-WorkingWithVbaMacros-CreateVbaProject.cpp" >}}

## See Also Useful Links

The resources, you may need to accomplish your tasks:

*   [Aspose.Words for C++ Online Documentation][9] - Knowledge Base Programmer's Guide and much more.
*   [Aspose.Words for C++ Product Page][10]
*   [Install Aspose.Words for C++ NuGet Package][11]
*   [Aspose.Words for C++ API Reference Guide][12] - Details about classes, methods, properties, constants, interfaces and much more.
*   [Download Examples at GitHub Repository][13] - You can get these code examples from GitHub.

To get technical support for Aspose.Words for C++, please feel free to post your queries/questions in [Aspose.Words for C++ support forum][14].




[1]: https://downloads.aspose.com/words/cpp/new-releases/aspose.words-for-c---19.11/
[2]: https://apireference.aspose.com/cpp/words/namespace/aspose.words.web_extensions/
[3]: https://docs.aspose.com/words/cpp/working-with-web-extensions/
[4]: https://apireference.aspose.com/cpp/words/class/aspose.words.drawing.horizontal_rule_format/
[5]: https://docs.aspose.com/words/cpp/working-with-shapes/#WorkingwithShapes-HorizontalRuleFormat
[6]: https://apireference.aspose.com/cpp/words/class/aspose.words.document/#a5f9fce4e11a6511c875df7b5c00ad3ab
[7]: https://apireference.aspose.com/
[8]: https://docs.aspose.com/words/cpp/working-with-vba-macros/#WorkingwithVBAMacros-CreatingaVBAProject
[9]: https://docs.aspose.com/words/cpp/
[10]: https://products.aspose.com/words/cpp
[11]: https://www.nuget.org/packages/Aspose.Words.Cpp/
[12]: https://apireference.aspose.com/cpp/words
[13]: https://github.com/aspose-words/Aspose.words-for-C
[14]: https://forum.aspose.com/c/words




