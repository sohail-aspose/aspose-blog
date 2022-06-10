---
title: 'Mail Merge in Word Documents using C# or VB.NET - .NET Mail Merge API'
seoTitle: "C# Mail Merge API | MS Word Mail Merge API for .NET | Aspose.Words"
description: "Learn how to use Mail Merge in MS Word documents using C# or VB.NET with .NET Mail Merge API without MS Word or Office Interop. MS Word Mail Merge Library."
date: Tue, 14 Jul 2020 06:59:00 +0000
draft: false
url: /2020/07/14/mail-merge-in-word-documents-using-csharp-or-vb.net/
author: Usman Aziz
summary: ''
tags: ['.net mail merge API', 'csharp mail merge api', 'mail merge without office', 'ms word mail merge in asp.net', 'ms word mail merge in csharp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words_-150x150-1-e1594387398675.png" alt="Aspose.Words">}}


In this article, I'll show you how to perform **MS Word Mail Merge using C# or VB.NET without MS Word or Office Interop**. [Aspose.Words for .NET][1] is a feature-rich and powerful Word API that provides all the basic as well as extended MS Word Mail Merge features. It lets you generate letters, envelopes, reports, invoices, and other types of documents within Windows Forms, ASP.NET web applications, or any .NET/.NET Core application.

Covering the salient features of our .NET Mail Merge API, this article is composed of the following sections:

*   [What is Mail Merge?][2]
*   [Data Sources for Mail Merge][3]
*   [Preparing Template for Mail Merge][4]
*   [.NET Mail Merge API - Installation][5]
*   [Perform Mail Merge in Word Document using C#][6]
*   [Mail Merge using XML Data Source][7]
*   [Custom Formatting of Merge Fields][8]
*   [Mail Merge with Regions][9]
*   [Nested Mail Merge Regions][10]

## What is Mail Merge? {#What-is-Mail-Merge}

[Mail Merge][11] is the way of automated generation of reports, letters, envelopes, invoices, and other types of documents. Mail Merge in MS Word allows you to create a template document containing merge fields and then populate those fields using records in the data source. To understand Mail Merge, suppose you have to send a letter to ten different people and only name and the address fields are to be updated. In such a case, simply create a template of the letter and then dynamically generate the letters by populating the name and address merge fields using the data source.

## Data Sources for Mail Merge {#Data-Source-for-Mail-Merge}

The data for the Mail Merge could be fetched from any data source such as XML, JSON, or a database. As far as Aspose.Words for .NET is concerned, you can use any data source which is supported by ADO.NET. The data can be loaded into a DataSet, DataTable, DataView, or an array of values.

## Preparing Template for Mail Merge {#Preparing-Template-for-Mail-Merge}

The Mail Merge template is the document that contains the merge fields. These fields are then populated with the data in the data source when the Mail Merge is executed. The template document doesn't need to be a template format and it can be a DOC/DOCX document. This is how you can prepare a template for Mail Merge.

*   Open your document or create a new one in MS Word.
*   Place the cursor where you want to add a merge field.
*   From the **Insert** menu select **Field** option.
*   From the **Field names** list, select **MergeField**.
*   Enter a name for the merge field in **Field name** and press **OK**.
*   Save the document.

The following is the screenshot of the [sample template][12] document.



{{< figure align=center src="images/template.jpg" alt="Mail Merge Template">}}


## .NET Mail Merge API - Installation {#NET-Mail-Merge-API}

Aspose.Words for .NET can be downloaded or installed using the following ways:

*   [Download DLL][13]
*   [Install via NuGet Package Manager][14]

## Perform Mail Merge in Word Document using C# {#Perform-Mail-Merge-in-Word-Document-using-CSharp}

Once you have the template ready, you can execute the Mail Merge to generate the documents. The following are the steps to execute the Mail Merge on the above-mentioned template.

*   Load the template document using [Document][15] class.
*   Set required Mail Merge options such as [Document.MailMerge.TrimWhitespaces][16].
*   Execute a Mail Merge using [Document.MailMerge.Execute()][17] method and pass the data source as the parameter.
*   Save the generated document using [Document.Save(String)][18] method.

The following code sample shows how to execute MS Word Mail Merge using an array of values in C#.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Mail-Merge-ExecuteArray-ExecuteArray.cs" >}}

### Word Document after Mail Merge



{{< figure align=center src="images/Mail-Merge-Word-Document-1.jpg" alt="Execute Mail Merge in C#">}}


## Perform Mail Merge using XML Data Source in C# {#Perform-Mail-Merge-using-XML-Data-Source-in-CSharp}

The XML files are widely used to keep as well as import/export data. Aspose.Words for .NET also support XML as a data source for the Mail Merge. Just read the XML into a [DataSet][19] object and execute the Mail Merge. The following is the sample XML file that we are going to use.

```
<customers>
<customer Name="John Ben Jan" ID="1" Domain="History" City="Boston"/>
<customer Name="Lisa Lane" ID="2" Domain="Chemistry" City="LA"/>
<customer Name="Dagomir Zits" ID="3" Domain="Heraldry" City="Milwaukee"/>
<customer Name="Sara Careira Santy" ID="4" Domain="IT" City="Miami"/>
</customers>
```

The following code sample fetches the data from an XML data source and executes the Mail Merge using C#.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Mail-Merge-XMLMailMerge-XMLMailMerge.cs" >}}

Below is the Mail Merge [template][20] that will be populated with XML data.



{{< figure align=center src="images/template2.jpg" alt="Mail Merge Template for XML">}}


The following is page 1 of the resultant Word document we get after executing the Mail Merge.



{{< figure align=center src="images/Mail-Merge-Word-Document.jpg" alt="Execute Mail Merge with XML in C#">}}


## Custom Formatting of Merge Fields {#Custom-Formatting-of-Merge-Fields}

Aspose.Words for .NET gives you more control over the Mail Merge during the execution. The [MailMerge.FieldMergingCallback][21] property allows you to customize the Mail Merge when any merge field is encountered. MailMerge.FieldMergingCallback accepts the class implementing the [IFieldMergingCallback.FieldMerging][22] and [IFieldMergingCallback.ImageFieldMerging][23] methods.

The following code sample shows how to customize the Mail Merge operation and apply formatting to the cells within [this template][24].

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Mail-Merge-MailMergeAlternatingRows-MailMergeAlternatingRows.cs" >}}

The following is the implementation of the **HandleMergeFieldAlternatingRows** class.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Mail-Merge-MailMergeAlternatingRows-HandleMergeFieldAlternatingRows.cs" >}}

## Mail Merge with Regions using C# {#Mail-Merge-with-Regions}

There might be the case when you need to populate and repeat a particular region in the Word document. For such a case, you can use the Mail Merge with regions. To create a region you need to specify the start and the end of the region and then Mail Megre will repeat that region for each record in the data source. For example, The following template contains two regions, Orders and OrderDetails with the merge fields «TableStart:Orders», «TableEnd:Orders» and «TableStart:OrderDetails», «TableEnd:OrderDetails» respectively.



{{< figure align=center src="images/template_regions.jpg" alt="Mail Merge with Regions">}}


The following is the code sample that performs Mail Megre on regions for the above-mentioned [template][25].

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Mail-Merge-ExecuteWithRegionsDataTable-ExecuteWithRegionsDataTable.cs" >}}

The following are the methods to read data from the database.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Mail-Merge-ExecuteWithRegionsDataTable-ExecuteWithRegionsDataTableMethods.cs" >}}

## Nested Mail Merge Regions {#Nested-Mail-Merge-Regions}

Most often, the data we have in the data source comes in the form of relationships. For example, the table "Order" will have a one-to-many relationship with the "OrderDetails" that will keep records of the items in an order. To deal with such parent-child relationships, nested Mail Merge is used. The following is a sample [invoice template][26] that well-suits this scenario.



{{< figure align=center src="images/template_nested.jpg" alt="Mail Merge Template with Regions">}}


The following is the sample XML data source that we'll use for the nested Mail Merge.

```
<?xml version="1.0" encoding="utf-8"?>
<Orders xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="OrdersSchema.xsd">
  <Order>
    <Number>23</Number>
    <Address>Nelson Street</Address>
    <Suburb>Howick</Suburb>
    <City>Auckland</City>
    <Phonenumber>543 1234</Phonenumber>
    <Date>03/01/2010</Date>
    <Total>14.00</Total>
    <Item>
      <Name>BBQ Chicken Pizza</Name>
      <Price>6.00</Price>
      <Quantity>1</Quantity>
      <ItemTotal>6.00</ItemTotal>
    </Item>
    <Item>
      <Name>1.5 Litre Coke</Name>
      <Price>4.00</Price>
      <Quantity>2</Quantity>
      <ItemTotal>8.00</ItemTotal>
    </Item>
  </Order>
  <Order>
    <Number>10</Number>
    <Address>Parkville Avenue</Address>
    <Suburb>Pakuranga</Suburb>
    <City>Auckland</City>
    <Phonenumber>548 7342</Phonenumber>
    <Date>05/03/2010</Date>
    <Total>6.00</Total>
    <Item>
      <Name>Hawaiian Pizza</Name>
      <Price>4.00</Price>
      <Quantity>1</Quantity>
      <ItemTotal>4.00</ItemTotal>
    </Item>
    <Item>
      <Name>Fries</Name>
      <Price>1.00</Price>
      <Quantity>2</Quantity>
      <ItemTotal>2.00</ItemTotal>
    </Item>
  </Order>
</Orders>
```

Whereas, the **OrderSchema.xsd** for this XML is:

```
<?xml version="1.0" encoding ="utf-8"?>
<xs:schema id="OrdersSchema"  xmlns:xs="http://www.w3.org/2001/XMLSchema">
 <xs:element name="Orders">
 <xs:complexType>
 <xs:sequence>
  <xs:element name="Order">
  <xs:complexType>
  <xs:sequence>
  <xs:element name="Number"/>
  <xs:element name="Address"/>
  <xs:element name="Suburb"/>
  <xs:element name="City"/>
  <xs:element name="Phonenumber">
  <xs:element name="Date"/>
  <xs:element name="Total"/>
  <xs:element name="Item">
   <xs:complexType>
   <xs:sequence>
   <xs:element name="Name"/>
   <xs:element name="Price"/>
   <xs:element name="Quantity"/>
   <xs:element name="ItemTotal"/>
   </xs:sequence>
  </xs:complexType>
  </xs:element>
  </xs:sequence>
  </xs:complexType>
 </xs:element>
 </xs:sequence>
 </xs:complexType>
 </xs:element>
</xs:schema>
```

The following code sample is used to execute the nested Mail Merge using C#.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Mail-Merge-NestedMailMerge-NestedMailMerge.cs" >}}

### Word Document after Mail Merge

Below is the first page of the resultant Word document after executing the Mail Merge.



{{< figure align=center src="images/Nested-Mail-Merge-Word-Document.jpg" alt="Word Document after Mail Merge">}}


## Conclusion

Aspose.Words for .NET is a feature-rich Mail Merge API that provides all the standard as well as extended Mail Merge features for .NET applications. Within a few lines of code, you can create simple or complex reports from various types of data sources seamlessly. You can read more about the .NET Mail Merge API from the [documentation][27]. To learn about Aspose.Words for .NET, get started with the [developer's guides][28], and [GitHub][29] code samples.

## Try Aspose.Words for .NET for Free

You can get a free temporary license to try Aspose.Words for .NET without any limitations. [Get your temporary license now][30].

## See Also

*   [Generate Word Documents from Templates in C# .NET][31]




[1]: https://products.aspose.com/words/net
[2]: #What-is-Mail-Merge
[3]: #Data-Source-for-Mail-Merge
[4]: #Preparing-Template-for-Mail-Merge
[5]: #NET-Mail-Merge-API
[6]: #Perform-Mail-Merge-in-Word-Document-using-CSharp
[7]: #Perform-Mail-Merge-using-XML-Data-Source-in-CSharp
[8]: #Custom-Formatting-of-Merge-Fields
[9]: #Mail-Merge-with-Regions
[10]: #Nested-Mail-Merge-Regions
[11]: https://en.wikipedia.org/wiki/Mail_merge
[12]: https://github.com/aspose-words
[13]: https://downloads.aspose.com/words
[14]: http://nuget.org/packages/Aspose.Words
[15]: https://apireference.aspose.com/words/net/aspose.words/document
[16]: https://apireference.aspose.com/words/net/aspose.words.mailmerging/mailmerge/properties/index
[17]: https://apireference.aspose.com/words/net/aspose.words/document/properties/mailmerge
[18]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/2
[19]: https://docs.microsoft.com/en-us/dotnet/api/system.data.dataset
[20]: https://github.com/aspose-words/Aspose.Words-for-.NET/tree/master/Examples/Data
[21]: https://apireference.aspose.com/words/net/aspose.words.mailmerging/mailmerge/properties/fieldmergingcallback
[22]: https://apireference.aspose.com/words/net/aspose.words.mailmerging/ifieldmergingcallback/methods/fieldmerging
[23]: https://apireference.aspose.com/words/net/aspose.words.mailmerging/ifieldmergingcallback/methods/imagefieldmerging
[24]: https://github.com/aspose-words/Aspose.Words-for-.NET/tree/master/Examples/Data
[25]: https://github.com/aspose-words/Aspose.Words-for-.NET/tree/master/Examples/Data
[26]: https://github.com/aspose-words/Aspose.Words-for-.NET/tree/master/Examples/Data
[27]: https://docs.aspose.com/display/wordsnet/Mail+Merge+and+Reporting
[28]: https://docs.aspose.com/display/wordsnet/Developer+Guide
[29]: https://github.com/aspose-words/Aspose.Words-for-.NET
[30]: https://purchase.aspose.com/temporary-license
[31]: https://blog.aspose.com/2020/03/05/generate-word-documents-from-templates-in-csharp-net/





