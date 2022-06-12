---
title: 'Convert Project Data to XAML using Java'
seoTitle: "Convert Project Data to XAML using Java | MPP to XAML in Java"
description: "Programmatically, convert Project data to XAML using Java with Aspose.Tasks for Java API. Convert MPP to XAML with additional save options in Java."
date: Sun, 12 Jun 2022 08:14:55 +0000
draft: false
url: /2022/06/12/convert-project-data-to-xaml-using-java/
author: Muzammil Khan
summary: 'As a Java developer, we can easily export Microsoft Project data from MPP files to XAML format programmatically in Java applications. In this article, you will learn **how to convert Microsoft Project data to XAML using Java**.'
tags: ['Convert Project to XAML', 'Convert Project to XAML in Java', 'Export Project Data to XAML', 'MPP to XAML', 'MPP to XAML in Java']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/convert-project-data-to-xaml-using-java.jpg" alt="Convert Project Data to XAML using Java">}}


[XAML][1] (E**x**tensible **A**pplication **M**arkup **L**anguage) is a simple and declarative language based on [XML][2]. It is a Microsoft variant of XML to define UI elements, data binding, and events. It enables creating, initializing, and setting the properties of objects with hierarchical relations. XAML is mainly used to create GUI in WPF (Windows Presentation Foundation), Silver light, WF (Workflow Foundation), Win UI (Windows UI Library), UWP (Universal Windows Platform), and Xamarin Forms. In this article, we will learn **how to convert Microsoft Project data to XAML using Java**.

The following topics shall be covered in this article:

1.  [Java API to Convert Project Data to XAML][3]
2.  [Export Project Data to XAML][4]
3.  [Convert MPP to XAML with Additional Options][5]
4.  [Convert MPP to XAML with Presentation Format][6]

## Java API to Convert Project Data to XAML {#Java-API-to-Convert-Project-Data-to-XAML}

For converting MS Project data from MPP to XAML, we will be using the **_[Aspose.Tasks for Java][7]_** API. It allows creating, editing, or manipulating of Microsoft Project files ([MPP][8], [MPT][9], [MPX][10], and [XML][11] programmatically. The _[Project][12]_ class of the API represents a project and exposes various methods to perform different functions. The _[XamlOptions][13]_ class allows specifying additional options while rendering project pages to XAML.

Please either [download][14] the JAR of the API or add the following _**pom.xml**_ configuration in a Maven-based Java application.

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
    <version>22.5</version>
    <classifier>jdk18</classifier>
</dependency>
```

## Export Project Data to XAML in Java {#Export-Project-Data-to-XAML-in-Java}

We can easily export project data from an MPP file to XAML format by following the steps given below:

1.  Load the MPP file using the **_Project_** class.
2.  Save the XAML file using the [save()][15] method. It takes the file path and **_[SaveFileFormat][16]_** as arguments.

The following sample code shows **how to convert MPP files to XAML format in Java**.

{{< gist aspose-tasks-gists 91d34226897652a5ea2b00fbe1fc4718 "Convert-Project-to-XAML-Java_Convert.java" >}}

## Convert MPP to XAML with Additional Options in Java {#Convert-MPP-to-XAML-with-Additional-Options-in-Java}

We can define **_XamlOptions_** like _FitContent_, _LegendOnEachPage_, _TimeScale_, and _View_ while converting MPP to XAML. We can convert the MPP file to XAML with additional options by following the given below steps:

1.  Firstly, load the MPP file using the **_Project_** class.
2.  Next, create an instance of the **_XamlOptions_** class.
3.  After that, set the desired options.
4.  Finally, save the XAML file using the [save()][17] method. It takes the file path and **_SaveFileFormat_** as arguments.

The following sample code shows **how to convert the MPP file to XAML format with additional options in Java**.

{{< gist aspose-tasks-gists 91d34226897652a5ea2b00fbe1fc4718 "Convert-Project-to-XAML-Java_ConvertWithOptions.java" >}}

## Convert MPP to XAML with Presentation Format in Java {#Convert-MPP-to-XAML-with-Presentation-Format-in-Java}

We can use different presentation formats while converting MPP files to XAML format. The [PresentationFormat][18] enumeration of the API provides the following options.

*   _GanttChart_ - Gantt Chart presentation format.
*   _TaskUsage_ - Task usage presentation format.
*   _ResourceUsage_ - Resource usage presentation format.
*   _ResourceSheet_ - Resource sheet presentation format.
*   _TaskSheet_ - Task sheet presentation format.

We can set the presentation format and then convert the MPP file to XAML by following the steps given below:

1.  Firstly, load the MPP file using the **_Project _**class.
2.  Next, create an instance of the _**XamlOptions **_class.
3.  After that, set the presentation format using the**_ setPresentationFormat()_**.
4.  Finally, save the XAML file using the **_save()_** method. It takes the file path and **_SaveFileFormat_** as arguments.

The following sample code shows **how to set the presentation format and convert the MPP file to XAML using Java.**

{{< gist aspose-tasks-gists 91d34226897652a5ea2b00fbe1fc4718 "Convert-Project-to-XAML-Java_SetPresentationFormat.java" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][19] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to load and convert MS Project (MPP) files to XAML in Java. We have also seen how to set XAML save options while exporting project data from MPP to XAML. Besides, you can learn more about **_Aspose.Tasks for Java_** API using the [documentation][20]. In case of any ambiguity, please feel free to contact us on the [forum][21].

## See Also

*   [Read Gantt Chart of Project using Java][22]
*   [Convert MPP to Excel using Java][23]




[1]: https://docs.fileformat.com/web/xaml/
[2]: https://docs.fileformat.com/web/xml/
[3]: #Java-API-to-Convert-Project-Data-to-XAML
[4]: #Export-Project-Data-to-XAML-in-Java
[5]: #Convert-MPP-to-XAML-with-Additional-Options-in-Java
[6]: #Convert-MPP-to-XAML-with-Presentation-Format-in-Java
[7]: https://products.aspose.com/tasks/java/
[8]: https://docs.fileformat.com/project-management/mpp/
[9]: https://docs.fileformat.com/project-management/mpt/
[10]: https://docs.fileformat.com/project-management/mpx/
[11]: https://docs.fileformat.com/project-management/p6xml/)
[12]: https://reference.aspose.com/tasks/java/com.aspose.tasks/project
[13]: https://reference.aspose.com/tasks/java/com.aspose.tasks/XamlOptions
[14]: https://downloads.aspose.com/tasks/java
[15]: https://reference.aspose.com/tasks/java/com.aspose.tasks/project#save(java.lang.String,int)
[16]: https://reference.aspose.com/tasks/java/com.aspose.tasks/SaveFileFormat
[17]: https://reference.aspose.com/tasks/java/com.aspose.tasks/project#save(java.lang.String,int)
[18]: https://reference.aspose.com/tasks/java/com.aspose.tasks/PresentationFormat
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/tasks/java/
[21]: https://forum.aspose.com/c/tasks/
[22]: https://blog.aspose.com/2022/06/08/read-gantt-chart-of-project-using-java/
[23]: https://blog.aspose.com/2022/05/10/convert-mpp-to-excel-using-java/




