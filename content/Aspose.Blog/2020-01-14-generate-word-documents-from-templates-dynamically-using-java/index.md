---
title: 'Generate Word Documents from Templates Dynamically using Java'
seoTitle: "Generate Word Documents from Templates in Java | Create Word Docs"
description: "Generate Word documents from templates in Java. Create word document by populating template placeholders or tags with Java object values or data sources."
date: Tue, 14 Jan 2020 11:43:18 +0000
draft: false
url: /2020/01/14/generate-word-documents-from-templates-dynamically-using-java/
author: Usman Aziz
summary: ''
tags: ['Create docx file from template in java', 'create word document from word template in java', 'create word document with xml', 'generate word document by template in java', 'generate word document from word template', 'generate word document in java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Generate-Word-from-Template-Java-1.png" alt="Generate word from template in java">}}


The **report generation** process more often consists of populating the predefined document templates containing the placeholders for desired fields. The reporting engines take the template document as input, populate the placeholders with the data dynamically and generate the resultant reports. This article is also going to showcase a similar use case where you can **generate** the **Word documents** by populating the **Word templates** **dynamically** and **programmatically** using **Java**.

To generate Word documents from DOCX templates, we'll use the **[LINQ Reporting Engine][1]** offered by **[Aspose.Words for Java][2]** API. **LINQ Reporting Engine** supports a variety of tags for text, images, lists, tables, hyperlinks, and bookmarks for Word templates. The template documents containing these tags are populated by the engine with data coming from Java objects as well as **XML**, **JSON**, or **CSV** data sources. So let's begin generating the Word documents from the templates using Java.

This article will cover how to generate Word document from a template using:

*   values from the Java objects,
*   XML data source,
*   JSON data source,
*   and CSV data source.

## Installing Aspose.Words for Java - Word Automation and Report Generation API

You can download _Aspose.Words for Java_ [JAR][3] or add it to your Maven-based application using the following configurations.

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-words</artifactId>
    <version>20.1</version>
    <type>pom</type>
</dependency>
```

## Generate Word Documents from Template using Java Objects

To begin the report generation, let's first create a Word document by populating the template with values from the Java objects. In order to define a document template, create a new Word document, insert the following tags and save it as a DOCX document.

```
<<[s.getName()]>> says: "<<[s.getMessage()]>>."
```

In the above template, "_s_" will be treated as an object of Java class that will be used to populate the tags. So let's create a class named _Sender_ with two data members.

{{< gist aspose-com-gists c30329ccddd339ce7f05c1e8cae06aa8 "SenderClass.java" >}}

Now, it is time to pass the Word template to the LINQ Reporting Engine and generate the Word document based on the values of _Sender_'s object. The following are the steps for generating the Word document:

*   Create the [Document][4] object and initialize it with the template's path.
*   Create and initialize an object of _Sender_ class.
*   Create an object of [ReportingEngine][5] class.
*   Build the report using [ReportingEngine.buildReport()][6] method that accepts the document template, the data source, and the name of the data source.
*   Save generated Word document using [Document.save()][7] method.

The following code sample shows how to generate a Word document from a Word template using the values of the Java object.

{{< gist aspose-com-gists c30329ccddd339ce7f05c1e8cae06aa8 "create-word-document-from-template-java-object.java" >}}

### Output



{{< figure align=center src="images/Create-word-document-in-Java.png" alt="generate word document by template with Java objects">}}


## Create Word Documents from Template using XML Data

Let's now take one step further and see how to populate the Word templates using an XML data source in a bit complex scenario. The following is the XML data source that we'll use to populate the Word template.

{{< gist aspose-com-gists c30329ccddd339ce7f05c1e8cae06aa8 "datasource.xml" >}}

In this scenario, we'll use the following tags in the template document for multiple records in the XML data source.

```
<<foreach [in persons]>>Name: <<[Name]>>, Age: <<[Age]>>, Date of Birth: <<[Birth]:"dd.MM.yyyy">>
<</foreach>>
Average age: <<[persons.average(p => p.Age)]>>
```

The Java code for generating Word document, in this case, would be the same and except for passing Java object as the data source, we'll pass the [XmlDataSource][8] object in _ReportingEngine.buildReport()_ method. The following code sample shows how to create a Word document by populating the document template using XML data source in Java.

{{< gist aspose-com-gists c30329ccddd339ce7f05c1e8cae06aa8 "create-word-document-from-template-XML.java" >}}

### Output



{{< figure align=center src="images/Create-word-document-in-Java-using-XML.png" alt="generate word document by template with XML in Java">}}


## Generate Word Documents from Template using JSON Data

Let's now have a look at how to generate Word document from the DOCX template using a JSON data source. Following is the JSON data that we'll use in this example.

{{< gist aspose-com-gists c30329ccddd339ce7f05c1e8cae06aa8 "datasource.json" >}}

In this example, we'll generate the Word document containing a list of the clients grouped by their managers. In accordance with this scenario, the DOCX template will look like the following:

```
<<foreach [in managers]>>Manager: <<[Name]>>
Contracts:
<<foreach [in Contract]>>- <<[Client.Name]>> ($<<[Price]>>)
<</foreach>>
<</foreach>>
```

For loading JSON data source, _Aspose.Words_ provides [JsonDataSource][9] class. The following code sample shows how to create a Word document from the template using a JSON data source in Java.

{{< gist aspose-com-gists c30329ccddd339ce7f05c1e8cae06aa8 "create-word-document-from-template-JSON.java" >}}

### Output



{{< figure align=center src="images/Create-word-document-in-Java-using-JSON.png" alt="create word document with JSON in Java">}}


## Generate Word Documents from Template using CSV Data

Last but not least, let's check out how to generate the Word document by populating the Word template using the following CSV data source.

{{< gist aspose-com-gists c30329ccddd339ce7f05c1e8cae06aa8 "datasource.csv" >}}

The following Word template will be used in this example:

```
<<foreach [in persons]>>Name: <<[Column1]>>, Age: <<[Column2]>>, Date of Birth: <<[Column3]:"dd.MM.yyyy">>
<</foreach>>
Average age: <<[persons.average(p => p.Column2)]>>
```

For dealing with CSV data sources, _Aspose.Words_ offers [CsvDataSource][10] class. The following code sample shows how to generate a Word document using a CSV data source in Java.

{{< gist aspose-com-gists c30329ccddd339ce7f05c1e8cae06aa8 "create-word-document-from-template-CSV.java" >}}

### Output



{{< figure align=center src="images/Create-word-document-in-Java-using-CSV.png" alt="create word document with CSV in java">}}


## Learn more about LINQ Reporting Engine

_LINQ Reporting Engine_ supports a wide range of tags for generating fully-featured Word documents dynamically in Java. You can explore more about these tags along with their syntax in [this article][11].

In case you would have any questions or queries, you can post to [Aspose.Words Forum][12].

## Related Article(s)

*   [Create Rich Word Documents Programmatically in Java][13]
*   [Create, Edit or Parse Word Documents in C#][14]




[1]: https://docs.aspose.com/display/wordsjava/About+this+Guide
[2]: https://products.aspose.com/words/java
[3]: https://downloads.aspose.com/words/java
[4]: https://apireference.aspose.com/java/words/com.aspose.words/Document
[5]: https://apireference.aspose.com/java/words/com.aspose.words/ReportingEngine
[6]: https://apireference.aspose.com/java/words/com.aspose.words/reportingengine#buildReport(com.aspose.words.Document,java.lang.Object,java.lang.String)
[7]: https://apireference.aspose.com/java/words/com.aspose.words/document#save(java.lang.String)
[8]: https://apireference.aspose.com/java/words/com.aspose.words/XmlDataSource
[9]: https://apireference.aspose.com/java/words/com.aspose.words/JsonDataSource
[10]: https://apireference.aspose.com/java/words/com.aspose.words/CsvDataSource
[11]: https://docs.aspose.com/display/wordsjava/Template+Syntax
[12]: https://forum.aspose.com/c/words
[13]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/
[14]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/





