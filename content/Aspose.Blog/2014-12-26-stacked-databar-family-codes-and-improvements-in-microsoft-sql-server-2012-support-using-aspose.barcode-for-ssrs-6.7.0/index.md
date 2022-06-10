---
title: 'Stacked DataBar Family Codes and Improvements in Microsoft SQL Server 2012 Support using Aspose.BarCode for SSRS 6.7.0'
date: Fri, 26 Dec 2014 23:08:59 +0000
draft: false
url: /2014/12/26/stacked-databar-family-codes-and-improvements-in-microsoft-sql-server-2012-support-using-aspose.barcode-for-ssrs-6.7.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.BarCode Product Family']
---

We are pleased to announce the release of Aspose.BarCode for SSRS 6.7.0. This release brings important changes in perspective of new symbologies support, full support of Microsoft SQL Server 2012 and other updates regarding Visual Studio 2012. We have also fixed a few internal errors. These errors were impacting the barcode visibility on the report server.

## Support of DataBar Stacked, DataBar Expanded Stacked, DataBar Omnidirectional Stacked and Patch Code

We have added support of stacked codes those are part of DataBar symbologies.

1.  **DataBar stacked** is a variation of the RSS-14 symbology that is stacked in two rows and is used when the normal symbol would be too wide for the application.
2.  **DataBar expanded stacked** barcode can grow vertically, it can encode a large amount of data in small space.
3.  **DataBar omnidirectional stacked** is perfectly suitable for POS (point of sale) applications.
4.  **Patch codes** are a set of 6 distinct barcode patterns (1, 2, 3, 4, 6 and T) that are typically used as document separators when scanning.

## Improvements in Microsoft SQL Server 2012 Support

For Microsoft SQL Server 2012, we have provided two assemblies. First "Design Version" works only with designers (Visual Studio or BIDS). This assembly is located in the Bin\\SSRS2012\\DesignVersion directory. Second "RunTimeVersion" works only with Server. This assembly is located in the Bin\\SSRS2012\\RunTimeVersion directory. We've updated manual installation docs as well. Please check: Install Manually

## Visual Studio 2012 Updates

Toolbox in Visual Studio 2012 can't detect any report component, but we can work with a report with Barcode component in Visual Studio 2012 without problem. The main problem is, how to put Barcode component to report and there are two ways:

1.  Create a report in Visual Studio 2010 and next open this report in Visual Studio 2012 and work with report.
2.  Add Barcode component to report manually in code. For this need open report code (View Code) and put into <ReportItems> element:```
     <CustomReportItem Name="BarCode1">
    
        <Type>BarCode</Type>
    
    </CustomReportItem> 
    ```
    
    after this we can switch to "View Designer" and work with barcode component.
    

This new release also includes a fix of caption text alignment.  The alignment settings were not working perfectly.

To view a complete list of API features and try the API, please visit the following page and [download the latest version of Aspose.BarCode for SSRS][1]. If you need any help, please feel free to ask in the [Aspose.BarCode forum][2]. For more details, please visit the Aspose.BarCode for SSRS documentation.




[1]: http://www.aspose.com/community/files/52/ssrs-rendering-extensions/aspose.barcode-for-reporting-services/default.aspx
[2]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx




