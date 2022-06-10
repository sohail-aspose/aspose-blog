---
title: 'Importing Primavera file format and Support for Formulas now available in Asopse.Tasks for .NET 8.1.0'
date: Wed, 11 Mar 2015 14:07:46 +0000
draft: false
url: /2015/03/11/importing-primavera-file-format-and-support-for-formulas-now-available-in-asopse.tasks-for-.net-8.1.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

[![][1]](https://products.aspose.com/tasks/net)

We are pleased to announce the release of Aspose.Tasks for .NET 8.1.0 that includes a number of new features, enhancements and other improvements. The API now supports adding custom fields with formulas, creating and reading custom bar styles, importing Primavera file formats, and others. For a detailed list of changes and downloading the new version, please visit the [product download][2] page. You may also visit our documentation section for having details about the public API changes in this version.

# Importing Primavera XML File Format

We provided the support of exporting project data to Primavera XML and XER file formats in one of our earlier versions. With this month’s release, the API now supports importing Primavera XML file formats. This further enriches the file formats supported by the API.

# Creation of Custom Fields with Formulas

With this month’s release, Aspose.Tasks now supports writing and reading formulas to Microsoft Project data extended attributes. The API’s _ExtendedAttributeDefinition_ class provides the _Formula_ property that can be used to set the formula. Once the formula is set, the extended attribute definition can be applied to a task for viewing the results. The attributes are added with Read-Only Access ot the customer fields and cannot be changed. More Info

# Exporting Project Data to HTML with additional Save Options

This month’s release enhances the feature of exporting project data to HTML by providing additional save options. The _HtmlSaveOptions_ now provides further flexibility for exporting only specific pages to the output. Our documentation section, saving project data as HTML, illustrates this feature with a sample code.

# Moving a Task under another Parent

A child task in can be moved under another task in Microsoft Project (MSP) by simply drag and drop. This moves the task and its children under the new parent. With this month’s release, this can also be achieved with Aspose.Tasks API. An overloaded method of _Add_ has been introduced that accepts another task as input and can be used to move a task under another task as shown in our documentation article, Moving a Task under another Parent.

# Support for Custom Bar Styles Reading/Writing

This month’s release introduces another new feature of reading and writing custom bar style for a task.  A task’s bar style can be customized for its shapes such as Mildde Shape, Start Shape, End Shape, and colors of each one of these. Our documentation article, working with Custom Bar Styles, illustrates this with code sample.

# Bug Fixes

This month’s release also fixes a number of bugs that further improves the overall functionality of the API. This includes exceptions raised during MPP to XML conversion and project recalculation. Additionally, it fixes issues related to tasks indentations, wrong API behavior in manual mode and saving certain project files to disc.

If you have any query or inquiry about the API, please feel free to write to us over [Aspose.Tasks forum][3]. We’ll be glad to assist you further.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/03/aspose-Tasks-for-net_100.png "aspose-Tasks-for-net_100"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.tasks-for-.net/entry611332.aspx
[3]: http://www.aspose.com/community/forums/aspose.tasks-product-family/96/showforum.aspx




