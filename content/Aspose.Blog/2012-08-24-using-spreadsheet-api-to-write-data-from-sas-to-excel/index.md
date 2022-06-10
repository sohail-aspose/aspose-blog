---
title: 'Gjensidige supported highly advanced Data Export from SAS to Excel using Aspose.Cells for .NET'
date: Fri, 24 Aug 2012 15:02:37 +0000
draft: false
url: /2012/08/24/using-spreadsheet-api-to-write-data-from-sas-to-excel/
author: Bjarke Felbo
summary: ''
tags: ['.NET API for data export to Excel', 'Advance data export to Excel format in .NET Application', 'Aspose.Cells', 'Data Export from SAS to Excel using Aspose.Cells for .NEt', 'Memory Efficient data export to Excel', 'Success Stories']
categories: ['Aspose.Cells Product Family']
---

## About Gjensidige Insurance



{{< figure align=center src="images/500px-Gjensidige_Logo.svg_.png" alt="">}}


Gjensidige Insurance is a multinational insurance company, which primarily is located in Scandinavia. The team of Analysis Denmark consists of 12 members, who examine and manipulate huge amounts of data. This data is turned into easily understandable graphs and sheets using Excel sheets or other similar tools. Many leaders throughout the company then examine this material and use it to better lead the company in the right direction.

## Problem

We have been using a SAS server for processing our SAS applications and we needed it to output our data to Excel in a more advanced way than the SAS software allowed us to do. Furthermore, we needed it to be able to do so efficiently and without errors. We were a bit puzzled by which solution would be the best, but a simple C# application and a flat data file (.txt) seemed to work out quite well.

## Solution

We chose [Aspose.Cells for .NET][1] as it seemed like a professional product that simply worked without any issues. The input from SAS data that was written to a flat .txt file by SAS, which was then read by our C# .NET application.

Below is an example of such a text file:



{{< figure align=center src="images/sas-to-excel-case-study-aspse-cells.png" alt="Data representation in Text file">}}


This data was then inserted into an Excel template using our .NET application and [Aspose.Cells for .NET][2]. The issue concerning the right Excel solution for us was whether it could support our highly advanced Excel sheets with plenty of macros etc.



{{< figure align=center src="images/sas-to-excel-case-study-aspse-cells-1.png" alt="Preview of Filtering Solution in Excel format" caption="<br>An example of one of our filtering solutions in Excel that we needed Aspose.Cells to handle">}}


We also needed it to not cause any issues with our SAS applications if any errors were encountered. Another important criterion was the ability to handle Excel sheets with a high amount of data without using a great deal of the server’s memory. Instead of having the usual approach of opening an entire Excel workbook, insert data into all worksheets and then save it, we chose to insert data into only one worksheet at a time. While this made performance worse, it helped prevent errors. After all, stability is the most important criteria for us.

## Experience

### **Finding a solution**

When we first contacted Aspose, we had been using Bytescout Spreadsheet SDK for 10 months. However, its performance was not good enough for us seeing as the output of a large Excel file could almost cause our server to halt. When using Bytescout Spreadsheet SDK with one of our larger outputs with more than 100.000 rows and 20 columns, the memory usage used to climb until the program crashed at around 1,5-2 gigabytes of allocated memory. However, once we switched to [Aspose.Cells for .NET][3], the memory for writing the same amount of data climbed steadily to around 700 megabytes and at that point, it used to stop.

### **Implementation**

The transition from Bytescout Spreadsheet SDK to [Aspose.Cells for .NET][4] was extremely easy and took less than a day. There were no substantial challenges with using [Aspose.Cells for .NET][5]. We were worried concerning our large amounts of data, macros, and formatting, but [Aspose.Cells for .NET][6] handled all of those without any issues at all.

### **Outcome**

The outcome has been that we were able to let our servers handle all of our needs concerning the output of data from SAS to Excel and we did not encounter any errors while using [Aspose.Cells for .NET][7].

## Next Steps

We do not currently have any plans to take our solution further. However, we are thinking of ways to use Aspose’s products in order to directly output our data into other kinds of files such as PDF documents.

## Summary

[Aspose.Cells for .NET][8] easily handled even large Excel sheets that would end up and did so extremely fast. Additionally, it handled all of our macros without any issues at all. We would therefore definitely recommend [Aspose][9] seeing as their product has handled all of our needs seamlessly without any real effort from our side.




[1]: https://products.aspose.com/cells/net
[2]: https://products.aspose.com/cells/net
[3]: https://products.aspose.com/cells/net
[4]: https://products.aspose.com/cells/net
[5]: https://products.aspose.com/cells/net
[6]: https://products.aspose.com/cells/net
[7]: https://products.aspose.com/cells/net
[8]: https://products.aspose.com/cells/net
[9]: https://www.aspose.com/




