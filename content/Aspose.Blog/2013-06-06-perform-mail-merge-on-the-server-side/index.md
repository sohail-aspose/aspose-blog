---
title: 'Bison Process CRM Performs Server Side Mail merge, MS Word and Excel files processing using APIs'
date: Thu, 06 Jun 2013 19:33:48 +0000
draft: false
url: /2013/06/06/perform-mail-merge-on-the-server-side/
author: Diego Kuenzi
summary: ''
tags: ['Aspose.Total', 'Java API for Excel files processing', 'Java API for MS Word files processing', 'Mail Merge in MS Word files using Java API', 'Manipulate Excel files using Aspose.Cells for Java', 'Send emails using Aspose.Email for Java', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About Bison



{{< figure align=center src="images/Screenshot-2020-05-06-at-4.49.51-AM.png" alt="Bison Company logo">}}


[Bison][1] is a provider of business IT solutions. With 30 years of market experience, we have unique expertise in assisting customers with their IT needs on a long-term basis.

We develop the business software Bison Process which focuses on flexible company processes and offers an industry model with specific processes for the industry sectors agriculture, wholesale, production, retail, steel, and trading.

Bison is one of Switzerland's leading IT companies, with a total of five branches in Switzerland and Germany. The headquarters is in Sursee (near Lucerne). The company employs over 350 people.

## Problem

All of our customers use Microsoft Office on a daily basis. Bison Process contains a fully integrated CRM module assisting employees in planning and monitoring sales projects, sales and purchasing teams, forecasts, and related activities. Our customers are used to work with Microsoft Word and would like to merge the master data that is stored in the Bison Process CRM module. Bison Process is integrated with a printing environment and our customers desire to print a mail merged result using this existing environment.

It is important for us to enable our customers to create mail merge templates by using the current Microsoft Word file formats (DOC, DOCX). We needed a solution that allows mail merge to be performed on the server-side. That way, we would be able to store the resultant file directly in the backend system or execute a mail merge in a background job without any user attendance. We also need to convert the resulting file to different file formats (e.g. PDF).

## Solution

To solve the problem, we considered developing a solution on our own without using a third-party product. However, we realized it is not our core business. We also feared that the undertaking might get too expensive and take too long. Hence we started evaluating a number of open-source [Java libraries][2]. Unfortunately, none of these libraries met our requirements: these libraries either didn't include a mail merge or only supported limited Microsoft Word formats.

When we encountered [Aspose.Words for Java][3], we were surprised by the simple API for [performing a mail merge][4]: only one method. With the sample project downloaded from the Aspose website, we were able to try a simple mail merge within 30 minutes - it just worked.

To achieve a mail merge using the master data stored in the Bison Process CRM, we added a new mail merge workflow to the existing customer list business object: this workflow gets executed on the server-side and collects the customer data to be merged and performs a mapping to the standard Microsoft Word merge field names.

The user first needs to create their own Microsoft Word template and store it within Bison Process as a mail merge template. To invoke the mail merge function, the user invokes a simple mail merge workflow on a given customer list. The result of the mail merge is automatically attached to the customer list and may be opened or printed.



{{< figure align=center src="images/Bison-is-a-provider-of-business-IT-solutions-1024x405.png" alt="Preview of Mail merge operation" caption="Image 1:- Flow diagram for the mail merge operation">}}


## Experience

We were looking for a solution that not only supports Microsoft Word file formats but also file formats of the other Microsoft Office Suite tools like Microsoft Excel and Microsoft Outlook. We were delighted to find [Aspose.Total for Java][5] is a comprehensive compilation of libraries. By choosing [Aspose.Total for Java][6], we are now able to implement further important office integration features into Bison Process which will strengthen the product’s market position.

We evaluated a [free trial][7] and were able to quickly create a proof of concept. We didn't need any [support][8] - the provided examples and the [documentation][9] is extensive and the API is self-explanatory. It took us only two days to implement the new mail merge workflow and provided the means to store mail merge templates. The core part of the implementation that uses [Aspose.Words for Java][10] API took us a mere two hours. When the developer presented the implementation in a code review, the attending colleagues were impressed upon the simple and embeddable API provided by the [Aspose libraries][11].

Bison Process is based on Java technology and the server-side runs on Microsoft or Linux operating systems. It was crucial for us to use a pure Java third-party library that does not depend on native libraries, and also does not depend on Microsoft Office libraries. [Aspose.Words for Java][12] is a pure Java library and met this important criterion.

We are very pleased with the outcome of the implementation. We were able to implement a [mail merge][13] feature in a short time. By purchasing [Aspose.Total for Java][14], we believe we have made a sustainable investment. Bison Process, our flagship product, could be improved by adding an Office integration feature, which helps our customers to work more efficiently with Bison Process.

## Next Steps

We are looking forward to using more of the [Aspose.Total for Java][15] functionality in the near future.

We plan to generate Excel documents using [Aspose.Cells for Java][16] on arbitrary data out of the Bison Process. This feature will enable customers to use Microsoft Excel to edit large data sets in an efficient manner.

We also plan to use [Aspose.Email for Java][17] to parse incoming mail messages in the MSG file format in order to automatically attach the message to the associated business object in Bison Process (e.g. Lead, Service Order). Another improvement will be the possibility to automatically [send mail messages][18] out of the Bison Process containing rich content and attachments.

These features will help our customers to complete their daily business more efficiently and will improve the market position of the Bison Process.

## Summary

We are satisfied with all the aspects when integrating a third-party library into a product: An easy-to-understand but comprehensive API, a pure Java library, extensive [documentation][19], and self-explanatory examples. We also would like to mention the pleasant cooperation with the representatives of [Aspose][20] regarding the negotiation of the [OEM license][21].

With [Aspose.Total for Java][22] we have now a good reference for what a third-party API should look like. This helps us when we need to evaluate other third-party libraries for special features that we want to integrate into the Bison Process. We recommend [Aspose.Total for Java][23] to other companies having similar challenges as we do.




[1]: https://www.bison-group.com/
[2]: https://products.aspose.com/total/java
[3]: https://products.aspose.com/words/java
[4]: https://docs.aspose.com/display/wordsjava/Mail+Merge+and+Reporting
[5]: https://products.aspose.com/total/java
[6]: https://products.aspose.com/total/java
[7]: https://downloads.aspose.com/total/java
[8]: https://forum.aspose.com/
[9]: https://docs.aspose.com/display/totaljava/Home
[10]: https://products.aspose.com/words/java
[11]: https://products.aspose.com/
[12]: https://products.aspose.com/words/java
[13]: https://docs.aspose.com/display/wordsjava/Mail+Merge+and+Reporting
[14]: https://products.aspose.com/total/java
[15]: https://products.aspose.com/total/java
[16]: https://products.aspose.com/cells/java
[17]: https://products.aspose.com/email/java
[18]: https://docs.aspose.com/display/emailjava/Developer+Guide
[19]: https://docs.aspose.com/display/totaljava/Home
[20]: https://www.aspose.com/
[21]: https://purchase.aspose.com/pricing/total/java
[22]: https://products.aspose.com/total/java
[23]: https://products.aspose.com/total/java




