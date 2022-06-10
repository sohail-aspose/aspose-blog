---
title: 'Previso Added Economic Modelling Capability to its Gas Forecasting Application with Aspose.Cells'
date: Fri, 21 Jun 2019 08:01:36 +0000
draft: false
url: /2019/06/06/economic-modeling-capability-within-forecasting-application/
author: Francesco Senatore
summary: ''
tags: ['Success Stories']
categories: ['Aspose.Cells Product Family']
---

## About Previso Software



{{< figure align=center src="images/Previso-Logo-3-1024x200.jpg" alt="Previso company logo">}}


[Previso][1] has created a comprehensive upstream oil and gas production forecasting tool that is a truly integrated modeling solution from “reservoir to market”.

What is unique about Previso’s approach is that the forecast is ‘market-driven’. Production is tracked on a component basis and back-allocated through the processing plants, pipelines, compressors, wells and, finally, each reservoir.

Gas production can be constrained and hydrocarbon liquids optimized based on multiple and complex market demands. The production constraints, prioritization, scheduling and event triggering can be as complex as required.

## Introduction

[Aspose.Cells for .NET][2] is an [Excel programming API][3] that offers easy and fast spreadsheet management suited for quickly processing large amounts of data in an Excel file, as well as a robust formula calculation engine capable of calculating the results of entire workbooks without relying on Microsoft Excel to be installed.

The Previso software is a well-established solution in the upstream gas forecasting space. The output from the software (gas forecasts by market) almost always ends up in a separate economic model to understand the final “value” of the project. With Aspose.Cells, Previso was able to quickly add spreadsheet modelling capability for economics that was not only very flexible but also tightly integrated into the solution.

## Problem

Previso planned to add economic functionality to its solution; however, a traditional development exercise, with bespoke functionality, would mean tedious and time-consuming development. It would also be a hard sell in the market, as the bulk of the client economic models are written in Excel due to its inherent flexibility and audibility. An Aspose solution allowed the modelling to continue in Excel, but with the spreadsheet tightly integrated into the main application.

This new functionality provided the users with the ability to use economic results (net present value, rate of return, payout etc) within the software’s scenario decision making capability. Early market testing with existing clients demonstrated that the tightly coupled economic solution with Aspose would be well received.

## Solution

Aspose.Cells forms the core part of Previso 5.0's economics capability. Firstly, an Excel file ('economic modelling template') is imported and stored as part of Previso's project file. Any subsequent changes to the Excel file require a reload of the file in order to refresh the project's economics template. Other than the spreadsheet load, there is no requirement to go back to Excel after the load or refresh. During the import, a set of metadata is created for each of the template's worksheets containing information about the sheet's structure, such as cell addresses of all input and output cells, among other things. Previso matches product worksheets to their corresponding markets by name. Supporting worksheets that don’t have a matching market in the project file are ignored, and vice versa.

Secondly, input data from Previso (e.g. product prices, tax rates, capital, and operating costs), along with additional data gathered from simulation results (such as product rates), are used to populate the workbook at run time, and afterwards passed to Aspose.Cells' calculation engine for the actual calculation. It should be noted that at no time does Previso rely on the native Excel spreadsheet calculation. All of the spreadsheet functionality is available through the Aspose calculation engine at runtime. There is no linking to an Excel file somewhere on the network that could be changed, corrupted, or go missing when it was needed.

**_All of the spreadsheet functionality is available through the Aspose calculation engine at runtime. There is no “linking” to an Excel file somewhere on the network that could be changed, corrupted, or go missing when it was needed._**

Finally, results are read from the workbook and displayed in a variety of reports. Additionally, the raw results can be exported with the complete data set and calculations in an Excel file for auditing purposes. Previso also offers the option to automatically calculate economics results every time a new simulation is run.



{{< figure align=center src="images/aspose-cells-previso-case-study.png" alt="" caption="Previso Spreadsheet Integration and Economic Workflow">}}


## Summary

Using Aspose.Cells, Previso has quickly and comprehensively added economic modelling capability to its gas forecasting application. The integration is fast and seamless. Users can build a standard economic model in Excel, which is in turn stored within the Previso application. At runtime, the spreadsheet can be run within the Previso software to generate economic results. As an added benefit, the users can also export the spreadsheet back out in order to pass on or audit the calculations.




[1]: http://www.previso.net/
[2]: https://products.aspose.com/cells/net
[3]: https://products.aspose.com/cells/family




