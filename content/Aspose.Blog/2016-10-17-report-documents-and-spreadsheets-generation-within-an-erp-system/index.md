---
title: 'Fermator Empowered ERP solution for Dynamic Report Generation in MS Word and SpreadSheets Format using  APIs'
date: Mon, 17 Oct 2016 17:48:00 +0000
draft: false
url: /2016/10/17/report-documents-and-spreadsheets-generation-within-an-erp-system/
author: Andreu Garcia
summary: ''
tags: ['.NET API for MS Word files processing', 'Aspose.Total', 'Aspose.Words', 'Dynamic report generation in MS Word format', 'Manipulate MS Word files using Aspose.Words for .NET', 'Programatically process MS Word files', 'Render MS Word files to PDF format', 'Report generation based on MS Word template', 'Success Stories']
categories: ['Aspose.Words Product Family', 'Aspose.Total Product Family']
---

## About Fermator Group



{{< figure align=center src="images/LogoFerm.png" alt="Fermator logo">}}


[Fermator Group][1] is the largest mono-product manufacturer of automatic doors for lifts in the world. Fermator doors are installed worldwide for light, medium and heavy traffic duty lifts, for domestic use, offices, airports, hotels, and public buildings. With headquarters in Spain and production plants located in France, Italy, Poland, Greece, India, China, and Brazil, the Fermator Group responds effectively to the demands of all markets requiring automatic doors for lifts.

Since the first manufacturing plant started operations, the company decided to have its own ERP system, with an intent to respond quickly to a market in constant evolution. This system has been in use for more than twenty years and now, although the strategy is still valid, the group has changed a lot (_new companies, new markets, new processes, new products…_) and requires a new ERP.

My team was responsible for developing a new ERP system, based on .NET technology and following agile methods. The scope of this ERP had to cover all the business processes included in the value chain of the company (_sales, planning, supply chain, manufacturing, assembly, shipment and invoicing), and other cross-activities (like quality, human resources, and IT management, among others_).

## Problem

We faced four main types of requirements related to reporting:

*   **Reports generation** – Our system will have to generate simple documents (_like invoices or packing lists, with a master & detail structure_), but also complex ones (_like assembly orders, with some schemas generated dynamically when the report is built_).
*   **Document generation** – Some times, the information in the system has used as a starting point to elaborate an editable document. That has been the case for quotes (sales people get a first version of the commercial quote from the system and complete it with particular conditions for each negotiation). Another example was the "model specification" document which was a vision of all the configurable characteristics available for each door type and model.
*   **Spreadsheets generation** – Another need to be solved was the spreadsheets generation. It might be a simple export of the visualized data in a grid, or complex reports in a spreadsheet format to cross information from several sources.
*   **Labels generation** – Our ERP supports also all our manufacturing processes. Many times, these are based on identification labels, which are read by workers with hand-held scanners. This implies bar codes generation (_when the space in the label or the document is not limited_) or bi-dimensional codes (_we have used QR codes_) when the label has reduced dimensions.

As a summary, reports were used almost by anyone in the company; documents, by the sales and engineering departments; spreadsheets, by the management and direction levels; and labels, by everyone on the shop floor.

## Solution

We tested [Aspose.Words for .NET][2] and other tools, and [Aspose.Words for .NET][3] really convinced us. We were able to define a number of Microsoft Word templates, which, nested together, make a stack of documents to generate a really professional set of reports.

This implementation (_the templates stack_) is useful to decouple the header, footer, table of contents, and other blocks of our reports. Thus, we can reuse them as building blocks and maintain these parts easily with one single update.

All the system reports have a parameter, where we define the method to be invoked to generate each report.



{{< figure align=center src="images/Fermator-Group-aspose-total-case-study.png" alt="Reports parameterisation preview" caption="Image 1:- Reports parameterization.">}}


From many places within the application, the user can click on a printer button, getting a list of available reports for that given context. When the user selects on one of these reports, the parametrized method is invoked and the report generated using the [Aspose libraries][4].



{{< figure align=center src="images/Fermator-Group-aspose-total-case-study-1.png" alt="Report generation using Aspose Libraries" caption="Image 2:- Generating the document.">}}


Then, the user will see an application window with the report in PDF format. From here, he will be able to send it directly to his default printer or to save it as PDF, DOCX or ODT. This part is not developed yet, but we have done a concept test and it will work.

## Experience

### **Finding a solution**

We have strong knowledge in our team about reporting with MS Access and with MS SQL Server Reporting Services. As we are in a process to change from Access to .NET, we thought Access was not an option. On the other hand, Reporting Services is excellent to make charts and user-defined reports, but we needed a quick response and a wide variety of output formats.

The sales support and [product support teams from Aspose][5] helped us in this phase of the process, and it was straightforward to try and check the product features.

### **Implementation**

We installed a fully functional license in a couple of hours. There was a learning curve to generate some reports. This was probably the toughest stage. We dedicated one person for a week to investigate the potential of the tool.

Once we were able to generate three or four types of reports, the knowledge was shared with all the team members and they became productive in a couple of days. We are really surprised by the number of examples we can find on the [technical web pages][6], GitHub solution, and [forums from Aspose][7].

### **Outcome**

In the end, we have what we were looking for. A powerful tool, highly customizable, easy to learn (_if you have got minimal knowledge about MS Word and .NET framework_), and very quick. We will be able to generate reports faster than with MS Reporting Services and, what is most important, with almost no limitation. If you can do it with MS Word, you will be able to do it with [Aspose.Words for .NET][8].

## Next Steps

We have only tried [Aspose.Words for .NET][9], but, as we described in the requirements section, we will have to generate reports in spreadsheet formats and barcodes. We have no doubt [Apose.Total for .NET][10] will fit our requirements, so we are betting directly for the whole package.

## Summary

As a summary, we can only say one thing: excellent product and excellent service. Sometimes, you can find a good product with a lack of customer care. This is not the case for [Aspose][11]. Examples are available and [technical support][12], diligent.

You can even set up a reporting team with different professional levels and skills (_designers and programmers_) to build your reports by phases, getting user approval after investing just the time you require to write an MS Office document and be sure you will be able to get the same output when it comes to programming.

We definitely recommend [Aspose.Words for .NET product family][13]. It is powerful, fast, and easy to learn.




[1]: http://www.fermator.com/
[2]: https://products.aspose.com/words/net
[3]: https://products.aspose.com/words/net
[4]: https://products.aspose.com/total/net
[5]: https://forum.aspose.com/
[6]: https://docs.aspose.com/display/totalnet/Home
[7]: https://forum.aspose.com/
[8]: https://products.aspose.com/words/net
[9]: https://products.aspose.com/words/net
[10]: https://products.aspose.com/total/net
[11]: https://www.aspose.com/
[12]: https://forum.aspose.com/
[13]: https://products.aspose.com/words/family




