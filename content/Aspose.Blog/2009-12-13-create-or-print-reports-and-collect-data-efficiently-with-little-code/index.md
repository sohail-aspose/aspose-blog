---
title: 'G Squared Consulting Implemented Mail Merge, Created, Printed reports and Collected Data Efficiently in a Student Tracking system'
date: Sun, 13 Dec 2009 18:20:00 +0000
draft: false
url: /2009/12/13/create-or-print-reports-and-collect-data-efficiently-with-little-code/
author: Danny Odonnell
summary: ''
tags: ['.NET API for DOC DOCX files manipulation', '.NET API for MS Excel files processing', 'Aspose.Cells', 'Aspose.PDF', 'Aspose.Total', 'Aspose.Words', 'Dynamic Excel worksheet creation', 'Dynamic MS Word document creation', 'MS Word document processing API', 'Populate fields on Word document with database content', 'Programatically manage Mail Merge fields in MS Word documents', 'Programatically process Pivot Tables in Excel worksheet', 'Render InfoPath forms to MS Word format', 'Success Stories', 'Word to PDF conversion using Aspose.Words for .NET', 'update mail merge fields in word document']
categories: ['Aspose.Words Product Family', 'Aspose.Total Product Family', 'Aspose.PDF Product Family', 'Aspose.Cells Product Family']
---

## About G Squared Consulting



{{< figure align=center src="images/GsquaredLLCLogoGreenBLACKoriginal-38l6uj5krpz3l46kymeeps.gif" alt="">}}


[G Squared Consulting][1] is an IT consulting company. Our client, a local school district vocational center, was seeking to streamline their business process and web presence. A new state mandate required a new way of tracking students, and with this came a need to retool many of their system processes, fundamentally changing the way they do business with their students. One of the aims was to reduce the amount of staff interaction with a student’s records before enrollment and allowing the prospective student to provide their information to the school in a form-specific manner. Given the district’s financial limitations, we needed to use a component-driven solution, with as little custom coding done as possible. Requirements included PDF and Word output, with the ability to do [Excel pivot table based data manipulation][2].

## Requirements Scenario

We had a need to give a school the ability to collect and store student demographics, financial aid, and grading information, provide teachers with on-demand student reports, and provide administrators the ability to track both overall program progress both academically and financially. We also needed to collect information from dynamic forms. Aspose.Forms in conjunction with InfoPath seemed like our best option, as we could design the forms easily using InfoPath, and host them in aspx pages with the Forms component.

Once this information was collected, we wanted to give the teachers the ability to print out forms, in both .doc and .pdf format. Once the principle approved the form, we wanted to have this info formatted precisely. This could be accomplished quickly and easily with **[Aspose.Words for .NET][3]** and [**Aspose.PDF for .NET**][4]. Finally, a number of grade and enrollment progression reports would be needed using [Excel pivot tables][5]. Here, **[Aspose.Cells for .NET][6]** was a natural and good fit.

## Solution Implementation

We used Visual Studio 2008, with [Aspose Products][7] for document generation and a third-party component suite for the presentation layer, on top of a DotNetNuke portal. We collected student entered information using InfoPath form generation, backed up with an Aspose XmlFormView component in a simple .NET user control converted to a DNN module. It took us longer to create the form using InfoPath than it took to write the code consuming it with the XmlFormView. Countless hours were saved on this step alone.

Many of the forms collected by the school have been approved by the School Board and are not easily changed, such as report cards. When a printed record of this information is needed, it must be in the original form. Using [mail merge fields in Aspose.Words for .NET][8], we were able to take the original Word documents, populate them with the data from the InfoPath form or student database, and generate both Word and PDF versions easily.

## Benefits

In a tightly cost-driven environment, the [Aspose products][9] gave our company a tremendous boost. Being able to use the existing forms was key, and having on-demand student based reports outputted in Excel, Word, or PDF with little coding really saved the day. We have created many dynamic Word and Excel documents using hand-created templates, WordML, and RTF generation, and wish that we had discovered Aspose many years earlier. The benefit of using an [Aspose.Words for .NET][10] template probably saved hundreds of hours messing around with WordML formatting and outputting alone. The ability to output these as PDF was critical, and again [Aspose][11] could not be beaten.

## Future Implementations

We intend to implement more student reporting using [Aspose.Cells for .NET][12] and [Aspose.PDF for .NET][13], and to extend the number of camera-ready documents generated using [Aspose.Words for .NET][14]. Our company will also be looking to bid (_and win!_) other government contracts using the cost savings projected by using this suite.

## Conclusion

In a highly cost-sensitive environment, we were able to create reports and collect data quickly, efficiently, and with very little code. The [Aspose suite of products][15] will now be a large part of our consulting business and will give us a leg up on our bigger competitors.

Screenshot of the Aspose.Form document progression:

1\. Original Word Document



{{< figure align=center src="images/Our-client-a-local-school-district.png" alt="Preview of document progression" caption="Image 1:- Preview of Word document">}}


2\. Converted to InfoPath document, and reformatted



{{< figure align=center src="images/Our-client-a-local-school-district-1.png" alt="Preview of Inforpath converted and reformatted document" caption="Image 2:- Document converted to InfoPath">}}


3\. Shown in ASP.NET page, using AsposeWeb:XmlFormView component.



{{< figure align=center src="images/Our-client-a-local-school-district-2.png" alt="Preview of form in Web page" caption="Image 3:- Preview of form on a web page">}}


At this point, we traversed the XmlDataNode of the XmlFormView and inserted the input data into the DB. This entire process was completed in a matter of hours.

Thank you, Aspose!




[1]: http://www.gsquaredllc.com/
[2]: https://docs.aspose.com/display/cellsnet/Pivot+Tables
[3]: https://products.aspose.com/words/net
[4]: https://products.aspose.com/pdf/net
[5]: https://docs.aspose.com/display/cellsnet/Pivot+Tables
[6]: https://products.aspose.com/cells/net
[7]: https://products.aspose.com/
[8]: https://docs.aspose.com/display/wordsnet/Mail+Merge+and+Reporting
[9]: https://products.aspose.com/
[10]: https://products.aspose.com/words/net
[11]: https://www.aspose.com/
[12]: https://products.aspose.com/cells/net
[13]: https://products.aspose.com/pdf/net
[14]: https://products.aspose.com/words/net
[15]: https://products.aspose.com/




