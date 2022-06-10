---
title: 'The Karis group implemented SalesForce document management with mail merge and print features using APIs'
date: Fri, 03 May 2013 06:12:47 +0000
draft: false
url: /2013/05/03/salesforce-document-management-with-mail-merge-and-print-features-using-apis/
author: David Mclain
summary: ''
tags: ['.NET API to manipulate MS Word files', 'Aspose.Words', 'Convert DOC/DOCX to PDF format', 'Insert dynamically generated data into MS Word files', 'Mail Merge for MS Word files', 'Print MS Word files using .NET Api', 'Programatically process MS Word files', 'Render MS Word files to PDF format', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About The Karis group



{{< figure align=center src="images/Screenshot-2020-04-26-at-6.02.14-AM.png" alt="">}}


[The Karis group][1] provides patient advocacy services to individuals who have exhausted their medical benefits and are now receiving care on a self-pay basis. Our team mediates directly between patients and providers, allowing patients to focus on their health while we focus on solutions for their bills.

Our negotiations generate large numbers of documents and to streamline our processes, we built a custom SalesForce.com solution that generates custom merge templates from our data and sends those documents out via a number of routes including faxing and e-signature.

## Requirements Scenario

In the original incarnation of the solution, a server-side copy of Microsoft Word was scripted through COM automation to open a file, merge data and then, either print or save the document. COM automation is not thread-safe when multiple teams members access the application at the same time, so the chances are that Word would freeze and the web application would be in an unrecoverable state until a full server reboots.

Our requirements for the new solution were:

*   All server-side side code needs to be multi-user safe
*   Use native Word document formats
*   Replicate [Mail Merge functionality][2]
*   [Ability to print][3] to a network printer

We also had a couple nice to have requirements including:

*   [Output to PDF][4]
*   [Ability to insert items into the document][5] dynamically

## Solution Implementation

Before we found [Aspose][6], we spent a fair amount of time struggling with RTF documents as a possible alternative to using Word documents. After that effort became bogged down, we took another look at [Aspose][7] and took advantage of the [free trial][8]. Within hours, we had the library integrated and [documents being produced][9] and [printed][10] without issue.

During [Aspose.Words for .NET][11] integration, we made extensive use of the [mail merge features][12] as well as the [print system][13]. The [online documentation][14] made the entire process very simple and our code ended up substantially easier to maintain and understand, compared to the COM automation solution we had in place before.

## Benefits

The old system was less stable but after the integration of [Aspose.Words for .NET][15], we haven't had any downtime and our documents looked similar as they appeared in Microsoft Word. Our system became more maintainable than it was before and we became less concerned about our ability to handle new documents as they were created.

## Conclusion

If we had not found [Aspose.Words for .NET][16], our solution could not have become as robust and easy to maintain as it is now. We were hesitant at first due to price, but we already have covered it up with increased productivity on the development side and decreased downtime for our users. Any developers, who are interested to programmatically work with Word documents we strongly recommend them to first try using [Aspose.Words for .NET][17].

## Screenshots



{{< figure align=center src="images/karis-group-aspose-words-case-study.png" alt="Dialog to Print, Preview, Download file" caption="Image 1:- Screen to select the document for Print, Preview, Download or Fax">}}


The user can select to merge a template from a bill and then chooses from a number of pre-built documents and can choose to immediately send that to a printer, view it in HTML, download it for local editing, fax it via RightFax or email it via EchoSign.



{{< figure align=center src="images/karis-group-aspose-words-case-study-1.png" alt="Resultant Word document preview" caption="Image 2:- Resultant MS Word document preview">}}


The completed document has all the relevant data from our SalesForce.com database in it and is ready for immediate release to a provider or patient.




[1]: https://www.thekarisgroup.com/
[2]: https://docs.aspose.com/display/wordsnet/Mail+Merge+and+Reporting
[3]: https://docs.aspose.com/display/wordsnet/Print+a+Document+Programmatically+or+Using+Dialogs
[4]: https://docs.aspose.com/display/wordsnet/Converting+a+Word+document+to+PDF
[5]: https://docs.aspose.com/display/wordsnet/Working+with+Document
[6]: https://www.aspose.com/
[7]: https://www.aspose.com/
[8]: https://downloads.aspose.com/words/net
[9]: https://docs.aspose.com/display/wordsnet/Programming+with+Documents
[10]: https://docs.aspose.com/display/wordsnet/Print+a+Document+Programmatically+or+Using+Dialogs
[11]: https://products.aspose.com/words/net
[12]: https://docs.aspose.com/display/wordsnet/Mail+Merge+and+Reporting
[13]: https://docs.aspose.com/display/wordsnet/Print+a+Document+Programmatically+or+Using+Dialogs
[14]: https://docs.aspose.com/display/wordsnet/Developer+Guide
[15]: https://products.aspose.com/words/net
[16]: https://products.aspose.com/words/net
[17]: https://products.aspose.com/words/net




