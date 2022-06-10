---
title: 'Aspose 最新产品资讯, 2007年8月'
date: Thu, 02 Aug 2007 04:44:00 +0000
draft: false
url: /2007/08/02/aspose-2007-8/
author: Salman Sarfraz
summary: ''
tags: ['Aspose China']
---

**    In This Issue**

*   欢迎！
*   产品推荐— Aspose.Slides for Reporting Services
*   使用Aspose.Cells for Reporting Services在MS SQL 服务器上生成 Excel报表
*   体验Aspose.Editor v2.1.0中改进的用户界面
*   Aspose.Pdf for Java的最新版本
*   Aspose.Grid v1.9.2的最新改进
*   Aspose.Words for Reporting Services可以在 MS SQL Server 2008 "Katmai"上使用
*   Aspose.Words for .NET v4.3.0对Windows Vista适用的最优化
*   技术小技巧—通过程序解析Microsoft Outlook Message files
*   Aspose.Pdf for .NET v3.5.5.0修补程序

**欢迎！**

欢迎来到Aspose2007年8月时事快报！在这个月的时事快报中，我们将对我们的推荐产品Aspose.Slides for Reporting Services作出相关介绍。我们还会介绍Aspose.Cells for Reporting Services, Aspose.Grid, Aspose.Words, Aspose.Pdf, Aspose.Editor 以及 Aspose.Words for Reporting Services这些产品在最新版本中新增的一些令人兴奋的功能。通过本月的  Tech-Tip，您将了解到来自Aspose的最新信息—如何使用Aspose.Network在程序中解析Microsoft Outlook Message files(\*.msg).

**产品亮点**

 [Aspose.Slides for Reporting Services][1]是目前市场上唯一能够在Microsoft SQL Server 2005 Reporting Services (x86 and x64)中生成正确的PPT或PPS报表的解决方案。所有RDL报表功能，包括表格，矩阵，图表和图片都可以高精度地转换为Microsoft PowerPoint presentations。Microsoft SQL Server Reporting Services没有将报表输出为Microsoft PowerPoint presentations的内置功能，但在服务器上安装了Aspose.Slides for Reporting Services之后，您可以获取两种额外的输出格式： PPT – PowerPoint Presentation via Aspose.Slides PPS – PowerPoint Show via Aspose.Slides Aspose.Slides for Reporting Services在服务器上创建presentation并不使用Microsoft PowerPoint. Aspose.Slides for Reporting Services使用内在的Aspose.Slides for .NET—在服务器上处理presentation的世界级组件。请下载Aspose.Slides for Reporting Services的免费试用版本（[download][2]），看其是否满足您的  商业需求。

**使用Aspose.Cells for Reporting Services在MS SQL 服务器上生成 Excel报表**

 [Aspose.Cells for Reporting Services][3]允许您传递本地Excel报表至Microsoft SQL Server 2005 Reporting Services。不同于Excel报表的内置呈现，Aspose.Cells for Reporting Services提供了一种扩展功能设置，并允许将RDL报表转换为：Excel 97-2003二进制XLS格式，SpreadsheetML 或 Excel 2007 XLSX 格式。 在新近发布的Aspose.Cells for Reporting Services,新增了其他一些有价值的功能，像支持背景图片，输出数据至CSV或Tab Delimited files等。此外，少数重大bug也得到解决。了解详情，请click here.

**体验Aspose.Editor v2.1.0中改进的用户界面**

Aspose发布了Aspose.Editor的新版本。主要目标是改进用户界面和提供编辑器的标准控件。Aspose.Editor现在嵌入的功能有标尺，主菜单栏，工具栏等等。开发者可以使用标准控件，并可定制或用第三方控件替换它们。这样可以使用户友好编辑器简单化并减少开发者的工作量。欲了解Aspose.Editor for .NET v2.1.0的更多改进细节，请click here.

**Aspose.Pdf for Java的最新版本**

在新更新的Aspose.Pdf中，java开发者可以使用一些新增的重要功能，如JavaScript，注释和书签。JavaScript 提供了一个最简单但有效的定制PDF文件的  方法。使用注释功能，您可以非常方便地在创建过程中往PDF中添加注释。使用书签您可以根据文档标题自动创建书签。一些重大的bug（如在PDF中添加表格，获取颜色信息，许可，控制图片大小和为PDF节设置背景图片等）已得到解决。请访问官方网页v2.2.0.0 和  v2.2.1.0.

**Latest Enhancements in Aspose.Grid v1.9.2**

添加了一些新的功能和重大  改进的Aspose.Grid v1.9.2更加优秀。新的功能包括：对基于呈现的XHTML1.0的支持，工作表序列化，定制和自动筛选，工具栏的拖拽和滚动等。此外，公式编辑的执行，XHTML呈现以及其他的  功能都令Aspose.Grid的效率得到很大优化。除了新增功能和改进之外，一些重大的bug在此版本中也得到了解决。了解更多关于Aspose.Grid的改进请click here.。

**Aspose.Words for Reporting Services可以在 MS SQL Server 2008 "Katmai"上使用**

非常高兴地宣布：经过 Aspose.Words团队的测试，[Aspose.Words for Reporting Services][4]在Microsoft SQL Server 2008 “Katmai” Reporting Services的CTP3上可以较好地运行。此外，textboxes对WritingMode属性的支持也已添加。欲了解更多信息以及Aspose.Words for Reporting Services的  其他改进，请访问v1.3.0 和  v1.3.1的发布网页。

**知识点**

您是否知道使用Aspose.Network您仅需用几行代码就可以解析Microsoft Outlook Message files（\*.msg）?下面就是： \[C#\] //Loading outlook email message file MapiMessage msg = MapiMessage.FromFile(@"C:\\WithAttachment.msg"); //Obtaining subject of the email message Console.WriteLine("Subject:" + msg.Subject); //Obtaining sender name of the email message Console.WriteLine("From:" + msg.SenderName); //Obtaining body of the email message Console.WriteLine("Body:" + msg.Body); //Obtaining information about number of attachments in the email message Console.WriteLine("Attachment Count:" + msg.Attachments.Count); //Iterating through all attachments in the email message foreach (MapiAttachment attachment in msg.Attachments) {         //Accessing the file name of the attachment        Console.WriteLine("Attachment:"+ attachment.FileName);                             //Saving attachment         attachment.Save(attachment.LongFileName); } \[VB\] 'Loading outlook email message file Dim msg As MapiMessage =  MapiMessage.FromFile("C:\\WithAttachment.msg") 'Obtaining subject of the email message Console.WriteLine("Subject:" + msg.Subject) 'Obtaining sender name of the email message Console.WriteLine("From:" + msg.SenderName) 'Obtaining body of the email message Console.WriteLine("Body:" + msg.Body) 'Obtaining information about number of attachments in the email message Console.WriteLine("Attachment Count:" + msg.Attachments.Count) ‘Iterating through all attachments in the email message Dim attachment As MapiAttachment For Each attachment In msg.Attachments        ‘Accessing the file name of the attachment        Console.WriteLine("Attachment:"+ attachment.FileName)        'Saving attachment        attachment.Save(attachment.LongFileName) Next

**Aspose.Words for .NET v4.3.0对Windows Vista适用的最优化**

最新发布的Aspose.Words for .NET v4.3.0对64位操作系统包括Windows Vista x64和Windows Server 2003 x64都是及其优化的。Aspose.Words已在Windows vista下深入测试，所有安装问题已得到解决。一些严重的 bug如 WordML输出，Word转换为PDF，书签，字体，本节页数域，HTML流输出等均已得到解决。了解更多详情，请参见complete story

**Aspose.Pdf for .NET v3.5.5.0 Mega Hotfix**

2007年7月，Aspose.Pdf团队发布了3大补丁，解决了以下方面的 30多个bug：Word/HTML转换为PDF，节或页分隔，脚注，表格，图片布置，目录（toc），页数，列合并，光标切换等。请到其官方发布网页查看已解决bug的完全列表（1st, 2nd 和  3rd 修补程序）。现在您可以下载最新版本以确保您的程序更加完美。

* * *

Aspose产品中国区独家代理 [慧都控件网][5]




[1]: /Products/Aspose.Slides.Reporting.Services/
[2]: /Community/Files/52/aspose.slides.reporting.services/default.aspx
[3]: /Community/Files/52/aspose.cells.reporting.services/default.aspx
[4]: /Community/Files/52/aspose.words.reporting.services/default.aspx
[5]: http://www.evget.com/



