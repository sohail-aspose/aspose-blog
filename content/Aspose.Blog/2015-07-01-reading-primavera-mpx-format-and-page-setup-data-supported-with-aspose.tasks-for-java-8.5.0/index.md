---
title: 'Reading Primavera MPX format and Page Setup Data supported with Aspose.Tasks for Java 8.5.0'
date: Wed, 01 Jul 2015 19:03:24 +0000
draft: false
url: /2015/07/01/reading-primavera-mpx-format-and-page-setup-data-supported-with-aspose.tasks-for-java-8.5.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

[![][1]](http://www.aspose.com/java/project-management-component.aspx)

We are pleased to announce the release of [Aspose.Tasks for Java 8.5.0][2]. This month’s release introduces new features of reading Primavera MPX format files, header and footer data, and adding extended attributes to resource assignments for visibility in Microsoft Project (MSP). It also provides a number of enhancements and other improvements by fixing various functionality bugs. For a complete list of API changes, please refer to our documentation section, Public API changes in Aspose.Tasks for Java 8.5.0.

# New Features &Enhancements

**Support for reading Primavera MPX Format:** Aspose.Tasks for Java now supports reading project data from Primavera MPX format. The same Project class constructor can be used to load by specifying the stream or path to the MPX file. More Info

**Reading Page Setup Information from MPP file:** Page setup information about a Project file spans on a separate dialog in Microsoft Project to provide all page settings of the document. Aspose.Tasks API now provides the capability of reading the page setup information from the MPP file using the PageInfo class. This class provides information about:

*   Page headers and footers
*   Page settings
*   Page view settings
*   Page margins
*   Legends

A detailed example about demonstration of this feature is available in our documentation article Reading Page Setup Information from MPP file.

**Ignoring Invalid Characters during reading MPP file:** Project files may have invalid characters in the custom fields. MS Project does not allow invalid character so the files have been created or manipulated with automation or some other tools. If these be loaded using the API, they may lead to exception. In order to ignore such invalid characters, the overloaded constructor of Project class can be used with the delegate method _ParseErrorCallBack_. More Info

**Extracting Embedded Objects from Task/Resource View:** Embedded objects (those which were created from file by selecting a file path) are packed into OLE Package inside MPP file. Aspose.Tasks for Java API allows extracting embedded objects from a Task or Resource view. The _OleObject_ class contains information about the embedded objects in Task or Resource View. More Info

# Other Improvements

This month’s release also includes a number of bug fixes that further improves the API functionality. These also include some calculation bugs that could have effect on the generated output.

As always, we welcome your queries/inquiries and are always to answer these on [Aspose.Tasks forum][3].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/07/aspose-Tasks-for-Java_100.png "aspose-Tasks-for-Java_100"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.tasks-for-java/entry637742.aspx
[3]: https://forum.aspose.com/c/tasks




