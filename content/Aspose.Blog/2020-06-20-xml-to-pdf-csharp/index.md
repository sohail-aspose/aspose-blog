---
title: 'Convert XML to PDF - Easy XML to PDF Conversion'
seoTitle: "XML to PDF | Convert XML to PDF | XML to PDF using C#"
description: "Convert XML to PDF file when input follows XSD schema of the API. Include HTML in XML file. Convert XML and XSLT to PDF in C#."
date: Sat, 20 Jun 2020 21:56:16 +0000
draft: false
url: /2020/06/20/xml-to-pdf-csharp/
author: Farhan Raza
summary: ''
tags: ['XML to PDF', 'convert xml to pdf', 'xml and xslt', 'xml xslt', 'xslt to pdf']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/XML-to-PDF.png" alt="XML to PDF">}}


In this article, we will be converting XML files to PDF using C#. [Aspose.PDF for .NET][1] API extensively supports the XML conversion feature because of the inclusions of many related enhancements, as requested by the API users. You can elevate your .NET applications with this efficient feature of exporting XML to PDF. Let us consider following use cases related to XML conversion using C#:

*   [Convert XML to PDF][2]
*   [Use HTML in XML and Convert to PDF][3]
*   [Convert XML and XSLT to PDF][4]

## Convert XML to PDF {#section1}

For converting an XML to PDF, you need to follow the XML Schema of Aspose.PDF for .NET API which is available as [XSD file][5]. Following is an XML file that we will be converting to PDF as a Hello World demonstration.

```
<?xml version="1.0" encoding="utf-8" ?>
<Document xmlns="Aspose.Pdf">
  <Page id="mainPage">
    <TextFragment>
      <TextSegment>Hello</TextSegment>
    </TextFragment>
 
    <TextFragment>
      <TextSegment>World!</TextSegment>
    </TextFragment>
  </Page>
</Document>
```

You need to follow the steps below to convert XML to PDF file:

1.  Initialize an object of [Document][6] Class
2.  Load XML file with [BindXml][7] method
3.  Save the converted PDF file

Following code snippet shows how to convert XML to PDF in C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "XMLtoPDF.cs" >}}

## Use HTML in XML and Convert to PDF {#section2}

Sometimes you might need to use HTML in XML prior conversion to HTML. Aspose.PDF for .NET API supports this feature as well. However, HTML and XML tags are quite similar. Therefore, you need to specify the CDATA tag so that the HTML is not parsed as XML markup. Below sample XML file includes HTML denoted by CDATA to avoid any anomaly:

```
<?xml version="1.0" encoding="utf-8" ?>
<Document xmlns="Aspose.Pdf">
  <Page id="mainSection">
    <HtmlFragment>
      <![CDATA[
        <font style="font-family:Tahoma; font-size:40px;">This is Html String.</font>
        ]]>
    </HtmlFragment>
  </Page>
</Document>
```

You can convert this XML file to PDF with following steps:

1.  Instantiate [Document][8] class object
2.  Load the input XML file
3.  Save the output PDF file

Below code snippet shows how to convert an XML file, containing HTML, to PDF in C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "XMLtoPDF.cs" >}}

## Convert XML and XSLT to PDF {#section3}

Sometimes you may have an existing XML file that contains important application data and you want to generate PDF reports using that XML file. In such scenarios, you can create XSLT file to transform your existing XML document to Aspose.PDF’s compatible XML document. Then you can proceed to convert XML to PDF. Let us learn this with simple and basic example:

```
<?xml version="1.0" encoding="utf-8" ?>
<Contents>
  <Content>Hello World!</Content>
</Contents>
```
```
<?xml version="1.0" encoding="utf-8" ?>
<xsl:stylesheet version="1.0" xmlns:xsl="http://www.w3.org/1999/XSL/Transform">
    <xsl:template match="text()"/>
    <xsl:template match="/Contents">
    <html>
      <Document xmlns="Aspose.Pdf" IsAutoHyphenated="false">
        <PageInfo>
          <DefaultTextState
                            Font = "Helvetica" FontSize="8" LineSpacing="4"/>
          <Margin Left="5cm" Right="5cm" Top="3cm" Bottom="15cm" />
        </PageInfo>
        <Page id="mainSection">
          <TextFragment>
            <TextSegment>
              <xsl:value-of select="Content"/>
            </TextSegment>
          </TextFragment>
        </Page>
      </Document>
    </html>
</xsl:template>
</xsl:stylesheet>
```

You can notice that the XML file does not follow the XML schema of Aspose.PDF for .NET API. However, the XSLT file transforms it to required compatibility. Now you can follow the steps below to convert such XML using XSLT to PDF:

1.  Initialize PDF [Document][9]
2.  [Bind][10] XML and XSLT file
3.  Save the output PDF document

The code snippet below is based on these steps which show how to convert XML to PDF in C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "XMLxsltToPDF.cs" >}}

## Conclusion

We have learned how to convert XML to PDF file provided the XML follows the mentioned schema of the API. Considering the popularity and usability of HTML tags, we have also considered the scenario when you need to include some HTML in the source XML file. Moreover, we have also explored how to convert XML and XSLT to PDF when the existing XML file does not follow the schema.

## See Also

[Merge Multiple PDF Files into One PDF using C# .NET][11]




[1]: https://products.aspose.com/pdf/net
[2]: #section1
[3]: #section2
[4]: #section3
[5]: https://github.com/aspose-pdf/Aspose.PDF-for-.NET/blob/master/Artifacts/Aspose.Pdf.xsd
[6]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[7]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/methods/bindxml/index
[8]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/methods/bindxml/index
[11]: https://blog.aspose.com/2020/01/16/merge-multiple-pdf-files-in-csharp-net/





