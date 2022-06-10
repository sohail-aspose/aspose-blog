---
title: 'Convert Excel to PDF in PHP - Track Conversion Progress'
date: Wed, 25 Sep 2019 18:30:16 +0000
draft: false
url: /2019/09/25/track-conversion-progress-for-excel-to-pdf-with-aspose.cells-for-php-via-java-19.8/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose.cells-for-php-via-java-128-e1534155845486.png" alt="">}}


Need to track conversion process while huge Excel files are being converted to PDF? Get the latest enhanced version of [Aspose.Cells for PHP via Java 19.8][1] to use this exciting feature by adding just a few lines of codes. We present an updated and enhanced version of Aspose.Cells for PHP via Java v19.8. This time we have added new features for processing the ODS file background to create more user-friendly output files having color and image in the background. We have also enhanced our rendering features to HTML, PDF and improvements in many functions of common use. Let me present a brief overview of the new version from the release notes and start exploring this release. What do you say? Here you are.

## Track Conversion Progress

You are converting a huge Excel file to PDF, watching the loading screen and waiting for the program to finish the task. A lot of patience is required for this and it seems that there should be something which shows the document conversion progress. That's it. We have achieved this functionality by providing the IPageSavingCallBack interface. Using this interface you will be able to get the total number of pages which are to be rendered to PDF along with the methods PageStartSaving and PageEndSaving. These methods should be implemented in some custom class which will continuously provide the current page number which is being rendered and the total number of pages. Using this custom class you can use a variety of graphical controls or simply display text in a console application to show the document conversion progress page by page.

Here is a ready to run example along with a custom class sample where these methods implementation is demonstrated. Just copy this code and enjoy the new progress monitoring feature.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-LoadingSavingConvertingAndManaging-DocumentConversionProgress-1.java" >}}

The following is the code for the _TestPageSavingCallback_ custom class.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-LoadingSavingConvertingAndManaging-DocumentConversionProgress-2.java" >}}

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

Older versions of Aspose.Cells were not converting the XSL to XLSX with Combo charts properly as these charts were being flattened. The good news is that this shortcoming is no more there with the release of this new version as this issue is addressed and the charts can be rendered correctly.

The following comparisons show the results before and after this update.

The result before the update



{{< figure align=center src="images/XlsToXlsxWithChartBefore.jpg" alt="">}}


The result after the update



{{< figure align=center src="images/XlsToXlsxWithChartAfter-1024x308.jpg" alt="">}}


{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Conversion-XLSToXLSXConversion.java" >}}

## Aspose.Cells for PHP via Java Resources

The following are the links to some useful resources you may need to accomplish your tasks.

*   [Aspose.Cells for Java Online Documentation][2] (Aspose.Cells for PHP via Java is ported from Aspose.Cells for Java. So, you can use the same documentation)
*   [Features][3]
*   [Release Notes][4]
*   [Download Aspose.Cells for PHP via Java][5]
*   [API Reference Guide][6]
*   [Free Support Forum][7]
*   [Paid Support Helpdesk][8]




[1]: https://downloads.aspose.com/cells/php/new-releases/aspose.cells-for-php-via-java-19.8/
[2]: https://docs.aspose.com/cells/phpjava/
[3]: https://docs.aspose.com/cells/java/aspose-cells-for-php-via-java-features/
[4]: https://docs.aspose.com/cells/#asposecells-for-php-via-java-resources
[5]: https://downloads.aspose.com/cells/php
[6]: https://apireference.aspose.com/php/cells
[7]: https://forum.aspose.com/c/cells
[8]: https://helpdesk.aspose.com/




