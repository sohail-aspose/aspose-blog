---
title: 'Nikosh Bangla Unicode Converter facilitated the conversion of hundreds of documents within no time using Aspose APIs'
date: Fri, 17 Jul 2009 12:12:51 +0000
draft: false
url: /2009/07/17/convert-hundreds-of-documents-nikosh-bangla-unicode-converter/
author: Mohammad Ashraful Anam
summary: ''
tags: ['Aspose.Total', 'DOC DOCX conversion to PDF Image TIFF XPS formats', 'Excel files creation and manipulation using Aspose.Cells for Java', 'MS Word document processing using Aspose.Words for Java', 'PowerPoint presentation processing using Aspose.Slides for Java', 'Render PowerPoint slides to Image PDF format', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About Bangladesh Election Commission



{{< figure align=center src="images/Screenshot-2020-05-14-at-10.50.05-PM.png" alt="Bangladesh Election Commission">}}


Bangla is the default language used on the [Bangladesh Election Commission website][1] and Until Unicode arrived, many languages like Bangla did not have any standard implementation. Unicode solved the coding scheme for us and standardized most languages. But most countries like Bangladesh and India have already hundreds of products that let users write their native languages. How was this achieved?

These languages were coded in normal ASCII characters and a keyboard interface written to translate each character to its Latin equivalent. Many fonts were developed as well. While these hack and slash schemes worked and were able to show and print Bangla correctly, each company had its own coding implementation. So each product was incompatible with another. A word document written with Product A and Font A1 would show gibberish when used with Product B and Font B1. This went one for more than 10 years. Unicode solved this problem, but what happens to the hundreds of documents written in non-standard ASCII encoding now that Unicode is here? We need to convert those documents to standard Unicode. Hence, “Nikosh Bangla Converter”.

## Requirements Scenario

It is quite easy to write a generic converter that will convert ASCII coded Bangla text to its Unicode equivalent. A simple text file containing hundreds of pages can be converted in less than a minute. The problem arises when we try to convert different MS Office documents. The MS Office Automation of PIA implementation was just too slow and it many cases it breaks the formatting.

We tested the two leading currently available Bangla converters. The test document was a 32 page Bangla document containing text, image, table and header and footer. One of the converters took 4.5 minutes to convert and the other 56 minutes! Even at 4.5 minutes, it was too long. If a document takes 5 minutes on average to convert a single document, it would take just too much time to convert hundreds of documents. We needed something that would reduce this time to less than a minute and at the same time, preserve all the styles. Also, the converter for only MS Word was available; there were absolutely no converters to convert MS Excel or PowerPoint documents.

## Solution Implementation

I started looking for all the available solutions. At first, I coded using Word Interop and as previously mentioned it was just too slow. I started looking for other available technologies. I found [Aspose][2] and Tx Text Converter. Both looked good.

I gave Aspose a try because it looked easier and also it had Word, Excel, and PowerPoint support which the other lacked. Then working over the weekend up to 3AM, I was finally ready with my first C# prototype converter (_I found a supplied C# sample that provided me a good start_). I tested it initially against a single page document and, it produced good results. Finally, I tested it against the complex 32 pages documents that I had tested with the other two products with and the results were very impressive. Not only did it convert very fast but also very accurately and without breaking any kind of formatting. After perfecting the MS Word conversion technique, we finally made a converter for MS Excel and PowerPoint also.

## Benefits

The chart below shows the performance comparison of our “Nikosh” implementation and the other converters available on the market. The speed increase is just amazing.



{{< figure align=center src="images/native-languages-aspose-total-case-study-1024x477.png" alt="Conversion performance chart" caption="Image 1:- Document conversion performance chart">}}


After creating and distributing the converter for free for several months, we have finally come to a point where everyone is asking for a converter that will run in Linux. The best part is that [Aspose][3] has almost the same product lineup for Java and we have been able to reproduce our program for Linux using [Aspose Total for Java][4].

## Future Implementations

Now that we are able to convert all MS Office legacy documents, we would try to squeeze even more performance out of [Aspose products][5] and make our converter even faster.

## Conclusion

I was really amazed that I was able to produce a fully working product in less than two days of work. And the speed at which I was able to perform all MS Office document operation was just amazing! You just can’t go wrong with this product!!!



{{< figure align=center src="images/native-languages-aspose-total-case-study-1.png" alt="Splash Screen" caption="Image 1:- Splash Screen">}}




{{< figure align=center src="images/native-languages-aspose-total-case-study-2.png" alt="Batch Conversion Screen (.NET version)" caption="Image 2:- Batch Conversion Screen (.NET version)">}}




{{< figure align=center src="images/native-languages-aspose-total-case-study-3.png" alt="MS Word document conversion screen " caption="Image 3:- MS Word document conversion screen (Java version)">}}





[1]: http://ecs.gov.bd/
[2]: https://www.aspose.com/
[3]: https://www.aspose.com/
[4]: https://products.aspose.com/total/java
[5]: https://products.aspose.com/




