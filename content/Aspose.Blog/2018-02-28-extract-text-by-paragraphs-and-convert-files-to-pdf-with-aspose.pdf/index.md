---
title: 'Extract Text by Paragraphs and Convert Files to PDF with Aspose.PDF'
date: Wed, 28 Feb 2018 21:47:36 +0000
draft: false
url: /2018/02/28/extract-text-by-paragraphs-and-convert-files-to-pdf-with-aspose.pdf/
author: Asad Ali
summary: ''
tags: ['Aspose.Pdf', 'Extract Paragraphs from PDF', 'Extract Text from PDF', 'Extract Text from Paragraph in PDF', 'Extract paragraph in PDF .NET', 'Extract paragraph in PDF Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="">}}


We at Aspose are very excited announcing new version of Aspose.PDF API. Aspose.PDF has been released for .NET and Java platforms with new 18.1 version. In this version of the API, we have offered exciting features including extracting paragraphs from PDF documents. Furthermore, we have improved usability and performance of the API. You can download Aspose.PDF API for .NET and Java platforms, from the links below:

*   [Aspose.PDF for .NET 18.1][1]
*   [Aspose.PDF for Java 18.1][2]

Before downloading latest version of the API, we strongly recommend you to have a look at release notes page(s) in API documentation. We have listed all features and enhancements along with public API changes in respective release notes. Please check following links for release notes page(s):

*   [Release Notes of Aspose.PDF for .NET 18.1][3]
*   [Release Notes of Aspose.PDF for Java 18.1][4]

## Extract Text from PDF by Paragraphs

With previous version(s) of the API, you were able to extract text from PDF documents by searching particular text (using “plain text” or “regular expressions”) from a single page or whole document. However, we have implemented a functionality to extract text from PDF document in paragraphs. We have implemented new function for searching sections and paragraphs in the text of PDF document pages. Following code snippet(s) illustrate **ParagraphAbsorber** usage:

**\[C#.NET\]**

```
private static void TextSample()
{
    Document doc = new Document(myDir + "amblatt2013-10-05.pdf");
    ParagraphAbsorber absorber = new ParagraphAbsorber();
    absorber.Visit(doc);
    foreach (PageMarkup markup in absorber.PageMarkups)
    {
        int i = 1;
        foreach (MarkupSection section in markup.Sections)
        {
            int j = 1;
            foreach (MarkupParagraph paragraph in section.Paragraphs)
            {
                StringBuilder paragraphText = new StringBuilder();
                foreach (List<TextFragment> line in paragraph.Lines)
                {
                    foreach (TextFragment fragment in line)
                    {
                        paragraphText.Append(fragment.Text);
                    }
                    paragraphText.Append("\r\n");
                }
                paragraphText.Append("\r\n");
                Console.WriteLine("Paragraph {0} of section {1} on page {2}:", 
                j, i, markup.Number);
                Console.WriteLine(paragraphText.ToString());
                j++;
            }
            i++;
        }
    }
}
```

**\[Java\]**

```
String myDir = "E:/LocalTesting/";
Document doc = new Document(myDir + "amblatt2013-10-05.pdf");
ParagraphAbsorber absorber = new ParagraphAbsorber();
absorber.visit(doc);
for ( PageMarkup markup : absorber.getPageMarkups())
{
 int i = 1;
 for (MarkupSection section : markup.getSections())
 {
  int j = 1;
  for (MarkupParagraph paragraph : section.getParagraphs())
  {
   StringBuilder paragraphText = new StringBuilder();
       for(List<TextFragment> line : paragraph.getLines())
  {
   for(TextFragment fragment : line)
   {
    paragraphText.append(fragment.getText());
   }
    paragraphText.append("\r\n");
  }
  paragraphText.append("\r\n");
  System.out.println("Paragraph {"+j+"} of section {"+i+"} on page {"+markup.getNumber()+"}:");
  System.out.println(paragraphText.toString());
  j++;
 }
 i++;
 }
}
```

## Inter-File Format Conversion

Since inter-file format conversion has been the most interesting feature offered by Aspose APIs, we have added new feature to convert Postscript/EPS into PDF. You can use following code snippet, in order to perform conversion using Aspose.PDF for .NET/Java API:

```
Document doc = new Document("input.ps", new PsLoadOptions());
doc.Save("output.pdf");
```

## Aspose.PDF for .NET and Java Resources

**The following resources will help you work with Aspose.PDF for .NET and Java:**

*   [Home page for Aspose.PDF API][5].
*   Aspose.PDF for [.NET][6] and [Java][7] wiki docs – Help documentation and API reference documents.
*   [Aspose.PDF product family forum ][8]– Post your technical questions, queries and any other problem you faced while running Aspose.PDF APIs.
*   [Enable Email Subscription ][9]– Do not limit yourself, stay up-to-date with the latest news about the Aspose.PDF APIs and new features, fixes, plus other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples ][10]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.PDF for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Release Notes ([.NET][12] and [Java][13] – For details on API fixes, please check Release Notes having a complete list of the new features.




[1]: https://www.nuget.org/packages/Aspose.Pdf/18.1.0
[2]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-pdf/18.1/
[3]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+18.1+Release+Notes
[4]: https://docs.aspose.com/display/pdfjava/Aspose.PDF+for+Java+18.1+Release+Notes
[5]: http://products.aspose.com/pdf
[6]: https://docs.aspose.com/display/pdfnet/Home
[7]: https://docs.aspose.com/display/pdfjava/Home
[8]: https://forum.aspose.com/c/pdf
[9]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[10]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET
[11]: https://github.com/aspose-pdf/Aspose.Pdf-for-java
[12]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+18.1+Release+Notes
[13]: https://docs.aspose.com/display/pdfjava/Aspose.PDF+for+Java+18.1+Release+Notes)




