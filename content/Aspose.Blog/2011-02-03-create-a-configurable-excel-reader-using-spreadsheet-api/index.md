---
title: 'Digital Synergy Solutions is using Aspose.Cells to create a configurable Excel Reader'
date: Thu, 03 Feb 2011 15:35:45 +0000
draft: false
url: /2011/02/03/create-a-configurable-excel-reader-using-spreadsheet-api/
author: Craig Jones
summary: ''
tags: ['Aspose.Cells', 'Success Stories']
categories: ['Aspose.Cells Product Family']
---

## About Digital Synergy Solutions



{{< figure align=center src="images/digital-synergy-solutions-case-study-aspose-cells-6.png" alt="">}}


Digital Synergy Solutions specializes in web application development and vendor software integration for clients within the financial industry. When architecting a solution for a client, we first always look to the market for “best in breed” products offering the most extensive feature set, as well as solid and consistent quality and support.

## Problem

Our client built a prototype application and eventually used it to service their clients’ needs. As they signed on new clients they built bespoke conversion code to read their clients’ Excel files by either using Excel Automation or ADO.



{{< figure align=center src="images/digital-synergy-solutions-case-study-aspose-cells-1-1.png" alt="">}}


As more clients signed on to use the services of their application, they sought to deploy it to a production server-based environment. Shortly thereafter, they found Excel automation on the server troublesome and found ADO access difficult to navigate, especially when reading form-like formatted Excel worksheets, where data regions could start and end on any row for a certain column.



{{< figure align=center src="images/digital-synergy-solutions-case-study-aspose-cells-2.png" alt="" caption="<br>Example Client Format 1 – Form, where data regions start and end on any row.">}}


Our client also sought the ability to onboard more of their clients with the shortest lead time as possible.



{{< figure align=center src="images/digital-synergy-solutions-case-study-aspose-cells-3.png" alt="" caption="<br>Example Client Format 2: Simple Form">}}


## Solution

Our solution was to service enable the load and conversion of varying client formats into a standard format before load and processing into the application’s database.

We evaluated several products on the market supporting server-side Excel automation and enabling cell level reading/writing. [Aspose.Cells][1] scored the highest for the available workbook, worksheet, and cell-level access and feature support. With [Aspose.Cells documentation][2], we were able to quickly demonstrate the ease of its usage and supportability to our clients.

We centralized file conversion into a standard format using a .NET web service. To address the requirement for a more streamlined client format on-boarding process, we made the mapping from the client format to the standard format configurable using XML.



{{< figure align=center src="images/digital-synergy-solutions-case-study-aspose-cells-4.png" alt="">}}


Our biggest challenge was how to configure the read of client formats supporting varying data region start and end on any row. Our configuration supported the notion of a record Start Marker, Marker and End Marker.



{{< figure align=center src="images/digital-synergy-solutions-case-study-aspose-cells-5.png" alt="">}}


For each record definition, we used [Aspose.Cells][3] to test the cell in the defined column position (“A”) for the Start Marker Value (“Buys”). We used the Start Marker Length (“1000”) to define how many record cells would be checked before determining that the data region was not provided within the worksheet. If found the record pointer is offset by the start record value (“2”), which indicates where the data records should actually start.

The record Marker was then used to test the cell in the defined column position (“A”) for the Marker Value (“.\*”, a regular expression) to ensure it was a valid record. The fields for each valid record were then mapped into the standard format. We used a similar configuration concept and [Aspose.Cells][4] to create and write the standard Excel format (which is beyond the scope of this case study).

The End Marker was then used to test the cell in the defined position (“A”) for End Marker Value (“%NOTHING%” which we used to indicate an empty or null value cell). The End Marker Length (“1”) defined how many times the End Marker could be found before the end of the data region was determined.

The whole procedure is then repeated for each data region defined as a record in the configuration file.

Several other features of [Aspose.Cells][5] have proven useful in supporting varying source file formats, namely Excel Version support ranging from CSV and tab-delimited format to Excel 97, 2000, XP, 2003 and 2007.

## Experience

Since implementation in 2009, there has not been one production issue involving the read of varying formatted files. From almost daily issues to no issues at all is definitely attributable to the stability of [Aspose.Cells][6].

Our client has now on-boarded over 20 different source formats using our solution and has streamlined source file format onboarding from 21-40 days to a repeatable 5-10 day end to end cycle. They are now also using the solution to convert their own internal Excel file formats to other standard formats.

## Next Steps

We have since extended the solution for our client to generate varying formatted outbound files supporting configurable formulas, conditional cell values and extensive style support.

We are currently planning to extend the solution to support configurable conditional formula and/or style placement (When Then Use When Then Use Otherwise Use / When Then Use When <Some Other Condition> Then Use <Style 2> Otherwise Use <Style 3>).

## Summary

The integration of [Aspose.Cells for .NET][7] into our file management solution offering multi-source format support contributed to a successful implementation and operational phase for our client. The usability, stability and supportability of Aspose.Cells won confidence in our client’s application and ultimately our client’s confidence in us to continue to deliver solid and robust solutions.

**Craig Jones  
**Technical Consultant  
Digital Synergy Solutions




[1]: https://products.aspose.com/cells
[2]: https://docs.aspose.com/display/cellsproductfamily/Home
[3]: https://products.aspose.com/cells/family
[4]: https://products.aspose.com/cells
[5]: https://products.aspose.com/cells
[6]: https://products.aspose.com/cells
[7]: https://products.aspose.com/cells/net




