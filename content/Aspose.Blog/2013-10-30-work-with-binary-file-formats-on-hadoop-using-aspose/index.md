---
title: 'Work with Binary File Formats on Hadoop using Aspose'
date: Wed, 30 Oct 2013 11:43:02 +0000
draft: false
url: /2013/10/30/work-with-binary-file-formats-on-hadoop-using-aspose/
author: Msabir
summary: ''
tags: []
categories: ['Aspose.Words Product Family', 'Aspose.Total Product Family', 'Aspose.Cells Product Family', 'Aspose.Email Product Family', 'Aspose.Slides Product Family']
---

Apache Hadoop has great capabilities for archiving big data through its flexible distributed file system (HDFS) across several nodes. This big data solution is also powered by the MapReduce Framework which enables developers to analyze the archived data through its APIs. The big data may be structured or unstructured and may be in any file format. Keeping this in mind, we have the released first version of the Aspose for Hadoop project which enables developers to work with a number of file formats. Below is a list of the file formats supported in the initial version:

*   Microsoft Word (DOC)
*   WordprocessingML (DOCX, XML)
*   Rich Text Format (RTF)
*   HTML, XHTML and MHTML
*   OpenDocument (ODT)
*   Microsoft Excel (XLS)
*   SpreadsheetML (XLSX, XML)
*   OpenDocument Spreadsheet (ODS)
*   PresentationML (PPTX, XML)
*   Outlook Emails (MSG)

Using the Aspose for Hadoop project, the Hadoop developers can parse text from any of the above formats. The text can then be used in MapReduce analysis algorithms or for any other purpose depending on the use case. The project comes up with two packages:

*   **com.aspose.hadoop.core** - Provides Aspose for Java wrapper classes to parse text from the above formats. The package includes a couple of classes to override Hadoop input formats so the binary sequence files can be created.
*   **com.aspose.hadoop.examples** - Provides mapper examples for creating and converting binary sequence files for all the supported formats into text sequence files.

The project can be downloaded from Github: [https://github.com/asposemarketplace/Aspose\_for\_Hadoop/][1]

The project readme file explains the project flow and usage. If you have any inquiries, suggestions, or confusion, we are keen to hear back from you. Inquiries can be posted in our forums or the GitHub [project repository][2].




[1]: https://github.com/asposemarketplace/Aspose_for_Hadoop/
[2]: https://github.com/asposemarketplace/Aspose_for_Hadoop/




