---
title: 'Generac Implemented MS Word Mail Merge, XSL to PDF, PDF concatenation, Manipulation and Printing  within e-commerce portal'
date: Wed, 17 Feb 2010 16:51:00 +0000
draft: false
url: /2010/02/17/manipulate-print-and-convert-documents-to-pdf-within-e-commerce-portal/
author: Eric Hemmer
summary: ''
tags: ['.NET API for Mail Merge feature in MS Word document', '.NET API to Concatenate PDF files', 'Aspose.Total', 'Combine PDF documents using Aspose.PDF for .NET', 'Concatenate PDF files using Aspose.PDF for .NET', 'Incorporate custom data into XSL and render output in PDF format', 'Mail Merge in MS Word files', 'Merge PDF files into single document', 'PDF files printing using Aspose.PDF for .NET', 'Print PDF documents using Aspose.PDF for .NET', 'Success Stories', 'XSL to PDF conversion']
categories: ['Aspose.Total Product Family']
---

## About Generac



{{< figure align=center src="images/generac-logo.png" alt="Generac logo">}}


[Generac Power Systems][1] provides a private e-commerce portal for its industrial product dealers. Portal functionality includes quotations and ordering, project management features, documentation libraries, and more. Much of the site is dynamically driven based on integrations to the ERP and other systems.

Generac previously used a combination of custom, open-source and commercial 3rd party components to provide document interaction capabilities to the end-user. However, these components were limited in features and presented numerous performance and maintenance issues on the web servers.

## Requirements Scenario

Generac needed to provide users with the ability to:

*   Produce printable, non-editable copies of Quotations, Order Acknowledgements, and Invoices based on data stored in a SQL Server database.
*   Produce editable copies of Customer Proposal documents, including custom logo images and content templates configurable by each user. These documents needed to be made available in different formats, selectable by the dealer.
*   Provide the option for users to download a single concatenated PDF file consisting of several manuals, installation drawings, etc. for a specified product. The single file option is provided for easier downloading and printing since the number of PDF files can be cumbersome.

## Solution Implementation

The first requirement was fairly straight-forward since Generac was already using [XML data to create PDF][2] copies of Quotations, Acknowledgements, Invoices, etc. The data is extracted from a database and transformed using XSL templates into a schema interpreted by a custom parser. The parser then utilizes an open-source product to create the PDF.

After using [Aspose.PDF for .NET][3], the parser and open-source products were eliminated by simply modifying the existing XSL templates to output a schema compatible with the [Aspose.PDF for .NET][4] DOM. Converting the existing XSL templates only required a few hours to complete.

The second requirement was slightly more complex, as the process of generating customized Customer Proposals involved more steps. This process also relied on the use of XML data and the same open-source product, with the output limited to Rich Text Format (RTF) only.

By using [Aspose.Words for .NET][5], the XML transformation and open-source products were eliminated from the process and the DocumentBuilder object was used to enhance the capabilities previously available by allowing insertion of formatted HTML markup provided by the user. The basic layout of the proposal was still handled using a Word document template and merge fields. The customized proposal text was merged into the template using the DocumentBuilder.InsertHTML method. [Aspose.Words for .NET][6] also allowed the user to choose the format of the resultant document.

The third requirement was new functionality. The portal did not previously allow users to combine multiple documents into a single PDF for easier downloading and printing. Each document (_sometimes as many as 20-30_) needed to be individually downloaded and printed, which was a time-consuming process. Bundling the individual files into a single “zip” archive could have made it easier to download, but still required each one to be opened and printed separately.

Using [Apsose.PDF for .NET][7], a button was provided to the user that enabled the option of [combining the individual PDF files into a single document][8], which can be downloaded as well as printed in a single step. This saved a considerable amount of time for the users and has proven to be a very popular enhancement to the site.

## Benefits

The [Aspose.Total for .NET][9] suite provided Generac with the ability to enable end-users to use the portal in a way that works with the products they have installed on their own systems, rather than limiting them to a specific format and version. The products also allowed considerable enhancements to the applications that did not exist before due to technical limitations.

Not needing to rely on document automation saved Generac considerable cost and provided a more stable environment.

Working with familiar technology and programming language allowed Generac developers to be more productive, as opposed to projects that rely on undocumented open-source products.

## Future Implementations

The portal is large and complex, offering many opportunities for future uses of the [Aspose][10] suite of products. A few of the enhancements under consideration include:

*   Using Aspose.Flash for .NET or [Aspose.Slides for .NET][11] to present sales and/or marketing PowerPoint presentations in the Portal site.
*   Using [Aspose.Cells for .NET][12] for budgeting/forecasting data imports and exports.
*   Using [Aspose.Words for .NET][13] to [add advanced mail merge][14] capabilities so Dealers can generate campaign and promotion letters to end customers.

## Conclusion

Generac selected [Aspose.Total for .NET][15] based on the flexibility of document formats and ease of use. The extensive features of the product suite provided considerable time-savings for not only the development team but also the end-users of their web site and in-house applications.

## Screenshots

For editable documents, users are provided the option of selecting the format of the generated document:



{{< figure align=center src="images/Generac-Power-Systems-aspose-total-case-study.png" alt="Option to select output format" caption="Image 1:- Option to select the output format">}}


Some product quotations included several individual files, intended to be printed and delivered as part of the submittal package. The user had the option of [combining all of the PDF files into a single document][16] for easier downloading and [PDF printing][17]:



{{< figure align=center src="images/Generac-Power-Systems-aspose-total-case-study-1.png" alt="Option to concatenate PDF files" caption="Image 2:- Option to combine PDF documents">}}


Users got the ability to specify custom default content for predetermined proposal sections, which was then merged into a document for downloading in the format of their choosing:



{{< figure align=center src="images/Generac-Power-Systems-aspose-total-case-study-2.png" alt="">}}




{{< figure align=center src="images/Generac-Power-Systems-aspose-total-case-study-3.png" alt="Option to specify a custom default content" caption="Image 3:- Option to specify a custom default content">}}




{{< figure align=center src="images/Generac-Power-Systems-aspose-total-case-study-4.png" alt="Preview of resultant MS Word document" caption="Image 4:- Resultant MS Word document">}}




[1]: https://www.generac.com/
[2]: https://docs.aspose.com/display/pdfnet/Working+with+XML
[3]: https://products.aspose.com/pdf/net
[4]: https://products.aspose.com/pdf/net
[5]: https://products.aspose.com/words/net
[6]: https://products.aspose.com/words/net
[7]: https://products.aspose.com/pdf/net
[8]: https://docs.aspose.com/
[9]: https://products.aspose.com/total/net
[10]: https://www.aspose.com/
[11]: https://products.aspose.com/slides/net
[12]: https://products.aspose.com/cells/net
[13]: https://products.aspose.com/words/net
[14]: https://docs.aspose.com/display/wordsnet/Mail+Merge+and+Reporting
[15]: https://products.aspose.com/total/net
[16]: https://docs.aspose.com/
[17]: https://docs.aspose.com/display/pdfnet/Working+with+PDF+printing+-+Facades




