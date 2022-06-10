---
title: 'Add and Search Hidden Text in PDF with Aspose.PDF for .NET 11.4.0'
date: Thu, 21 Apr 2016 12:12:15 +0000
draft: false
url: /2016/04/21/add-and-search-hidden-text-in-pdf-use-same-page-object-after-calling-processpragraphs-method-with-aspose.pdf-for-.net-11.4.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Add hidden text to PDF', 'Hide text in PDF programmatically', 'Search hidden text in PDF', 'Set text visibility in PDF programmatically']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="add hidden text in PDF using C#">}}


We are glad to announce the release of [Aspose.PDF for .NET 11.4.0][1] which offers some new features as well as enhancements to previously supported functionalities. The capability to add hidden text in PDF document is one of the major new features introduced in this release. Furthermore, we also have introduced the capability to use PDF file objects after calling ProcessPragraphs() method which is not possible with earlier versions.

## Add and Search Hidden Text in PDF Document using C#

In order to add hidden text, set TextState.Invisible property to 'true' for the added text. TextFragmentAbsorber finds all text that matches the pattern (if specified). Please note that hidden text in the document will be invisible for end-user while viewing the document with PDF reading software (e.g. Acrobat Reader). But it can be found using a text search. There are several ways to make text invisible for end-user in PDF and we have implemented one of those techniques. However, the text added through our approach can be found using TextFragmentAbsorber and we can not guarantee that any hidden text added by third-party applications can be found using the same approach but in case you encounter any issue, please share the resource file and we can further investigate the scenario.

```
//Create document with hidden text
Aspose.Pdf.Document doc = new Aspose.Pdf.Document();
Page page = doc.Pages.Add();
TextFragment frag1 = new TextFragment("This is common text.");
TextFragment frag2 = new TextFragment("This is invisible text.");
//Set text property - invisible
frag2.TextState.Invisible = true;

page.Paragraphs.Add(frag1);
page.Paragraphs.Add(frag2);
doc.Save(myDir + "39400_out.pdf");
doc.Dispose();

//Search text in the document
doc = new Aspose.Pdf.Document(myDir + "39400_out.pdf");
TextFragmentAbsorber absorber = new TextFragmentAbsorber();
absorber.Visit(doc.Pages[1]);

foreach (TextFragment fragment in absorber.TextFragments)
{
    //Do something with fragments
    Console.WriteLine("Text '{0}' on pos {1} invisibility: {2} ", 
        fragment.Text, fragment.Position.ToString(), fragment.TextState.Invisible);
}
doc.Dispose();
```

## Using Page Object after ProcessPragraphs() Call

The ProcessPragraphs() method was introduced to calculate objects placed inside PDF file and in case we need to have page count information during PDF file generation, this method can be used as it manipulates file objects and returns the desired information. In earlier release versions, once this method was called, the file objects could not be accessed any further. So if you need to add any new object to the existing page instance, it was not possible and you had to have a new Page instance where objects can be placed. Nevertheless, starting this new release, you can utilize the same Page objects even after calling the ProcessPragraphs() method.

```
// instantiate Document object
Document document1 = new Document();
// add page to pages collection of PDF file
var page1 = document1.Pages.Add();
// create a loop of 5 to add objects inside PDF file
for (int i = 1; i <= 5; i++)
{
    var table1 = new Aspose.Pdf.Table();
    table1.ColumnWidths = "100";
    table1.IsInNewPage = true;
    Aspose.Pdf.Row row1 = table1.Rows.Add();
    Aspose.Pdf.Text.TextFragment tf = new Aspose.Pdf.Text.TextFragment("part" + i);
    tf.IsInLineParagraph = false;
    tf.IsKeptWithNext = false;
    Aspose.Pdf.Cell cell1 = row1.Cells.Add();
    cell1.Paragraphs.Add(tf);
    page1.Paragraphs.Add(table1);        
}
// Process paragraphs inside PDF file
document1.ProcessParagraphs();
// print number of page count in PDF
Console.WriteLine("# of pages in PDF = " + document1.Pages.Count);
// add text to earlier page instances of PDF file
document1.Pages[1].Paragraphs.Add(new Aspose.Pdf.Text.TextFragment("Post ProcessParagraphs() call text"));
document1.Pages.Add();
// Print page count of PDF file
Console.WriteLine("# of pages in PDF after ProcessParagraphs() call = " + document1.Pages.Count);
// save resultant PDF document
document1.Save(@"C:\pdftest\ProcessParagraphIssue.pdf");
```

## Miscellaneous fixes

As well as the enhancements and features discussed above, there have been specific improvements regarding PDF to PDF/A, Multi-Column PDF, FootNote rendering, generation of large table objects inside PDF, XFA Form to Standard Acro Form conversion, PDF to Image, PDF to HTML, HTML to PDF conversion, Text replacement and rendering PDF files to XPS format conversion. Please download and try the latest release of [Aspose.PDF for .NET 11.4.0][2].




[1]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+11.4.0+Release+Notes
[2]: https://downloads.aspose.com/pdf/net




