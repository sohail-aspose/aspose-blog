---
title: 'ASP.NET PDF Editor - Create PDF Files in ASP.NET Core'
seoTitle: ""
description: ""
date: Thu, 06 Feb 2020 12:38:12 +0000
draft: false
url: /2020/02/06/create-pdf-files-in-asp-net-core-mvc/
author: Usman Aziz
summary: ''
tags: ['.net core pdf generator', 'asp.net pdf creator', 'asp.net pdf generator', 'create pdf files in asp.net core', 'create pdf files programmatically in asp.net core']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Create-PDF-Files-ASP.NET-Core.png" alt="ASP.NET Core PDF Generator">}}


**[PDF][1]** (Portable Document Format) is a well-known and widely used format to display or view digital documents without worrying about the compatible software, operating system, or hardware. Creating PDF files programmatically is quite useful for generating documents such as reports, resumes, invoices, etc. online within the web applications. So in this article, I'll show you **how to create an ASP.NET PDF editor** that will let you **create PDF files programmatically in ASP.NET Core** web application using C#.

## Create PDF Files in ASP.NET Core

In order to create PDF files programmatically, we'll develop a **PDF editor** in the ASP.NET Core web application. This application will be based on a **WYSIWYG HTML editor** to create the content and **[Aspose.PDF for .NET][2]** to generate the PDF based on that content. So let's begin creating our PDF editor application in ASP.NET Core by following the below steps.

*   Create a new **ASP.NET Core Web Application** in Visual Studio.



{{< figure align=center src="images/ASP.NET-Core-MVC-Web-Application.png" alt="asp.net core generate pdf ">}}


*   Select **Web Application (Model-View-Controller)** from the templates.



{{< figure align=center src="images/MVC-Project-Template.png" alt="asp.net core web application">}}


Since this PDF editor uses the WYSIWYG HTML editor to create the content for PDF documents, for the demonstration, I have used CKEditor's Standard Package. You can feel free to choose your favorite HTML editor that could best serve your requirements. If you are good to go with the afore-mentioned editor then follow the below step for its integration, else skip it.

*   Download the CKEditor's [package][3], extract it and copy/paste the folder in **wwwroot** directory.



{{< figure align=center src="images/Integrate-HTML-Editor.png" alt="asp.net pdf generator">}}


*   Open NuGet Package Manager and install the packages of **Aspose.PDF** and **CKEditor**.



{{< figure align=center src="images/Aspose.PDF-and-CKEditor-NPM.png" alt="Create PDF in ASP.NET Core">}}


*   Open **Views/Home/index.cshtml** and replace the script with the following.

{{< gist aspose-com-gists cff53cfa900b8d4959be12e963e2598e "index.cshtml" >}}

*   Open **Controllers/HomeController.cs** and replace the code with the following.

{{< gist aspose-com-gists cff53cfa900b8d4959be12e963e2598e "HomeController.cs" >}}

*   Build the application and run it in your favorite browser.

## Creating PDF Files using ASP.NET PDF Editor - Demo

The following is the demonstration of how to create PDF files using ASP.NET PDF Editor we have just created.

<figure class="wp-block-embed is-type-video is-provider-youtube wp-block-embed-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">https://youtu.be/oSmVjmdnqlo</div></figure>

## Download Source Code

You can download the complete source code of the ASP.NET PDF Editor from [GitHub][4].

## Get a Free License for Aspose.PDF for .NET

You can request a free [temporary license][5] of **Aspose.PDF for .NET** to avoid evaluation limitations.

## Related Articles

*   [Encrypt and Decrypt PDF Files using C#][6]
*   [Generate PDF Files using C#][7]




[1]: https://wiki.fileformat.com/view/pdf/
[2]: https://products.aspose.com/pdf/net
[3]: https://ckeditor.com/ckeditor-4/download/
[4]: https://github.com/Usman Azizgroupdocs/PDF-Creator-ASP.NET-Core
[5]: https://purchase.aspose.com/temporary-license
[6]: https://blog.aspose.com/2020/04/28/encrypt-or-decrypt-pdf-files-programmatically-using-csharp-asp.net/
[7]: https://blog.aspose.com/2020/12/02/create-pdf-files-using-csharp/





