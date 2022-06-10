---
title: 'WebResa Uses Aspose.Words for Generating Technical Documents from CMS'
date: Wed, 20 Oct 2010 12:56:39 +0000
draft: false
url: /2010/09/20/generating-technical-documents-from-cms-using-apis/
author: Usman Aziz
summary: ''
tags: ['Aspose.Words', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About WebResa



{{< figure align=center src="images/logo_webresa2.gif" alt="">}}


WebResa is an extranet solution devoted to travel agencies, and especially to tracking agencies. With WebResa, agencies can manage their travels, detailed description, departure dates, and availability. They can also share this information with partners (reselling agencies, tourism offices, and governmental offices).

One of the options proposed by WebResa is to manage detailed information on the travel as day by day program, equipment required, meeting point information, cultural or economic information on the track. All this information can be used to create practical sheets in Word format, which the agency can print and send to the customers.

## Requirements Scenario

The main goal of this project was to create on the fly a structured Word document, easy to print, download and modify, including a list of sections. This document should be printed by the agency or its resellers and should be customized with respect to the design rules.

## Solution

In WebResa we have created a form in order to create and fill the section using an HTML editor or a copy/paste function form a word document. Each section can include formatted text, tables, images, and links.

On the other hand, we have asked the agencies to produce a template Word document, including a specific header and footer with a logo, and custom text style for each section.

In this way, a track can be printed with different aspects, depending on which reseller print the practical sheet.

So the last step of editing the final document is done by [Aspose.Words][1] which loads the right template, and fills every section with the specific formatted text or image.

## Benefits

We previously used MS-Word automation to accomplish that task. But we had maintenance problems because our development environment was not the same as the production environment. Moreover, when we changed our production server, and the operating system, migrating to Windows 2008, it was a nightmare to make the automation working. At the end, we couldn’t succeed.

Also, automation kept several MS-Word processes in memory so we had to be careful in using it.

It was very easy to adapt to the development and use of the [Aspose component][2]. Also, we solved all our environment and memory problems, and we are now sure to have a reliable system.

## Future Implementations

In the future new functionalities are projected so agencies could merge selected practical sheets in a unique document, using various templates, and creating a Word or PDF document. It is also planned to import the XML practical sheet on the fly and produce formatted word documents using Aspose components.

## Conclusion

When I take into consideration the time lost trying to use the automation way, I must say that I should have chosen [Aspose.Words for .NET][3] solution earlier. It would have saved us a lot of time wasted on a nonreliable solution used instead of implementing Aspose.Words for .NET.

Having that first experience in mind, in another project I directly used [Aspose.Cells for .NET][4] and it was very easy to implement and to maintain.



{{< figure align=center src="images/sokar-development-case-study-aspose-words.png" alt="">}}


### Manage the Practical Sheet

From this page, we can import text from a word document, manage each document section and export the final content in Word format as well as in XML.



{{< figure align=center src="images/sokar-development-case-study-aspose-words-1.png" alt="">}}


### Editing Each Section

Modify or creating each section can be done using an HTML editor. Text can be styled, tables or images can be added.



{{< figure align=center src="images/sokar-development-case-study-aspose-words-2.png" alt="" caption="The header of the resulting document using both template and dynamic content.">}}




{{< figure align=center src="images/sokar-development-case-study-aspose-words-3.png" alt="" caption="Inside the document, styled text and table are converted to word format.">}}


**Christophe Liacopoulos  
**SOKHAR




[1]: https://products.aspose.com/words
[2]: https://products.aspose.com/
[3]: https://products.aspose.com/words/net
[4]: https://products.aspose.com/cells/net




