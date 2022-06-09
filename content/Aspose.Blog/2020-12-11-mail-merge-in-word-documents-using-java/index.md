---
title: 'Mail Merge in MS Word Documents using Java'
seoTitle: ""
description: ""
date: Fri, 11 Dec 2020 18:05:06 +0000
draft: false
url: /2020/12/11/mail-merge-in-word-documents-using-java/
author: Usman Aziz
summary: 'This post covers **how to perform Mail Merge operations in MS Word documents using Java**. By the end of this article, you will learn how to create Mail Merge templates and execute Mail Merge programmatically.'
tags: ['complete MS Word mail merge tutorial', 'create mail merge template in java', 'mail merge in word in java']
categories: ['Aspose.Words Product Family']
---

This post covers **how to perform Mail Merge operations in MS Word documents using Java**. By the end of this article, you will learn how to create Mail Merge templates and execute Mail Merge programmatically.

*   [About Mail Merge][1]
*   [Java Mail Merge API][2]
*   [Data Sources for Mail Merge][3]
*   [Create a Mail Merge Template in MS Word][4]
*   [Create a Mail Merge Template using Java][5]
*   [Perform Mail Merge in Word Document using Java][6]
*   [Mail Merge using XML Data Source][7]
*   [Perform Mail Merge with Regions][8]
*   [Create Nested Mail Merge Regions][9]
*   [Custom Formatting of Merge Fields][10]

## About Mail Merge {#About-Mail-Merge}

[Mail Merge][11] is a convenient way of generating letters, envelopes, invoices, reports, and other types of documents dynamically. Using Mail Merge, you create a template file containing the merge fields and then populate those fields using the data in a data source. Let's suppose you have to send a letter to 20 different people and you only need to change the name and the address of the receivers on each copy. In this case, you can create a Mail Merge template for the letter and then generate 20 letters by populating the name and address fields dynamically.

## Java Mail Merge API - Free Download {#Java-Mail-Merge-API}

[Aspose.Words for Java][12] is a well-known word processing API that lets you create various types of documents from scratch. The API provides built-in Mail Merge features that allow you to dynamically generate documents using templates and data sources. Aspose.Words for Java can be downloaded as [JAR][13] or installed within the Maven-based applications.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-words</artifactId>
    <version>20.11</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Data Sources for Mail Merge {#Data-Sources-for-Mail-Merge}

The data in the Mail Merge could be fetched from any data source such as JSON, XML, spreadsheet, or a database.

## Create Template for Mail Merge in MS Word {#Prepare-Mail-Merge-Template}

The template being used in Mail Merge can be a simple Word document (i.e [DOCX][14] and it doesn't need to be in a template format. The template document contains the merge fields that are populated with data when Mail Merge is executed. The following are the steps of how to prepare a Mail Merge template using MS Word.

*   Create a new document in MS Word.
*   Place the cursor where you want to add a merge field.
*   From the **Insert** menu select the **Field** option.
*   From the **Field names** list, select **MergeField**.
*   Enter a name for the merge field in the **Field name** and press **OK**.
*   Save the document as DOCX.

The following is the screenshot of the [sample template][15] document.



{{< figure align=center src="images/template.jpg" alt="mail merge word template">}}


## Create Mail Merge Template using Java {#Create-Mail-Merge-Template-using-Java}

You can also generate the Mail Merge template programmatically. The following are the steps for it.

*   Create an instance of [DocumentBuilder][16] class.
*   Insert merge fields using methods provided by _DocumentBuilder_ such as [insertTextInput][17], [insertField][18], [InsertParagraph][19], and etc.
*   Save the document using [DocumentBuilder.getDocument().save(String fileName)][20] method.

The following code sample shows how to create a Mail Merge template using Java.

{{< gist aspose-com-gists ef6c4280ab216d12222a5c252b936892 "create-template.java" >}}

## Perform Mail Merge in Word Document using Java {#Perform-Mail-Merge-in-Word-Document-using-Java}

Once the template is ready, you can populate the merge fields with data. The following are the steps of performing Mail Merge on a Word template.

*   Create a new template using [Document][21] class (or load the existing template).
*   Create an instance of [DocumentBuilder][22] class and pass the _Document_ object to its constructor.
*   Execute a Mail Merge using [Document.getMailMerge().execute()][23] method and pass the data source as the parameter.
*   Save the generated Word document using [DocumentBuilder.getDocument().save(String)][24] method.

The following code sample shows how to perform mail merge in Word documents using Java.

{{< gist aspose-com-gists ef6c4280ab216d12222a5c252b936892 "mail-merge.java" >}}

### Template



{{< figure align=center src="images/execute_simple_mail_merge_1-1.png" alt="simple mail merge in java">}}


### Output



{{< figure align=center src="images/execute_simple_mail_merge_2.png" alt="simple mail merge">}}


## Perform Mail Merge using XML Data Source {#Mail-Merge-using-XML-Data-Source}

In the previous example, we performed Mail Merge using the Java objects. However, in most of the cases, a data source is used to populate the merge fields. For demonstration, let's check out how to use an XML data source in Mail Merge. The following are the steps for it.

*   Load the XML data source using the _DataSet_ class.
*   Load the Mail Merge template using [Document][25] class.
*   Use the _execute_ function to populate the merge fields using the desired data table in the data source.
*   Save the generated Word document using [Document.save(String)][26] method.

The following is the XML data source being used in this example.

{{< gist aspose-com-gists ef6c4280ab216d12222a5c252b936892 "datasource.xml" >}}

The following code sample shows how to populate the Mail Merge template using the Customer data table in the provided XML data source.

{{< gist aspose-com-gists ef6c4280ab216d12222a5c252b936892 "mail-merge-xml.java" >}}

### Template



{{< figure align=center src="images/fill_merge_template_from_xml.png" alt="mail merge with XML">}}


### Output



{{< figure align=center src="images/fill_merge_template_from_xml_2-368x1024.png" alt="mail merge xml">}}


## Mail Merge with Regions in Java {#Mail-Merge-with-Regions}

In certain cases, you may need to repeat a particular region in the document. For example, you want to display orders placed by each customer in a separate table. In such cases, you can take advantage of the Mail Merge regions. In order to create a region, you can specify the start and the end of the region. As a result, the region will be repeated for each instance of the data during the Mail Merge execution.

The following screenshot shows a template in which the region consists of a table. It starts with _«TableStart:Customers»_ and ends at _«TableEnd:Customers»_.



{{< figure align=center src="images/execute_mail_merge_with_regions_1-1024x192.png" alt="mail merge region template">}}


The following code sample shows how to create a template with regions and populate it with the data.

{{< gist aspose-com-gists ef6c4280ab216d12222a5c252b936892 "mail-merge-region.java" >}}

### Output



{{< figure align=center src="images/execute_mail_merge_with_regions_2-1024x318.png" alt="mail merge region">}}


## Create Nested Mail Merge Regions using Java {#Nested-Mail-Merge-Regions}

Another popular scenario in Mail Merge is when you have nested regions. For example, when you have to list the orders and the items in each order then you can use the nested regions. The following image makes the picture more clear about the nested regions.



{{< figure align=center src="images/nested_mail_merge_with_regions_2-1024x340.png" alt="">}}


In the image above, we have the _Orders_ table and the _Items_ table where each record in _Items_ is linked to a record in _Orders_. Hence, there exists a one-to-many relationship between these two tables. In such cases, Aspose.Words executes the Mail Merge taking care of the relationships defined in the DataSet. For instance, if we have an XML data source then Aspose.Words will either use the schema information or the structure of XML to find out the relationships. Thus, you will not have to handle it manually by yourself and the _Document.getMailMerge().executeWithRegions(DataSet)_ method will work for you (as the previous example).

## Apply Custom Formatting on Merge Fields {#Custom-Formatting-of-Merge-Fields}

In order to give you more control over the Mail Merge, Aspose.Words for Java allows you to customize the merge fields during the Mail Merge execution. The [setFieldMergingCallback(IFieldMergingCallback)][27] method accepts a class which implements [fieldMerging(FieldMergingArgs)][28] and [imageFieldMerging(ImageFieldMergingArgs)][29] methods for custom control over the Mail Merge process. The _fieldMerging(FieldMergingArgs)_ event occurs when a merge field is encountered during the Mail Merge execution.

The following is the complete code sample of how to customize the Mail Merge operation and apply formatting to the cells.

{{< gist aspose-com-gists ef6c4280ab216d12222a5c252b936892 "custom-mail-merge.java" >}}

## Conclusion

Mail Merge provides you with a wide range of features to generate MS Word documents dynamically. You can generate simple as well as complex reports based on the data in databases or other data sources. In this article, you have seen how to implement the Mail Merge features programmatically using Java. You can learn more about the Java Mail Merge API using the [documentation][30].

## See Also

*   [Create Rich Word Documents Programmatically in Java][31]




[1]: #About-Mail-Merge
[2]: #Java-Mail-Merge-API
[3]: #Data-Sources-for-Mail-Merge
[4]: #Prepare-Mail-Merge-Template
[5]: #Create-Mail-Merge-Template-using-Java
[6]: #Perform-Mail-Merge-in-Word-Document-using-Java
[7]: #Mail-Merge-using-XML-Data-Source
[8]: #Mail-Merge-with-Regions
[9]: #Nested-Mail-Merge-Regions
[10]: #Custom-Formatting-of-Merge-Fields
[11]: https://en.wikipedia.org/wiki/Mail_merge
[12]: https://products.aspose.com/words/java
[13]: https://downloads.aspose.com/words/java
[14]: https://docs.fileformat.com/word-processing/docx/)
[15]: https://github.com/aspose-words
[16]: https://apireference.aspose.com/words/java/com.aspose.words/DocumentBuilder
[17]: https://apireference.aspose.com/words/java/com.aspose.words/documentbuilder#insertTextInput(java.lang.String,int,java.lang.String,java.lang.String,int)
[18]: https://apireference.aspose.com/words/java/com.aspose.words/documentbuilder#insertField(int,boolean)
[19]: https://apireference.aspose.com/words/java/com.aspose.words/documentbuilder#insertParagraph()
[20]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[21]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[22]: https://apireference.aspose.com/words/java/com.aspose.words/DocumentBuilder
[23]: https://apireference.aspose.com/words/java/com.aspose.words/mailmerge#execute(com.aspose.words.IMailMergeDataSource)
[24]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[25]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[26]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[27]: https://apireference.aspose.com/words/java/com.aspose.words/mailmerge#FieldMergingCallback
[28]: https://apireference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback#fieldMerging(com.aspose.words.FieldMergingArgs)
[29]: https://apireference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback#imageFieldMerging(com.aspose.words.ImageFieldMergingArgs)
[30]: https://docs.aspose.com/words/java/mail-merge-and-reporting/
[31]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/





