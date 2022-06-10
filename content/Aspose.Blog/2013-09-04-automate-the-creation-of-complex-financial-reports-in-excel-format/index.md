---
title: 'The Digital Group Automated the creation of complex financial reports in Excel format using Aspose.Cells for .NET'
date: Wed, 04 Sep 2013 14:10:25 +0000
draft: false
url: /2013/09/04/automate-the-creation-of-complex-financial-reports-in-excel-format/
author: The Digital Group
summary: ''
tags: ['Aspose.Cells', 'Success Stories']
categories: ['Aspose.Cells Product Family']
---

## About The Digital Group (T/DG)



{{< figure align=center src="images/logo.png" alt="">}}


The Digital Group (T/DG) is a premier provider of information technology services with extensive expertise in all facets of software development. With capabilities at all points of the software life-cycle, we can provide support from concept to development to operations. For the last decade, our teams have been delivering industry-leading solutions for our customers.

The Digital Group, with its headquarters in Princeton, New Jersey, was incorporated in 1999 having a global talent pool of top-notch professionals providing technology and management consulting services and solutions, with offices in the US, India, Fiji, and Australia. TDG’s Services & Solutions delivery capability is anchored in an integrated set of core competencies that span, people, processes and technology coupled with practice competencies in System Administration, Web Software Engineering, Enterprise Applications, Enterprise Integration, Corporate Compliance, and Legacy Migration. We provide a cost-optimized global delivery model with onsite, near-site and off-shore capabilities.

## Solution

One of our clients had a requirement to automate the generation of Complex Financial reports in Excel format. Considering the complexity of Reports and required performance criteria, the Technical team evaluated a few options and the final decision has to be made between a couple of options before finalizing the solution. Options were –

1.  [Aspose.Cells for .NET][1] (7.5.2)
2.  Microsoft.Office.Interop.Excel

We decided to do a POC of a small part of the functionality with the above two options. Functionality was, data tabled data had to be extracted from the dataset and exported to an Excel sheet.

### **How did it work?**

**Aspose**: For exporting data to Excel we have used [Aspose.Cells for .NET][2], which provides the most flexible group of components that enable .NET applications to create and manage Excel® spreadsheets without requiring Microsoft Excel® to be installed on the server.

It has **ImportDataTable** method that imports a System.Data.DataTable object into a worksheet. We just need a few lines of code to get the export data task done.



{{< figure align=center src="images/The_Digital_Group_uses_Aspose.Cells_for_.NET_in_preference_to_INTEROP.png" alt="">}}


With **INTEROP**, the same task is done using looping which takes more time in completing the task.

So we were required to loop through the data table columns and rows and write data to cells in an Excel sheet.



{{< figure align=center src="images/The_Digital_Group_uses_Aspose.Cells_for_.NET_in_preference_to_INTEROP-1.png" alt="">}}


Following is the result of a comparison made between both approaches.

We ran the test with a different number of records and noticed the time difference between ASPOSE and INTEROP.

#### **Scenario 1**

To export 2500 records ASPOSE took ‘0.7252908’ seconds where INTEROP took 2 minutes.



{{< figure align=center src="images/The_Digital_Group_uses_Aspose.Cells_for_.NET_in_preference_to_INTEROP-2.png" alt="Performance of data export using Aspose.Cells for .NET">}}


#### **Scenario 2**

To export 1050 records ASPOSE took ‘0.7243860’ seconds where INTEROP took 55 seconds.



{{< figure align=center src="images/The_Digital_Group_uses_Aspose.Cells_for_.NET_in_preference_to_INTEROP-3.png" alt="Performance for data export using Aspsoe.Cells for .NET">}}


#### **Scenario 3**

To export 5014 records ASPOSE took ‘0.9859248’ seconds where INTEROP took 5 Minutes and 19 seconds.



{{< figure align=center src="images/The_Digital_Group_uses_Aspose.Cells_for_.NET_in_preference_to_INTEROP-4.png" alt="Third scenario to export data using Aspose.Cells for .NET">}}


## Experience

Excel Financial Report generation was one of the core functionality of the project. Requirement was to have flexible financial report output with Performance as a crucial factor. Project timeline was tight as well. We were looking for a solution which not only meets all requirements but also saves development time.

After POC, We figured out that [Aspose.Cells for .NET][3] was the best fit with below highlights,

### **Functional Features**

We can perform a variety of Excel operations like:

*   _[Worksheet scope][4]_ – Add, Remove Rename worksheet. Sorting data, managing hyperlinks, pictures, comments.

*   _[Row-Column scope][5]_ – We generated rows and columns with financial data for multiple years.

*   Operations like Hide/Unhide, Freeze/Unfreeze, formatting of entire Row/Column can be easily performed.

*   _Cell scope_ – Populating values, [setting formula][6], Formatting, Replacing values in Cells or Range of cells can be achieved with ease. Even cells can merge/unmerged or use of Named ranges is possible.

### **Performance**

As showcased above Aspose was a clear winner in performance. Time taken to generate Thousands of rows with considerable columns was less than a second. All the above functional features can be achieved with great operational speed for a higher number of rows/columns.

### **Availability & Support**

We used the [Free Trial version][7] of [Aspose.Cells for .NET][8] for a feasibility check. It was easily available from Aspose. We discussed with [Aspose Support][9] representative regarding licensing queries and concluded on required license type and number. Aspose suggested Developer OEM license which met all requirements with optimized cost.

We also did not require to install Microsoft Office on the Aspose server.

### **Rapid Development**

We noticed that to achieve particular functionality, the line of code required using Aspose is lesser than other options.

Aspose has a smooth Learning curve as the developer completed the POC within a couple of Days. There are samples available on the Aspose site almost for all functional features which were helpful. Overall it resulted in reduced Development efforts and invariably time.

We recommended the client to use Aspose as it was a clear winner in performance & features.

## Next Steps

In our project, we used [Aspose.Cells for .NET][10]. We also decided that going forward, we will be considering to evaluate other [Aspose products][11] wherever applicable.

We also have been using Aspose products for a couple of other clients where the client himself has recommended for [Aspose][12].

## Summary

We concluded on below points

*   The INTEROP approach was taking a significant amount of time as compared to ASPOSE. The performance was better in ASPOSE.
*   ASPOSE required fewer lines of code as compared to INTEROP which requires more coding which involves looping.
*   You require to purchase a separate license for ASPOSE whereas there is no additional license required for INTEROP.

[Aspose.Cells for .NET][13] was the best fit for our project requirement due to its performance & features.

As mentioned earlier, developers can easily pick up on Aspose details, thanks to the smooth learning curve and Samples available on the Aspose site itself. Using Aspose, we are able to save some amount of development efforts as well.

[Aspose][14] team was supportive throughout the POC and implementation.

Our development team was satisfied with the ease, performance, and reliability of [Aspose products][15]. We did finalize Aspose for future implementation for this client as well as recommended Aspose products to other development teams. Last but not the least, we would like to recommend Aspose components whenever it fits with your requirements.




[1]: https://products.aspose.com/cells/net
[2]: https://products.aspose.com/cells/net
[3]: https://products.aspose.com/cells/net
[4]: https://docs.aspose.com/display/cellsnet/Worksheets
[5]: https://docs.aspose.com/display/cellsnet/Rows+and+Columns
[6]: https://docs.aspose.com/display/cellsnet/Formulas
[7]: https://downloads.aspose.com/
[8]: https://products.aspose.com/cells/net
[9]: https://forum.aspose.com/c/cells
[10]: https://products.aspose.com/cells/net
[11]: https://products.aspose.com/
[12]: https://www.aspose.com/
[13]: https://products.aspose.com/cells/net
[14]: https://www.aspose.com/
[15]: https://products.aspose.com/




