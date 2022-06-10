---
title: 'PDF to PDF/A-2A Conversion, Set Output File Dimensions, Create Link to Already Attached Files with Aspose.Pdf for .NET 9.7.0'
date: Wed, 22 Oct 2014 10:51:01 +0000
draft: false
url: /2014/10/22/pdf-to-pdfa-2a-conversion-set-resultant-file-dimensions-create-link-to-already-attached-files-with-aspose.pdf-for-.net-9.7.0/
author: Codewarior
summary: ''
tags: ['convert pdf to pdfa', 'create links in pdf .net', 'create pdf document in .net', 'pdf manipulation library', 'pdf to pdf2a', 'pdf to pdfa conversion']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


We are very much excited to announce the release of [Aspose.PDF for .NET 9.7.0][1] which has brought many useful features including converting PDF to PDF/A-2A, creating internal links to PDF attachments, enhanced text formatting and many more. Every new release is more powerful, reliable and performance optimized compared to previous versions. To benefit the latest features, we always encourage our customers to migrate to the latest release.

## PDF to PDF/A-2A Conversion

Aspose.PDF for .NET has been supporting conversion from PDF to PDF/A compliant documents and also offers the capability to validate a PDF file's PDF/A compliance. In this release, we have added support for the conversion of PDF to PDF/A\_2A format. Therefore a new value **PDF\_A\_2A** is added to **PdfFormat** enumeration. Please try using the following code snippet to accomplish this requirement.

```
// Load PDF file
Document doc = new Aspose.Pdf.Document("input.pdf");
// Set PDF/A compliance as PDF/A_1a
doc.Convert(new MemoryStream(), PdfFormat.PDF_A_2A, ConvertErrorAction.Delete);
// Save updated document
doc.Save("compliant.pdf");
```

## Create Internal Link to Already Attached Files

Aspose.Pdf for .NET supports the feature to add/update attachments inside PDF documents. It also offers the feature to create link annotations inside PDF files. The link can point to a page within the document, any other file placed on the system, a JavaScript link or some web location. However, the latest release also enables developers to create links to attachments already in the PDF file. For further information, please visit Add Hyperlink to Open Attachments in PDF.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Links-Actions-CreateDocumentLink-CreateDocumentLink.cs" >}}

## PDF to HTML - Set Output File Size (Dimensions)

HTML to PDF and PDF to HTML conversion are some of the main features that the development team is working to improve and in recent releases, we have made significant improvements to them. In the current release, we offer the new capability to set the output file dimensions when converting a PDF file to HTML format. The PdfPageEditor class present in the Aspose.Pdf.Facades namespace provides the feature to update/manipulate pages of PDF document. It also offers the feature to set/update page dimensions of input PDF file. In order to accomplish our requirement, we can first load the source PDF document into PdfPageEditor object, update page dimensions and then render the output in HTML format using HtmlSaveOptions class. For further details, please visit [PDF to HTML - Set Output File Size.][2]

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-DocumentConversion-PDFToHTMLFormat-SetOutputFileDimensions-SetOutputFileDimensions.cs" >}}

## Add SVG Object to Table Cell

Aspose.Pdf for .NET supports the feature to add table cell inside PDF file. While creating table inside PDF file, we can add text or images inside table cells. Furthermore, this API also offers the feature to [convert SVG files to PDF format][3]. So with a blend of both features, we can accomplish the requirement of loading SVG image and add it inside table cells. For further details, please visit [Add SVG Object to Table Cell][4].

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Tables-AddSVGObject-AddSVGObject.cs" >}}

## Set TextFragment Formatting as Underline

A PDF file consists of elements such as Text, Images, Attachments, Annotations, Hyperlinks, Tables etc. When adding Text string to PDF file, we may have a requirement to set formatting for text instance. The latest release of Aspose.Pdf for .NET 9.7.0 offers the feature to set Underline formatting for TextFragment when adding to PDF file. Please try setting **TextState.Underline** property as **true** to accomplish this requirement.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Text-AddText-AddUnderlineText.cs" >}}

## Add Choice Option in Combobox Field

In case you need to add choice option to combo-box field in XFA form, then you need to update the XML template of the document so that the choice is added.

```
Document doc = new Document("37348.pdf");
string[] fields = doc.Form.XFA.FieldNames;
XmlNode node = doc.Form.XFA.GetFieldTemplate(fields[0]);
XmlNode items = node.SelectSingleNode("tpl:items", doc.Form.XFA.NamespaceManager);
XmlNode item = items.OwnerDocument.CreateNode(XmlNodeType.Element, "text", items.NamespaceURI);
item.InnerText = "Choice # 4 ( New )";
items.AppendChild(item);
doc.Save("37348-out.pdf");
```

Among the above stated new features/enhancements, there are numerous other features introduced in this release. We have also made fixes for issues reported in earlier releases. Please get a chance to download and try using the latest release of [Aspose.PDF for .NET 9.7.0][5]




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Convert+PDF+File+into+HTML+Format#ConvertPDFFileintoHTMLFormat-PDFtoHTML-SetOutputFileDimensions
[3]: https://docs.aspose.com/display/pdfnet/Convert+a+File+to+PDF+Format#ConvertaFiletoPDFFormat-ConvertSVGFiletoPDFFormat
[4]: https://docs.aspose.com/display/pdfnet/Add+and+Extract+a+Table#AddandExtractaTable-AddSVGObjecttoTableCell
[5]: https://downloads.aspose.com/pdf/net




