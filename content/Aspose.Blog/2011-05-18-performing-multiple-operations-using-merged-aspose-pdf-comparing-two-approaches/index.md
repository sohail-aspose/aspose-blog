---
title: 'Performing Multiple Operations using Merged Aspose.PDF: Comparing Two Approaches'
date: Wed, 18 May 2011 19:43:29 +0000
draft: false
url: /2011/05/18/performing-multiple-operations-using-merged-aspose-pdf-comparing-two-approaches/
author: Shahzad Latif
summary: ''
tags: ['Shahzad Latif']
---

I have already discussed, in my previous post, the three parts of the merged [Aspose.PDF][1] API. If you haven't read this post yet then you may read it now: Introduction to the Merged Aspose.PDF API. In this post, I'm going to show you the code snippets from Aspose.Pdf.Facades and Aspose.Pdf DOM API.

These code snippets will help you understand the process to edit existing PDF files using both of these approaches. I'll explain the process of performing multiple operations and compare the code as well. For the sake of simplicity, I'm going to keep the examples short, considering only two operations: add text and add header. Later on, we'll get into more complex scenarios, but for this post, let's stick with two operations.

## Code is like Painting!

Well, if you're a programmer, you definitely know that code is like painting; the only difference is that you can't hang it on the wall. :) The more options and flexibility we have to engage our creative faculties, the better! New merged Aspose.Pdf provides the same. You can use Aspose.Pdf.Facades to edit existing PDF files either for the sake of backward compatibility or to implement some functionality quickly; Or, you can use Aspose.Pdf DOM API to perform multiple operations in one go and to gain access to the individual elements of the PDF document.

## Adding Text and Header using Aspose.Pdf.Facades

In the following code snippet, you can see that in order to add text and header you need to use two different classes -- PdfFileMend and PdfFileStamp. Each class opens and saves the PDF file separately. This approach provides the advantage of writing less code and achieving your goal using only two methods -- AddText and AddHeader; however, it adds a little overhead when you open and close the same file multiple times.

> //create formatted text to add in the main body and the header  
> FormattedText formattedText = new FormattedText("Aspose - Your File Format Experts!",  
> System.Drawing.Color.AliceBlue,  
> System.Drawing.Color.Gray,  
> Aspose.Pdf.Facades.FontStyle.Courier,  
> EncodingType.Winansi,  
> true,  
> 14  
> );
> 
> //create PdfFileMend object to add text  
> PdfFileMend mender = new PdfFileMend("input.pdf", "output1.pdf");  
> //add text in the PDF file  
> mender.AddText(formattedText, 1, 100, 200, 400, 400);  
> //close PdfFileMend object  
> mender.Close();
> 
> //open document to add header  
> PdfFileStamp fileStamp = new PdfFileStamp("output1.pdf", "finaloutput.pdf");  
> //add header  
> fileStamp.AddHeader(formattedText, 10);  
> //save updated PDF file  
> fileStamp.Close();

## Adding Text and Header using New DOM API

Aspose.Pdf DOM API, on the other hand, opens and closes the PDF file only once and performs multiple operations. You create a Document object to open and close the PDF file. The Document class provides all the methods, properties and collections to work with various elements of the PDF file. Once all the operations are performed, the output PDF is finally saved with all the changes.

> //open document  
> Document pdfDocument = new Document("input.pdf");  
> //get particular page  
> Page pdfPage = (Page)pdfDocument.Pages\[1\];
> 
> //create text fragment  
> TextFragment textFragment = new TextFragment("Aspose - Your File Format Experts!");  
> textFragment.Position = new Position(100, 600);
> 
> //set text properties  
> textFragment.TextState.FontSize = 12;  
> textFragment.TextState.Font = FontRepository.FindFont("Courier");  
> textFragment.TextState.BackgroundColor = System.Drawing.Color.Gray;  
> textFragment.TextState.ForegroundColor = System.Drawing.Color.AliceBlue;
> 
> // create TextBuilder object  
> TextBuilder textBuilder = new TextBuilder(pdfPage);
> 
> // append the text fragment to the PDF page  
> textBuilder.AppendText(textFragment);
> 
> //create header  
> TextStamp textStamp = new TextStamp("Aspose - Your File Format Experts!");  
> //set properties of the header  
> textStamp.TopMargin = 10;  
> textStamp.HorizontalAlignment = HorizontalAlignment.Center;  
> textStamp.VerticalAlignment = VerticalAlignment.Top;  
> //add header on all pages  
> foreach (Page page in pdfDocument.Pages)  
> {  
> page.AddStamp(textStamp);  
> }
> 
> //save document  
> pdfDocument.Save("output.pdf");

## You Want to See this Code Running? At Your System!

Well, although a public release is not in the pipeline right away, if you're interested, I can try to make special arrangements to grab a latest copy from our development team! You can get back to me via [Aspose.Pdf.Kit forum][2]. If you have any comments, questions, or suggestions then please do let us know.




[1]: https://products.aspose.com/pdf
[2]: http://forum.aspose.com



