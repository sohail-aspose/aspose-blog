---
title: 'Setec generates Automatic Internal Reports for IoT Sensors and Energy Savings and Consumptions'
date: Wed, 24 Jan 2018 04:31:12 +0000
draft: false
url: /2018/01/24/generate-dynamic-reports-using-java-excel-api/
author: Pierre Eric
summary: ''
tags: ['Aspose.Cells', 'Success Stories']
categories: ['Aspose.Cells Product Family']
---

## About Setec Smart Efficiency



{{< figure align=center src="images/advizeo-by-setec.png" alt="">}}


[Setec Smart Efficiency][1] is a young French Start-up based in Paris. We are incorporated in the SETEC group, a big French engineering office at the origin of some major French infrastructures like the Channel tunnel, the engineering of many highspeed railroads, bridges, etc.

At Setec smart efficiency, our goals are to:

*   ensure our clients are making energy savings;
*   satisfy the client with comfort in his installations (monitoring humidity, temperature, CO2…);
*   help maintenance teams to detect bad behaviors in the installed material;

All these goals are reachable by putting some connected non-intrusive measure instruments providing real-time data on behalf of available IoT networks and exploiting it by using our software “Advizeo by Setec”. Our teams are composed of energy managers and developers.

## Problem

Our energy managers are accompanying our clients who are using our “SaaS solution” called Advizeo. But in order to provide a higher level of energy reporting and make clients realizing energy savings, they would like to have **specific internal tools** in order to save time which is today allocated to making some Excel-based reports.

## Solution

The solution we found to solve our energy managers' problem was to conceive software that will produce automatically the data reporting based on the data we produce through our API.

The prerequisite for the software was that **we had to use the existing Excel templates** our energy managers were filling and formatting by hand:



{{< figure align=center src="images/adviseo-aspose-cells-case-study.png" alt="" caption="Figure 1 - Example of an excel file used to summarize the data for a sensor">}}


So in order to respect this input, **we went looking for a technical solution**, a library that could meet **our requirements**:

*   Take an Excel file as input;
*   Allow inserting and manipulating pictures;
*   Allow executing formulas stored in the Excel file;
*   Allow data insertion;
*   Allow chart configuration and display;
*   Allow playing with cell formatting;
*   Allow exporting as PDF;
*   Library available in Java;
*   A library which does not require MS Office suite installed because the app will be deployed on a Linux server.

With the help of [Aspose.Cells for Java][2], we were able to integrate it in a Java console Application (using Java 1.8).

The Application connects to the database and retrieves data about buildings, then an Excel template is opened and we use [Aspose.Cells for Java][3] API to interact with the opened Workbook.



{{< figure align=center src="images/adviseo-aspose-cells-case-study-1.png" alt="" caption="<br>Figure 2 - Clearing some data in the opened template and setting the building's name information.">}}


After making many other operations we are able to re-compute all formulas and save our workbook as a new Excel file and also as a PDF file. We can also disable some sheets we do not want to display, it is very useful for the PDF output!



{{< figure align=center src="images/adviseo-aspose-cells-case-study-2-1024x570.png" alt="" caption="<br>Figure 3 - Example of file saving method using Aspose.Cells for Java">}}


At the end of the process, the files are available to the energy managers in our network filesystem.



{{< figure align=center src="images/adviseo-aspose-cells-case-study-3.png" alt="" caption="<br>Figure 4 - Another file generated as pdf output">}}


## Experience

**Finding a solution:** We first gave a look at [Aspose][4] because one of our IT Project managers has used Aspose in a company he used to work before. But we also made a comparison between other well-known tools like Crystal Reports or Jasper reports. But all these tools did not meet the target process we wanted to implement. They did not match the technical environment we wanted to use and furthermore they would have required the use of a new report editing tool that our business teams didn’t know. That is why [Aspose.Cells for Java][5] was our better option. We first use the trial version and knew we would like to take a license in order to take advantage of watermark removal and support.

**Implementation:** We first launch a POC with a Freelance person in order to test if our solution was good, then an internal developer took charge of the industrialization of the process. The POC took one week because we had a lot of internal data to retrieve in the report but the adaptation to [Aspose.Cell API for Java][6] took only a few hours in a workday.

As a developer, it is very convenient to have a library through which you can make operations in an Excel file as if you were coding VBA Macros, the cells indexes are the same. Moreover, interaction with the Excel files comes very easy like:

*   Get a specific datasheet by its name (e.g: myWorksheetCollection.get(“worksheetName”);
*   Setting a specific cell value (e.g: myCell.get(rowIndex, colIndex).setValue(myValue) );
*   Interacting through a worksheet’s pictures collection (e.g: myWorksheet.getPictures());
*   Specifying charts data source for vertical/horizontal axes: (e.g: chart.getNSeries().get(serieIndex).setXValues(worksheetDataRange) );

Another thing which is great is that cell ranges can be called as in Excel formulas (e.g: “E8:F14” or “SheetName!$E$5” ), so migrating from VBA to Java code if there were any macros inside the template file is also possible.

**Outcome:** We succeeded in testing the solution on different datasets but we are still limited by the trial version with only 100 opened files.

## Next Steps

As our initial problem was solved, we are planning to put in place more different report types using excel inputs and using [Aspose.Cells for Java][7] in these new projects but with using the Java Software to bin the data to the report.

We also plan to buy a license for [Aspose.Cells.for Java][8] in order to replace the trial version and benefit from all the features without limitations because the trial version put watermarks on pdf and excel files and the limit for opened files is 100.

## Summary

We would recommend the use of [Aspose.Cells for Java][9] because it is easy to implement and the API is simple to understand and very fluent. The only thing we perhaps regret is the price of the library which is not very affordable for a start-up. Nevertheless, for a company with a higher budget, it will not be a problem.




[1]: https://www.setec.fr/en/
[2]: https://products.aspose.com/cells/java
[3]: https://products.aspose.com/cells/java
[4]: https://www.aspose.com/
[5]: https://docs.aspose.com/display/cellsjava/Home
[6]: https://docs.aspose.com/display/cellsjava/Home
[7]: https://products.aspose.com/cells/java
[8]: https://products.aspose.com/cells/java
[9]: https://products.aspose.com/cells/java




