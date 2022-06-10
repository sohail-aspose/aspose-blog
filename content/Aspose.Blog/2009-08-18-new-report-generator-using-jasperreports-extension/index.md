---
title: 'AGE web solutions Srl Uses Aspose.Words for JasperReports for Report Generation'
date: Tue, 18 Aug 2009 11:18:43 +0000
draft: false
url: /2009/08/18/new-report-generator-using-jasperreports-extension/
author: Matteo Tassinari
summary: ''
tags: ['Aspose.Words', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About AGE web solutions Srl



{{< figure align=center src="images/Age-Web-Solution.jpg" alt="">}}


AGE web solutions Srl operates in the field of working security and safety and has developed the "626Suite", a complete software tool aimed to aid the users in the compilation and management of the Document for Risk Evaluation, which is a mandatory legal document for every Italian company, written to asses and evaluate every possible risk which may come to harm to any worker of the company.

This tool is a web-based application that gathers a huge amount of data about the working conditions in a company and needs to generate well-designed reports of all the data inserted by the user. Such reports were formerly created using the JasperReports tools, which lacks some of the most important features we need.

Thanks to Aspose.Words for JasperReports, it is possible to build a completely new report engine without the need of replacing all the report templates which have been created over the past years.

## Requirements

In order to obtain easily editable reports containing the data of the Document for Risk Evaluation, 626Suite requires a way to natively generate reports in DOC or DOCX format instead of the position-based RTF format.

Also, in order to reduce development costs, it is also necessary to keep the underlying print engine and report templates, to avoid completely redo them from scratch.

## Solution

In our search for a solution capable of generating an easily editable Document for Risk Evaluation, we found that [Aspose.Words for JasperReports][1] fully meets our functional requirements: it allows our program suite to generate reports natively in DOC and DOCX format, while allowing us to maintain the original print engine and report templates, so avoiding the costs which we would have sustained if we had to create a new engine from scratch.

Thanks to [Aspose.Words for JasperReports][2] functionalities our software suite is capable of creating well-formed reports which can be easily modified by our final customers, without compromise on the report quality, even for the more complex ones.

The new version of the print engine relies on some servlets running on top of the tomcat service our suite is based on. Each servlet can manage a certain kind of report, and the two servlets which generate the full final reports (the main document and the “Attachment” document) also use Aspose.Words for Java functionalities to merge together all the single reports generated during the print step.

The printing procedure of a single module follows these steps:

*   The servlet is launched with all required parameters
*   The template is compiled and filled with data from the database source
*   The report is exported in the selected format

At the end of these three steps, a single document is generated. All these documents need to be merged into a single one in order to create the final Document for Risk Evaluation.

## Experience and Benefits

Aspose.Words for JasperReports delivers all the desired functionalities with minimal implementation, integration and maintenance efforts. It also performed really well in all our print tests, including those required to print the final document, which is usually about 300 pages long.

Key benefits are:

*   easy integration with the original 626Suite print engine, which is based on JasperReports and tomcat to dynamically compile and fill the report templates
*   easy of use and implementation: it just requires to change a few lines of code in our servlets
*   well-organized and useful documentation

## Conclusion

626Suite was created to help our customers in the creation and management of the Document for Risk Evaluation for their company.  
Thanks to Aspose.Words for JasperReports, it is now possible for them to generate a fully-editable document instead of the old position-based RTF version, which makes the maintainability of the Document itself much greater, also ensuring its legal value.

The experience with this Aspose product has been more than positive so far, thanks to its ease of use and simplicity, and we are considering its use in more projects to come.



{{< figure align=center src="images/age-web-solutions-case-study-aspose-words.png" alt="" caption="Screenshot showing a glimpse of the user interface of 626Suite">}}


**Matteo Tassinari  
**AGE web solutions Srl




[1]: https://products.aspose.com/words/jasperreports
[2]: https://products.aspose.com/words/jasperreports




