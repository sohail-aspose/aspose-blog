---
title: 'Generate Word Documents from Templates in C# .NET'
seoTitle: "Generate Word Document from Template in C# .NET | .NET Word API"
description: "Generate Word document from template in C# .NET. Dynamically create Word reports from predefined Word templates using objects, CSV, JSON, and XML data in C#."
date: Thu, 05 Mar 2020 16:35:38 +0000
draft: false
url: /2020/03/05/generate-word-documents-from-templates-in-csharp-net/
author: Usman Aziz
summary: ''
tags: ['Create Word document from Template in ASP.NET', 'Dynamically create Word reports from Word templates', 'Generate Word document from template in csharp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Generate-Word-from-Template-C.png" alt="Generate Word from template in C#">}}


The automated generation of Word documents is widely used by enterprises for creating a multitude of reports. In some cases, the documents are created from scratch. On the other hand, predefined templates are used to generate Word documents by populating the placeholders. In this article, I'll demonstrate **how to generate Word documents from templates dynamically and programmatically in C#**. You'll come to know how to populate the Word templates from different types of data sources.

The following scenarios along with the code samples will be covered in this article:

*   [C# Word Automation API][1]
*   [Generate Word document from a template using C# object's values][2]
*   [Generate Word document using an XML data source][3]
*   [Create Word document using a JSON data source][4]
*   [Generate Word document using a CSV data source][5]

## C# Word Automation API {#CSharp-Word-Automation-API}

We'll use [Aspose.Words for .NET][6] - A Word automation API that allows you to generate Word document from scratch or by populating the predefined Word templates. You can either [download][7] API's binaries or install it using one of the following methods.

### Using NuGet Package Manager



{{< figure align=center src="images/Aspose.Words-NuGet.png" alt="">}}


### Using the Package Manager Console```
PM> Install-Package Aspose.Words
```

## Generate Word Document from Template using C# Objects {#Generating-Word-document-from-a-template-using-CSharp-object-values}

First of all, let's see how to populate the Word template using the C# objects. For this, we'll create a Word document (DOC/DOCX) with the following placeholders as the content of the document:

```
<<[sender.Name]>> says: "<<[sender.Message]>>."
```

Here, the _sender_ is the object of the following class that we'll use to populate the template.

\[gist id="4f0e741d863333a8ea3874eadaf34372" file="sender.cs"\]

Now, we'll use the reporting engine of _Aspose.Words_ to generate the Word document from the template and the object of _Sender_ class by following the below steps.

*   Create an object of the [Document][8] class and initialize it with the Word template's path.
*   Create and initialize an object of _Sender_ class.
*   Instantiate [ReportingEngine][9] class.
*   Populate the templates using [ReportingEngine.BuildReport()][10] that takes the _Document_'s object, data source and the name of the data source as parameters.
*   Save generated Word document using [Document.Save()][11] method.

The following code sample shows how to generate a Word document from template in C#.

\[gist id="4f0e741d863333a8ea3874eadaf34372" file="generate-word-from-template-object.cs"\]

### Output



{{< figure align=center src="images/Create-word-document-in-Java.png" alt="">}}


## Generate Word Document from an XML Data Source in C# {#Generating-Word-document-using-an-XML-data-source}

For generating the Word document from an XML data source, we'll use a bit more complex Word template with the following placeholders:

```
<<foreach [in persons]>>Name: <<[Name]>>, Age: <<[Age]>>, Date of Birth: <<[Birth]:"dd.MM.yyyy">>
<</foreach>>
Average age: <<[persons.Average(p => p.Age)]>>
```

The XML data source I have used in this example is given below.

\[gist id="4f0e741d863333a8ea3874eadaf34372" file="datasource.xml"\]

The following are the steps to generate a Word document from an XML data source:

*   Create an instance of the _Document_ class and initialize it with the Word template's path.
*   Create an instance of the [XmlDataSource][12] class and initialize it with the XML file's path.
*   Instantiate _ReportingEngine_ class.
*   Use _ReportingEngine.BuildReport()_ method in the same way we have used before to populate the Word template.
*   Save the generated Word document using _Document.Save()_ method.

The following code sample shows how to generate a Word document from an XML data source in C#.

\[gist id="4f0e741d863333a8ea3874eadaf34372" file="generate-word-from-template-XML.cs"\]

### Output



{{< figure align=center src="images/Create-word-document-in-Java-using-XML.png" alt="">}}


## Generate Word Document from a JSON Data Source in C# {#Generate-Word-Document-from-a-JSON-Data-Source-in-CSharp}

Let's now see how to generate a Word document using a JSON data source. In this example, we'll generate a list of the clients that are grouped by their managers. The following would be the Word template in this case:

```
<<foreach [in managers]>>Manager: <<[Name]>>
Contracts:
<<foreach [in Contract]>>- <<[Client.Name]>> ($<<[Price]>>)
<</foreach>>
<</foreach>>
```

The following would be the JSON data source that we'll use to populate the template:

\[gist id="4f0e741d863333a8ea3874eadaf34372" file="datasource.json"\]

For generating the Word document from JSON, we'll use the [JsonDataSource][13] class for loading and using the JSON data source and the rest of the steps will remain the same. The following code sample shows how to generate a Word document from the template using JSON in C#.

\[gist id="4f0e741d863333a8ea3874eadaf34372" file="generate-word-from-template-JSON.cs"\]

### Output



{{< figure align=center src="images/Create-word-document-in-Java-using-JSON.png" alt="">}}


## Generate Word Document from CSV Data Source in C# {#Generating-Word-document-using-a-CSV-data-source}

For generating the Word document from CSV, we'll use the following Word template:

```
<<foreach [in persons]>>Name: <<[Column1]>>, Age: <<[Column2]>>, Date of Birth: <<[Column3]:"dd.MM.yyyy">>
<</foreach>>
Average age: <<[persons.Average(p => p.Column2)]>>
```

The template will be populated with the following CSV data:

\[gist id="4f0e741d863333a8ea3874eadaf34372" file="datasource.csv"\]

Now, lets come to the C# code. All the steps will remain the same here as well except for the one change that is we'll use the [CsvDataSource][14] class to load the CSV data. The following code sample shows how to generate the Word document from a CSV data source.

\[gist id="4f0e741d863333a8ea3874eadaf34372" file="generate-word-from-template-CSV.cs"\]

### Output



{{< figure align=center src="images/Create-word-document-in-Java-using-CSV.png" alt="">}}


## Try Aspose.Words for .NET for Free

You can try _Aspose.Words for .NET_ using a free [temporary license][15].

## Conclusion

In this article, you have learned how to generate Word documents from templates using C#. Furthermore, you have seen how to use objects, XML, JSON and CSV data sources to generate Word documents. You can explore more about the C# Word automation API using [documentation][16]. In addition, you can contact us via our [forum][17].

## See Also

*   [.NET Word Automation – Create, Edit or Convert MS Word Documents using C#][18]



[1]: #CSharp-Word-Automation-API
[2]: #Generating-Word-document-from-a-template-using-CSharp-object-values
[3]: #Generating-Word-document-using-an-XML-data-source
[4]: #Generate-Word-Document-from-a-JSON-Data-Source-in-CSharp
[5]: #Generating-Word-document-using-a-CSV-data-source
[6]: https://products.aspose.com/words/net
[7]: https://downloads.aspose.com/words/net
[8]: https://apireference.aspose.com/net/words/aspose.words/document
[9]: https://apireference.aspose.com/net/words/aspose.words.reporting/reportingengine
[10]: https://apireference.aspose.com/net/words/aspose.words.reporting.reportingengine/buildreport/methods/1
[11]: https://apireference.aspose.com/net/words/aspose.words.document/save/methods/2
[12]: https://apireference.aspose.com/net/words/aspose.words.reporting/xmldatasource
[13]: https://apireference.aspose.com/net/words/aspose.words.reporting/jsondatasource
[14]: https://apireference.aspose.com/net/words/aspose.words.reporting/csvdatasource
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/words/net/
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/





