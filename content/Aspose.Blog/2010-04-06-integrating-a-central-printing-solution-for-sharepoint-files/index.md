---
title: 'iMUSH Integrated a central printing solution for SharePoint repository using Aspose APIs'
date: Tue, 06 Apr 2010 11:39:00 +0000
draft: false
url: /2010/04/06/integrating-a-central-printing-solution-for-sharepoint-files/
author: Shai Petel
summary: ''
tags: ['Aspose.Total', 'Concatenate PDF files using Aspose.PDF for .NET', 'Integrate .NET APIs to SharePoint solution', 'Manipulate and Print MS Word files using Aspose.Words for .NET', 'Manipulate and print Excel files using Aspose.Cells for .NET', 'Print PDF document using Aspose.PDF for .NET', 'Print PowerPoint presentations using Aspose.Slides for .NET', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About KWizCom



{{< figure align=center src="images/kwizlogo.png" alt="KWizCom logo">}}


[KWizCom][1] goal is to provide nothing less than outstanding products and exceptional customer service!  
Entrust KWizCom to help you achieve your business goals and put you on the fast track to productivity. We created a product iMUSH which is a bundle of products for SharePoint that enable users to perform tasks on a bunch of items at once. iMUSH includes the following solutions for SharePoint: Scan, Print, Files, and Reports

iMUSH-Print will enable users to collect several documents and web forms from SharePoint and combine them into one printable file, allowing them to save it for later or send it to the printer.

## Requirements Scenario

iMUSH-Print allows users to collect several documents from different formats and merge them into one file. For that, we need a strong, reliable, and fast server-side conversion tool that can convert documents in-memory from one format to another, and merge them into one large PDF/XPS file for a print-preview.

Since we have been working on the server-side, as we wish to support any client OS/Browser combination and as SharePoint-files are not stored in the file system but in a database, it was important for us to use in-memory conversion without the need to work with the local file system.

As an ISV, our target audiences are simple-click install solutions that do not require any server-side components or many configurations, and our product won't be used by many IT specialists. Furthermore, we shall also support any type of server configuration/platform that our customers may have.

The scenarios we support in iMUSH-Print are:

*   To any document library or subfolder, add a print menu with the following options:
    *   Print all documents in this folder, or print selected documents
        *   [Print the documents alone][2]
        *   Print the document's properties
        *   Print both the documents and their properties
    *   Print all documents properties in a table
*   To any list or subfolder in a list, add a print menu with the following options:
    *   Print all items in this folder, or print selected items
        *   Print the item's properties
        *   Print the item's attachments
        *   Print both the item's properties with their attachments
    *   Print all items properties in a table
*   To any list item, add a print menu with the following options:
    *   Print the item properties
    *   Print the item attachments
    *   Print both the item properties with their attachments
*   To any document, add a print menu with the following options:
    *   Print the documents alone
    *   Print the document's properties
    *   Print both the documents and their properties

**Note**: Documents and attachments may be of any type, including images, PDF, office documents, HTML, InfoPath, and more.

Once the user has selected the content he wishes to print, he should then see a print preview file that he then could send to his printer.

## Solution Implementation

We have implemented a feature for SharePoint that registers print menu items into the document library, list, and view item forms.

Once installed, it allows for any site collection owner to activate the iMUSH-Print feature which will add these menu items and allow all users to start working with the product.

Using [Aspose.Total for .NET][3], we were able to have our ASP.NET application resides in SharePoint and [convert documents from various formats into PDF in memory][4], without the need for access to the server’s file system and with no IO overhead.

Aspose was one of the only solutions that supported even our most advanced configuration scenarios while having no server configuration requirements at all, and not requiring Office on the server while providing excellent results in Office document conversions.

## Benefits

Before [Aspose][5], we implemented a solution that relied on Office 2007 to be installed on the server and had to connect to its COM objects for the conversion.

The problems were massive, such as:

*   Configuring COM+ access for any application pool user
*   Office limitations on performance and lack of threading support
*   Extremely slow and heavy conversion process
*   Lots of IO work with the file system, having to save temp files before and after conversion
*   And more

By using [Aspose][6], we were able to eliminate any configuration problems we had with the other solution and, now we do not require our customers to install office on the server!

Not only that, by using [Aspose.Total for .NET][7], we increased our performance by more than 100% and reduced our file-system IO to nothing.

## Future Implementations

Aspose platform supports much more than what we bargain for.

As a leading ISV, KWizCom is always releasing innovative solutions for SharePoint.

Our experience in the past with other leading providers such as Telerik showed us that by leveraging the best platforms for development – we will always be a step ahead of our competition, as it opens the door for many new products.

Our next step will be to implement Export to PDF to many of our existing products such as Calendar Plus and List Aggregator. Many customers requested this feature so far.

## Conclusion

Although our products are in early beta stages, by using [Aspose.Total for .NET][8], we were able to deliver a high-quality solution while saving valuable development time.

Integration with Aspose was lightning fast. In less than a couple of hours, we had all our test cases converted to Aspose and they worked even better than before!

The ROI on [Aspose.Total for .NET][9] will be swift and certain.

## **Screenshots**



{{< figure align=center src="images/iMUSH-aspose-total-case-study.png" alt="iMUSH bundle installation" caption="Image 1:- iMUSH bundle installation">}}




{{< figure align=center src="images/iMUSH-aspose-total-case-study-1.png" alt="Document library print menu" caption="Image 2:- Document library print menu">}}




{{< figure align=center src="images/iMUSH-aspose-total-case-study-2.png" alt="Document library print settings popup" caption="Image 3:- Document library print settings popup">}}




{{< figure align=center src="images/iMUSH-aspose-total-case-study-3.png" alt="Get the PDF ready for print" caption="Image 4:- Get the PDF ready for print">}}




{{< figure align=center src="images/iMUSH-aspose-total-case-study-4.png" alt="Document context menu print" caption="Image 5:- Document context menu print">}}




{{< figure align=center src="images/iMUSH-aspose-total-case-study-5.png" alt="Document properties toolbar print" caption="Image 6:- Document properties toolbar print">}}




{{< figure align=center src="images/iMUSH-aspose-total-case-study-6.png" alt="List toolbar print menu" caption="Image 7:- List toolbar print menu">}}




{{< figure align=center src="images/iMUSH-aspose-total-case-study-7.png" alt="List item toolbar print menu" caption="Image 8:- List item toolbar print menu">}}




{{< figure align=center src="images/iMUSH-aspose-total-case-study-8.png" alt="List item toolbar print menu popup" caption="Image 9:- List item toolbar print menu popup">}}




{{< figure align=center src="images/kwiz-case-study-aspose-total-1024x354.png" alt="KWizCom iMUSH SharePoint Features preview" caption="Image 10:- KWizCom iMUSH SharePoint Features, including files, print, and scan">}}


**Shai Petel  
**VP R&D, KWizCom Corp




[1]: https://kwizcom.com/
[2]: https://docs.aspose.com/display/pdfnet/Working+with+PDF+printing+-+Facades
[3]: https://products.aspose.com/total/net
[4]: https://docs.aspose.com/display/wordsnet/Convert+a+Document+to+PDF
[5]: https://www.aspose.com/
[6]: https://www.aspose.com/
[7]: https://products.aspose.com/total/net
[8]: https://products.aspose.com/total/net
[9]: https://products.aspose.com/total/net




