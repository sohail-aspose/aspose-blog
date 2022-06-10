---
title: 'Improved PDF to HTML and PDF to PDF/A Conversion with Aspose.PDF for .NET 11.5.0'
date: Thu, 05 May 2016 19:49:51 +0000
draft: false
url: /2016/05/05/csharp-pdf-to-html-and-pdf-to-pdfa-conversion-aspose.pdf-for-.net/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


A new release of [Aspose.PDF for .NET 11.5.0][1] has been published and in terms of features and stability, its an improved and better version as compared to earlier versions. We have always strived to implement the possible new features and enhancements requested by our customers so that they can create amazing applications. Our API's have uncompromising capabilities for document manipulation/generation and these startling features put incredible power that leaps past most API's in the market. It makes even complex work as easy as two lines of code can perform interfile format conversion. The key to our API's experience is its simple and workable approach, which helps in creating incredible applications with fewer lines of code.

## Get Warning against Font Substitution

One of the customers recently had a requirement to show a warning when fonts are substituted. This is a useful feature in tests, as it allows to fail the tests faster if the font is missing, rather than having to track down why the result looks incorrect. In order to cater to this requirement, the following members are added in Document class to get notifications about font substitutions:

*   public delegate void FontSubstitutionHandler(Aspose.Pdf.Text.Font oldFont, Aspose.Pdf.Text.Font newFont);
*   public event FontSubstitutionHandler FontSubstitution;

In order to get notifications for font substitutions, please try using following code snippet:

```
void OnFontSubstitution(Aspose.Pdf.Text.Font oldFont, Aspose.Pdf.Text.Font newFont)
{
   Console.WriteLine(string.Format("Font '{0}' was substituted with another font '{1}'",
               oldFont.FontName, newFont.FontName));
}

//...
Document doc = new Document("sample.pdf");
doc.FontSubstitution += new Document.FontSubstitutionHandler(OnFontSubstitution);
```

## Retrieve Form Fields in Tab order

When we iterate through form fields, the fields are returned in the order in which they were created. However recently we had a requirement to retrieve them in the tab order, if the tab order has been set manually in the PDF file. In order to accomplish this requirement, two properties are added in our API.

1.  Field.TabOrder is tab order of the field.

This property allows to set or get tab order of the field on the page.

```
foreach (Field field in pdf1.Form.Fields)
{
   Console.WriteLine(field.PartialName + " " + field.TabOrder);
}
```

1.  Page.FieldsInTabOrder

Returns list of fields in tab order.

```
foreach (Field field in doc1.Pages[1].FieldsInTabOrder)
{
       Console.WriteLine(field.PartialName);
}
```

## Miscellaneous Fixes

As well as the enhancements and features discussed above, there have been specific improvements regarding PDF to PDF/A, PDF to HTML, XPS to PDF, HTML to PDF, FootNote rendering, Text manipulation and Image placement/manipulation in PDF document. Please download and try the latest release of [Aspose.PDF for .NET 11.5.0][2].




[1]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+11.5.0+Release+Notes
[2]: http://www.aspose.com/downloads/pdf-family/net/new-releases/aspose.pdf-for-.net-11.5.0/




