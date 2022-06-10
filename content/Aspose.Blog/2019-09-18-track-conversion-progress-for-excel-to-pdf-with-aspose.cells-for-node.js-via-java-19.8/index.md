---
title: 'Convert Excel to PDF - Track Conversion Progress in Node.js'
date: Wed, 18 Sep 2019 11:26:53 +0000
draft: false
url: /2019/09/18/track-conversion-progress-for-excel-to-pdf-with-aspose.cells-for-node.js-via-java-19.8/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-nodejs-150x150.png" alt="">}}


Do you want a feedback mechanism while huge Excel files are converted to PDF? Great! Get the latest enhanced version of [Aspose.Cells for Node.js via Java 19.8][1] to use this exciting feature by adding just a few lines of codes.

We are happy that once again we got the chance to present an updated and enhanced version of Aspose.Cells for Node.js via Java v19.8. This time we have added new features for processing the ODS file background to create more user-friendly output files having color and image in the background. We have also enhanced our rendering features to HTML, PDF and improvements in many functions of common use. Well, I think rather than writing a lot about these features one by one, better to have a brief overview of the new version from the [release notes][2] and then start exploring this release. What do you say?

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

Following comparisons show the results before and after this update.

The result before the update



{{< figure align=center src="images/XlsToXlsxWithChartBefore.jpg" alt="">}}


The result after the update



{{< figure align=center src="images/XlsToXlsxWithChartAfter-1024x308.jpg" alt="">}}


{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Conversion-XLSToXLSXConversion.java" >}}  

**Important To Know**

As we already announced that Aspose.Cells for JavaScript via Java has been renamed to Aspose.Cells for Node.js via Java now. Aspose.Cells for Node.js via Java is a subset component that includes all the important and useful features present in its native Aspose.Cells for Java. Aspose.Cells for Node.js via Java presents all the useful features of Aspose.Cells for Java using Node.js. It is a class library that enables you to perform a great range of spreadsheet processing tasks. Aspose.Cells for Node.js via Java is a scalable and feature rich API that offers spreadsheet format conversion, styling of worksheets at every level, chart management & rendering, and our reliable Formula Calculation Engine.

Please note, The APIs structure still remains the same, so it won’t disturb our existing clients who can still use the APIs without any changes in the code. We have revamped the [Wiki Conf. Docs][3] accordingly. We have also changed Aspose.Cells for JavaScript via Java node to Aspose.Cells for Node.js via Java in [Downloads][4] section. Moreover, the product pages are now updated. Similarly [API Reference][5] section for the product and other important areas are already accommodated accordingly.

So what are you waiting for? Open your IDE and start testing these new features using this latest release [Aspose.Cells for Node.js via Java 19.8.][6] You may also consult the [Developer's Guide][7] for all the details of Aspose.Cells and if need a ready to run project with all the examples, just click [here][8] and download the project from GitHub. [Forums][9] are there for assisting you and answering all your queries about this product.




[1]: https://downloads.aspose.com/cells/nodejs
[2]: https://docs.aspose.com/cells/java/aspose-cells-for-node-js-via-java-19-8-release-notes/
[3]: https://docs.aspose.com/cells/java/
[4]: https://downloads.aspose.com/cells/nodejs
[5]: https://apireference.aspose.com/nodejs/cells
[6]: https://downloads.aspose.com/cells/nodejs/new-releases/aspose.cells-for-node.js-via-java-19.8/
[7]: https://docs.aspose.com/cells/java/
[8]: https://github.com/aspose-cells/Aspose.Cells-for-Java
[9]: https://forum.aspose.com/c/cells




