---
title: 'Reading VBA Project Information supported with Aspose.Tasks for Java 9.4.0'
date: Mon, 27 Jun 2016 15:53:16 +0000
draft: false
url: /2016/06/27/reading-vba-project-information-supported-with-aspose.tasks-for-java-9.4.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2016/06/Aspose.Tasks-for-Java.png "Aspose.Tasks for Java")

Aspose.Tasks for Java 9.4.0 has been released. This month’s [release][1] includes a new feature for reading VBA information from Microsoft Project documents. The API can now read VBA project information such as references information, modules information and module attributes information. Since the Java API is auto-ported from its equivalent .NET version, the internal functionality of the API fixes a number of bugs that further improve the overall stability of the API. For a detailed list of what is new and fixed, please visit the product release notes section of this new release.

# New Features & Enhancements

**Reading VBA Project Information:** This month’s release provides the capability to read VBA project information from a Microsoft Project document. The API’s VbaProject class provides the interface for reading this information such as Name, Description, complication arguments and context Id.

**Reading References Information from VBA:** In order to read the references information from the document’s VBA project, the getReferences() method exposed by the VbaProject class can be used. It returns a collection of all the references contained in the VBA project that can be further traversed for information such as Name and Library identifiers.

**Reading Modules Information form VBA:** Module information from a VBA project of a document can be retrieved using the getModules() method of the VbaProject class. It returns a collection of modules contained in the VBA project. Each module can then be retrieved as an instance of IVbaModule that can be used to retrieve information such as module name and source code.

**Reading Module Attributes Information from VBA:** Each module, represented by IVbaModule, gets you access to its attributes information such as Key and values. The getAttributes() method of IVbaModule class can be used to retrieve this information for the selected module.

# Other Improvements

This month’s release also fixes a number of bugs that were reported by our valued customers with the last version of the API. This further aids to the stability of the API in terms of sustainable functionality.

# API Resources

*   Product Documentation – Provides complete information about system requirements, installation, Programmer’s Guide, Technical articles and API Changes
*   API Reference Guide – Provides information about the product namespaces, classes and methods
*   [GitHub Examples][2] – Ready to download and execute examples of the API
*   [Forum Support][3] – Post your queries/inquiries on Aspose.Tasks forum to get support from our technical support team.




[1]: http://www.aspose.com/downloads/tasks/java
[2]: https://github.com/asposetasks/Aspose_TASKS_Java
[3]: https://forum.aspose.com/c/tasks




