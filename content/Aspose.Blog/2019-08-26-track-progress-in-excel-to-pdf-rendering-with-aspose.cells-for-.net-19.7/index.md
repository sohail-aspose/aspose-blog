---
title: 'Track Progress in Excel to PDF Conversion in C#'
date: Mon, 26 Aug 2019 18:47:51 +0000
draft: false
url: /2019/08/26/track-progress-in-excel-to-pdf-rendering-with-aspose.cells-for-.net-19.7/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="">}}


Do you need to track your Excel to PDF conversion for bigger files? Aspose.Cells can suit your needs; it provides a sort of callback event/mechanism that notifies you the progress of the conversion. All you need to do it is implement an interface and write your code using Aspose.Cells APIs for your needs. In this post, I will share how to track your conversions for Excel to PDF rendering. Moreover, Aspose.Cells now supports to convert combo charts precisely and elegantly from XLS to XLSX and vice versa. You may find these exciting features and other enhancements in the release. So let's not wait another moment to review the [release notes][1].  To get essence of the public release ([Aspose.Cells for .NET v19.7][2], I am giving you preview of the new features and other enhancements available in it.

## C# Excel to PDF - Track Conversion Progress

Suppose, you are converting a huge Excel file to PDF, watching the loading screen and waiting for the program to finish the task. A lot of patience is required for this and you think there should be some means which shows the document conversion progress. We have achieved this functionality by providing the [IPageSavingCallBack][3] interface. Using this interface you will be able to get the total number of pages which are to be rendered to PDF along with the methods [PageStartSaving][4] and [PageEndSaving][5]. These methods should be implemented in some custom class which will continuously provide the current page number which is being rendered and the total number of pages, etc. Using this custom class you can design graphical controls or simply display text on console to show the document conversion progress page by page.

Here is a ready to run example along with a custom class sample where these methods implementation is demonstrated. Just copy this code and enjoy the new progress monitoring feature.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-LoadingSavingConvertingAndManaging-DocumentConversionProgress-1.cs" >}}

The following is the code for the _TestPageSavingCallback_ custom class.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-LoadingSavingConvertingAndManaging-DocumentConversionProgress-2.cs" >}}

Here is the sample output of the program:

_Start saving page index 0 of pages 11  
End saving page index 0 of pages 11  
Start saving page index 1 of pages 11  
End saving page index 1 of pages 11  
Start saving page index 2 of pages 11  
End saving page index 2 of pages 11  
Start saving page index 3 of pages 11  
End saving page index 3 of pages 11  
Start saving page index 4 of pages 11  
End saving page index 4 of pages 11  
Start saving page index 5 of pages 11  
End saving page index 5 of pages 11  
Start saving page index 6 of pages 11  
End saving page index 6 of pages 11  
Start saving page index 7 of pages 11  
End saving page index 7 of pages 11  
Start saving page index 8 of pages 11  
End saving page index 8 of pages 11_

Following is the summary of this new feature:

*   Get total number of pages which can be rendered
*   Get trigger when a page rendering is started with page index
*   Get trigger when a page rendering is finished with page index
*   Cancel or abort an operation at a particular page as per your requirement

## Convert XLS to XLSX with Combo Chart {#mce_0}

Older versions of Aspose.Cells were not converting the XSL to XLSX with Combo charts elegantly as these rendered charts might be flattened. The good news is that this shortcoming is no more there with the release of this new version as this issue is addressed and the charts can be rendered correctly.

Following comparisons show the results before and after this update.

The result before the update



{{< figure align=center src="images/XlsToXlsxWithChartBefore.jpg" alt="">}}


The result after the update



{{< figure align=center src="images/XlsToXlsxWithChartAfter-1024x308.jpg" alt="">}}


{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Conversion-XLSToXLSXConversion.cs" >}}  

To use these features and benefit other enhancements and fixes, I recommend you to try the release [Aspose.Cells for .NET v19.7][6]. Moreover, I recommend you to browse [Developers’ Guide][7] for your complete reference on what you can deliver using the APIs. Also, you are always welcome to share your review, concerns or feedback on [forums][8].




[1]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+19.7+Release+Notes
[2]: https://www.nuget.org/packages/Aspose.Cells/19.7.0)
[3]: https://apireference.aspose.com/net/cells/aspose.cells.rendering/ipagesavingcallback
[4]: https://apireference.aspose.com/net/cells/aspose.cells.rendering/ipagesavingcallback/methods/pagestartsaving
[5]: https://apireference.aspose.com/net/cells/aspose.cells.rendering/ipagesavingcallback/methods/pageendsaving
[6]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-19.7/
[7]: https://docs.aspose.com/display/cellsnet/Developer+Guide
[8]: https://forum.aspose.com/c/cells




