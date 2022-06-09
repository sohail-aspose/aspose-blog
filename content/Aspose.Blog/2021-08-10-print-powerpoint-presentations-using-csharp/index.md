---
title: 'Print PowerPoint Presentations using C#'
seoTitle: "Print PowerPoint Presentations using C# | Set Printer and Print Options"
description: "Use .NET PowerPoint API to print PowerPoint presentations using C# .NET. Specify desired printer and other printing options to print the presentations."
date: Tue, 10 Aug 2021 16:32:00 +0000
draft: false
url: /2021/08/10/print-powerpoint-presentations-using-csharp/
author: Usman Aziz
summary: 'Often, you may need to print the PowerPoint presentations programmatically from your web or desktop applications. In order to achieve it, this article covers **how to print PowerPoint presentations using C#**. Furthermore, you will also learn how to set the desired printer and other printing options dynamically.'
tags: ['print powerpoint presentation using csharp', 'print ppt with print settings csharp', 'print ppt with specific printer csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Print-Presentation.jpg" alt="Print Presentation C#">}}


Often, you may need to print the PowerPoint presentations programmatically from your web or desktop applications. In order to achieve it, this article covers **how to print PowerPoint presentations using C#**. Furthermore, you will also learn how to set the desired printer and other printing options dynamically.

*   [C# API to Print PowerPoint Presentations][1]
*   [Print PowerPoint Presentations][2]
*   [Print PowerPoint Presentation with Specific Printer][3]
*   [Set PowerPoint Printing Options Dynamically][4]

## C# API to Print PowerPoint Presentations {#API-to-Print-PowerPoint-Presentations}

In order to print PowerPoint presentations, we will use [Aspose.Slides for .NET][5]. It is a presentation manipulation API that lets you create, modify and convert PowerPoint presentations from within your .NET applications. You can either [download][6] the API or install it using [NuGet][7].

```
PM> Install-Package Aspose.Slides.NET
```

## Print PowerPoint Presentations using C# {#Print-PowerPoint-Presentations}

The following are the steps to print a PowerPoint presentation with the default printer using C#.

*   Create an instance of [Presentation][8] class to load the PowerPoint presentation.
*   Call the [Presentation.Print()][9] method to print the presentation.

The following code sample shows how to print a PowerPoint presentation.

{{< gist aspose-com-gists 8c978af9f3f8cd902dff92bea4060aa3 "print-presentation.cs" >}}

## C# Print PowerPoint Presentation with Specific Printer {#Print-PowerPoint-Presentation-with-Specific-Printer}

You can also specify the printer's name in order to print a PowerPoint presentation. The following are the steps to print a presentation with a particular printer.

*   Load the PowerPoint presentation using [Presentation][10] class.
*   Call the [Presentation.Print(string)][11] method and pass printer's name as its parameter.

The following code sample shows how to print a PowerPoint presentation with a specific printer.

{{< gist aspose-com-gists 8c978af9f3f8cd902dff92bea4060aa3 "print-presentation-with-specific-printer.cs" >}}

## Set PowerPoint Printing Options Dynamically {#Set-PowerPoint-Printing-Options-Dynamically}

You can also set the other printing options such as the number of copies, page margins, page orientation, etc. The following are the steps to set different printing options for PowerPoint presentations.

*   Load the PowerPoint presentation using [Presentation][12] class.
*   Create an instance of [PrinterSettings][13] class and set the desired options such as:
    *   _PrinterSettings.Copies_ to set number of copies,
    *   _PrinterSettings.DefaultPageSettings.Landscape_ to print slides in landscape orientation,
    *   and [more][14].
*   Call the [Presentation.Print(PrinterSettings)][15] method and pass PrinterSettings object as its parameter.

The following code sample shows how to set different options for printing PowerPoint presentations.

{{< gist aspose-com-gists 8c978af9f3f8cd902dff92bea4060aa3 "print-presentation-print-settings.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][16].

## Conclusion

In this article, you have learned how to print PowerPoint presentations using C#. Furthermore, you have seen how to specify the printer's name and other printing options. In addition, you can visit the [documentation][17] to explore other features of Aspose.Slides for .NET. Also, you can feel free to let us know about your queries via our [forum][18].

## See Also

*   [Create MS PowerPoint Presentations in C#][19]




[1]: #API-to-Print-PowerPoint-Presentations
[2]: #Print-PowerPoint-Presentations
[3]: #Print-PowerPoint-Presentation-with-Specific-Printer
[4]: #Set-PowerPoint-Printing-Options-Dynamically
[5]: https://products.aspose.com/slides/net
[6]: https://downloads.aspose.com/slides/net
[7]: https://www.nuget.org/packages/Aspose.Slides.Net
[8]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[9]: https://apireference.aspose.com/net/slides/aspose.slides.ipresentation/print/methods/1
[10]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[11]: https://apireference.aspose.com/net/slides/aspose.slides.ipresentation/print/methods/1
[12]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[13]: https://docs.microsoft.com/en-gb/dotnet/api/system.drawing.printing.printersettings?view=net-5.0
[14]: https://docs.microsoft.com/en-gb/dotnet/api/system.drawing.printing.printersettings?view=net-5.0#properties
[15]: https://apireference.aspose.com/net/slides/aspose.slides.ipresentation/print/methods/1
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/slides/net/developer-guide/
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/





