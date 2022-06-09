---
title: 'Create MS Word Editor in ASP.NET MVC'
seoTitle: ""
description: ""
date: Fri, 17 Apr 2020 17:28:44 +0000
draft: false
url: /2020/04/17/asp.net-mvc-word-editor-create-edit-word-documents/
author: Usman Aziz
summary: ''
tags: ['Create Word Documents in ASP.NET', 'Edit Word Documents in ASP.NET', 'MS Word Editor in ASP.NET MVC']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/ASP.NET-MVC-Word-Editor.jpg" alt="ASP.NET MVC Word Editor">}}


[Aspose.Words for .NET][1] provides a complete set of features for manipulating and converting MS Word documents within a multitude of .NET applications. Particularly, you can create new or edit the existing Word documents within the desktop or web applications. In this post, I'll show you how to leverage the Word processing capabilities of _Aspose.Words for .NET_ and create a web-based **MS Word Editor in ASP.NET MVC**.

## ASP.NET MVC Word Editor - Create Word Documents

We are going to create an ASP.NET MVC Word Editor that will be based on a WYSIWYG HTML editor for writing and updating the content of the documents. Furthermore, _Aspose.Words for .NET_ will be used for rendering the Word document's content into HTML for editing and generating Word documents from the updated content.

### Steps to Create MS Word Editor in ASP.NET MVC

For the demonstration, I have used JavaScript-based [Suneditor][2] WYSIWYG editor in this application. You may either use the same or select any other HTML editor that suits your requirements. The following are the steps to create the ASP.NET Word Editor.

*   First, create a new **ASP.NET Core Web Application** in Visual Studio.



{{< figure align=center src="images/ASP.NET-Core-MVC-Web-Application.jpg" alt="">}}


*   Select the **Web Application (Model-View-Controller)** template.



{{< figure align=center src="images/MVC-Project-Template.jpg" alt="">}}


*   Download the WYSIWYG editor's files and keep them in **wwwroot** directory.



{{< figure align=center src="images/WYSIWYG-Editor.jpg" alt="">}}


*   Open NuGet Package Manager and install the **Aspose.Words for .NET** package.



{{< figure align=center src="images/Aspose.Words-NuGet.jpg" alt="">}}


*   Add the following script in **index.cshtml** view.

{{< gist aspose-com-gists f48951a077ac02613f2881a234a0967d "index.cshtml" >}}

*   Add the following methods in **HomeController.cs** controller.

{{< gist aspose-com-gists f48951a077ac02613f2881a234a0967d "HomeController.cs" >}}

*   Finally, build and run the application in your favorite browser.



{{< figure align=center src="images/ASP.NET-Word-Editor.jpg" alt="">}}


## Demo

The following is the demonstration of how to create or edit Word documents in ASP.NET Word Editor.

### Create a Word Document in ASP.NET



{{< figure align=center src="images/Create-Word-Document.webp" alt="">}}


### Edit a Word Document in ASP.NET



{{< figure align=center src="images/Edit-Word-Document-new.webp" alt="">}}


## Download Source Code

You can download the source code of MS Word Editor from [here][3].

## Conclusion

In this article, you have learned how to create MS Word documents in ASP.NET. The step-by-step guide along with code samples has shown how to create a simple web-based MS Word editor in ASP.NET MVC. Alongside, you can explore more about Aspose.Words for .NET using the following resources.

*   [API Documentation][4]
*   [Source Code examples][5]

## Try Aspose.Words for .NET for Free

You can try _Aspose.Words for .NET_ for free by requesting a [temporary license][6].

## Related Articles

*   [ASP.NET Excel Viewer][7]
*   [ASP.NET PowerPoint Viewer][8]




[1]: https://products.aspose.com/words/net
[2]: https://www.cssscript.com/minimal-wysiwyg-editor-pure-javascript-suneditor/
[3]: https://github.com/usman-aziz/ASP.NET-MVC-Word-Editor
[4]: https://docs.aspose.com/display/wordsnet
[5]: https://github.com/aspose-words/Aspose.Words-for-.NET
[6]: https://purchase.aspose.com/temporary-license
[7]: https://blog.aspose.com/2020/01/31/view-excel-files-in-asp-net-mvc-csharp-excel-viewer/
[8]: https://blog.aspose.com/2020/02/23/asp-net-core-powerpoint-viewer-display-ppt-pptx-presentations/





