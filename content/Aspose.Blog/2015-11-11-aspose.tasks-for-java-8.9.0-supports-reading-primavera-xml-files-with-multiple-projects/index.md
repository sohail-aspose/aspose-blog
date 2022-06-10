---
title: 'Aspose.Tasks for Java 8.9.0 supports Reading Primavera XML files with Multiple Projects'
date: Wed, 11 Nov 2015 14:33:23 +0000
draft: false
url: /2015/11/11/aspose.tasks-for-java-8.9.0-supports-reading-primavera-xml-files-with-multiple-projects/
author: Muhammad Waqas
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

[![][1]](http://www.aspose.com/java/project-management-component.aspx)

We are pleased to announce the release of [Aspose.Tasks for Java 8.9.0][2]. This month’s release includes enhancements to the API functionality of working with Primavera file formats. In addition, it fixes a number of bugs that further improves the overall API functionality. A complete list of all API changes can be found in our documentation section, Public API Changes in Aspose.Tasks for Java 8.9.0.

# Enhancements

**Loading Primavera XML file with Multiple Projects:** Aspose.Tasks API already supports working with Primavera XML files. Such XML file may contain more than one project in a single file where each project is identified through its unique id. Like its equivalent .NET version, this month’s release provides the capability to read individual project from such project documents using its unique id. A new class, PrimaveraXmlReadingOptions, has been included in the API now for specifying the project’s unique id for loading.

**Primavera XML Save Options:** Aspose.Tasks API now supports adding a Root task to a project file in case it is not already available. This helps the API reading Primavera XML files that does not have any Work Break Down (WBS) inside and contains only activities. In addition, the API now provides the PrimaveraXmlOptions class to save the XML file with or without the created root task. The value of this flag is set to true by default.

# Other Improvements

This month’s release also fixes a number of bugs that were reported with our last month’s release. For a detailed list of what is new and fixed, please the [product download page][3] of Aspose.Tasks for Java API.

# API Resources

*   Product Documentation – Provides complete information about system requirements, installation, Programmer’s Guide, Technical articles and API Changes
*   API Reference Guide – Provides information about the product namespaces, classes and methods
*   [GitHub Examples][4] – Ready to download and execute examples of the API
*   [Forum Support][5] - Post your queries/inquiries on Aspose.Tasks forum to get support from our technical support team.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/11/aspose-Tasks-for-Java_100.png "aspose-Tasks-for-Java_100"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.tasks-for-java/default.aspx
[3]: http://www.aspose.com/community/files/72/java-components/aspose.tasks-for-java/default.aspx
[4]: https://github.com/asposetasks/Aspose_TASKS_Java
[5]: http://www.aspose.com/community/forums/aspose.tasks-product-family/96/showforum.aspx




