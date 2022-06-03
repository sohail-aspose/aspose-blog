---
title: 'Convert MPP to Excel using Java'
date: Tue, 10 May 2022 04:56:18 +0000
draft: false
url: /2022/05/10/convert-mpp-to-excel-using-java/
author: 'Muzammil Khan'
summary: 'As a Java developer, you can easily export project data from MPP files to Excel spreadsheets (XLSX) programmatically. In this article, you will learn **how to convert MPP to Excel using Java**.'
tags: ['Convert MPP to Excel in Java', 'Convert MPP to XLSX in Java', 'Export Project Data to Excel', 'MPP to Excel using Java', 'MPP to XLSX Converter', 'MPP to XLSX using Java', 'Save Project as Excel']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/convert-mpp-to-excel-using-java.jpg" alt="Convert MPP to Excel using Java">}}


An MPP file is a project created by Microsoft Project. It allows organizing, tracking, and maintaining projects.  It contains tasks, resources, assignments, timeline, budget, and different other project-related information. We can easily export project data from [MPP][1] files to Excel spreadsheets ([XLSX][2] programmatically in Java. In this article, we will learn **how to convert MPP to Excel using Java**.

The following topics shall be covered in this article:

*   [Java API to Convert MPP to Excel][3]
*   [Convert MPP to Excel][4]
*   [Convert MPP to Excel with Advanced Options][5]

## Java API to Convert MPP to Excel {#Java-API-to-Convert-MPP-to-Excel}

For converting MPP files to Excel, we will be using the [Aspose.Tasks for Java][6] API. It allows creating, editing, or manipulating Microsoft Project files programmatically in Java applications. Please either [download][7] the JAR of the API or add the following _**pom.xml**_ configuration in a Maven-based Java application.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-tasks</artifactId>
    <version>22.4</version>
    <classifier>jdk18</classifier>
</dependency>
```

## Convert MPP to Excel in Java {#Convert-MPP-to-Excel-in-Java}

We can convert the MPP file to an Excel file by following the steps given below:

1.  Firstly, load the _MPP_ file using the **_[Project][8]_** class.
2.  Finally, call the **_[save()][9]_** method to save as _XLSX_. It takes the output file path and **_[SaveFileFormat][10]_** as arguments.

The following code sample shows **how to convert MPP to Excel using Java**.

{{< gist aspose-tasks-gists 51fa245f0ab39913edde7943099e5771 "Convert-MPP-to-Excel-using-Java_Convert.java" >}}



{{< figure align=center src="images/Convert-MPP-to-Excel-in-Java-1024x512.jpg" alt="Convert MPP to Excel in Java." caption="Convert MPP to Excel in Java.">}}


## Convert MPP to Excel with Advanced Options {#Convert-MPP-to-Excel-with-Advanced-Options-in-Java}

We can also apply various settings while converting the MPP file to Excel. For this purpose, the API provides the **_XlsxOptions_** class that allows specifying additional options when rendering project pages to XLSX. We can specify XLSX save options by following the steps given below:

1.  Firstly, load the _MPP_ file using the **_[Project][11]_** class.
2.  Next, create an instance of the **_[XlsxOptions][12]_** class.
3.  After that, set various options such as _PageSize_, _Encoding_, _ResourceView_, _AssignmentView_, etc.
4.  Finally, call the **_[save()][13]_** method to save as _XLSX_. It takes the output file path and **_[SaveOptions][14]_** as arguments.

The following code sample shows **how to convert MPP to XLSX with advanced options using Java**.

{{< gist aspose-tasks-gists 51fa245f0ab39913edde7943099e5771 "Convert-MPP-to-Excel-using-Java_Convert_with_Options.java" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][15] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   save MS Project data as an XLSX file in Java;
*   set various options to export data from MPP to Excel programmatically.

Besides, you can learn more about [Aspose.Tasks][16] for Java API using the [documentation][17]. In case of any ambiguity, please feel free to contact us on the [forum][18].

## See Also

*   [Convert MS Project MPP Files to SVG Format using Java][19]
*   [Convert MPP Microsoft Project File to PDF Programmatically in Java][20]




[1]: https://docs.fileformat.com/project-management/mpp/
[2]: https://docs.fileformat.com/spreadsheet/xlsx/)
[3]: #Java-API-to-Convert-MPP-to-Excel
[4]: #Convert-MPP-to-Excel-in-Java
[5]: #Convert-MPP-to-Excel-with-Advanced-Options-in-Java
[6]: https://products.aspose.com/tasks/java/
[7]: https://downloads.aspose.com/tasks/java
[8]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project
[9]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/project#save(java.lang.String,int)
[10]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/SaveFileFormat
[11]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project
[12]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/XlsxOptions
[13]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/project#save(java.lang.String,com.aspose.tasks.SaveOptions)
[14]: http://SaveOptions
[15]: https://purchase.aspose.com/temporary-license
[16]: https://products.aspose.com/tasks/
[17]: https://docs.aspose.com/tasks/java/
[18]: https://forum.aspose.com/c/tasks/15
[19]: https://blog.aspose.com/2021/10/29/convert-ms-project-mpp-files-to-svg-format-using-java/
[20]: https://blog.aspose.com/2021/04/26/convert-mpp-pdf-java/




