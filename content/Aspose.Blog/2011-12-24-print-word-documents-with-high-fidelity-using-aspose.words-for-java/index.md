---
title: 'Print Word Documents with High Fidelity using Aspose.Words for Java'
date: Sat, 24 Dec 2011 06:58:51 +0000
draft: false
url: /2011/12/24/print-word-documents-with-high-fidelity-using-aspose.words-for-java/
author: Adam Skelton
summary: ''
tags: ['Print MS Word Documents in Java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="Aspose.Words Logo">}}


Printing is a function that has been around in Aspose.Words for .NET for quite a while. We are proud to announce to that starting in Version 10.5, printing is also fully supported in [Aspose.Words for Java][1]. You can easily print all or only specified pages of a document with just a few lines of code.

TheAspose.Words for Java API provides the handy _Document.Print_ method whose overloads allow you to print a document using various different options with just one line of code. You can choose to print using default settings, print to a specific printer by name and even printing options such as page range to print. ([read more][2]

## Pass Any Document Loaded into Aspose.Words to Standard Java Printing Devices

Aspose.Words provides the **AsposeWordsPrintDocument** class which allows any document loaded into Aspose.Words to be printed with the standard Java printing API. This class provides the “typical” one document page per physical page printing.

The **AsposeWordsPrintDocument** class implements the following print interfaces:

*   Pageable
*   Printable

This class can be passed directly to standard Java print classes such as **PrinterJob** using **PrinterJob.setPageable** or **PrinterJob.setPrintable** and allows you to easily print the document with dialogs such as the standard print dialog.

## Previewing a Document before Printing

The standard Java API doesn’t provide any existing functions to print preview any Java on its own. With Aspose.Words, not only do we provide the facilities to print documents, we also provide sample code to preview documents before printing in the **DocumentPreviewAndPrint** sample. The preview provided by the print preview dialog is the same as what is expected when the document it printed to a real printer. Check out the images below for a small demonstration.

**The input document to be printed.**



{{< figure align=center src="images/rendering-preview-1024x576.jpg" alt="Print Preview Word Doc">}}


Additionally, the full source document in DOC format is available for download from this [link][3].

**Next, the print preview of the above document generated using Aspose.Words for Java.**



{{< figure align=center src="images/print-preview-cropped-1024x699.jpg" alt="Print Word Document">}}


**Finally, the physical output printed on a local printer using Aspose.Words for Java. As you can see Aspose.Words prints this document with high fidelity.**



{{< figure align=center src="images/Print-Preview-Output.jpg" alt="MS Word Print Preview Output">}}


## Print Multiple Document Pages onto a Single Sheet of Paper

You can utilize Aspose.Words for Java to fully customise how documents are printed. An example of this is printing multiple document pages onto a physical page by implementing your own print document class. Achieving this using Aspose.Words is a straight forward task. We have already provided the sample code ready for use in the **MultiplePagesOnSheet** sample.

**The output of running this sample code on the same document as previous with settings of four pages on one sheet:**



{{< figure align=center src="images/Multiple-Pages-Output-1-744x1024.jpg" alt="Multiple Pages Output">}}


## Implementing Custom Printing Logic

Finally, it’s worth mentioning you can use the built-in methods in the Aspose.Words API to implement your own printing classes based on your own logic. Without going into too much detail, this is the basis of how the previous sample of printing multiple pages on one sheet is implemented. Using such methods as Document.renderToSize, Document.getPageInfo you can use Aspose.Words to integrate with Java’s printing framework, customize the print process to your liking and custom print documents loaded into Aspose.Words.

You can check out an example of this in action by taking a look at the code for the previous sample. The full code for this sample can be downloaded from here: [Program.java][4]

## Find out More

You can test out all these great features for yourself by downloading the latest version of Aspose.Words for Java from the [Aspose.Words Downloads][5] page.




[1]: https://products.aspose.com/words/java
[2]: https://docs.aspose.com/display/wordsjava/Rendering+and+Printing)
[3]: https://github.com/aspose-words/Aspose.Words-for-Java/
[4]: https://github.com/aspose-words/Aspose.Words-for-Java/
[5]: https://downloads.aspose.com/words/java




