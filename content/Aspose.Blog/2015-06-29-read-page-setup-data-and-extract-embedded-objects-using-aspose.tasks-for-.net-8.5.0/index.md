---
title: 'Read Page Setup Data and Extract Embedded Objects using Aspose.Tasks for .NET 8.5.0'
date: Mon, 29 Jun 2015 17:46:55 +0000
draft: false
url: /2015/06/29/read-page-setup-data-and-extract-embedded-objects-using-aspose.tasks-for-.net-8.5.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

[![][1]](https://products.aspose.com/tasks/net)[Aspose.Tasks for .NET 8.5.0][2] has been released. This month’s release includes new features of retrieving Page setup information from MPP file, and enhancements such as reading embedded objects and ignoring invalid characters while reading such MPP files. Our documentation section, Public API Changes in Aspose.Tasks for .NET 8.5.0, lists all the API changes that are part of this release. For further queries, please feel free to reach us over [Aspose.Tasks forum][3].

# New Features & Enhancements

This section provides details about the new features as well as enhancements that are part of this month’s release.

**Retrieving Page Setup Data from MPP File:** Microsoft Project provides complete Page setup dialog with 6 tabs that can be used to configure headers, footers, legend, margin and other information. Aspose.Tasks API now provides the capability to retrieve this information using the PageInfo class. More Info

**Extracting Embedded Objects Data:** Microsoft Project data files (MPP/XML) may contain embedded objects such as documents, excel sheets, PDF, images etc. in Task or Resource views. Aspose.Tasks API provides the capability to extract these from a project's Task or Resource. The Project class provides OleObjects collection that contains all the embedded objects of the Project for accessing. More Info

**Ignoring Invalid Characters from Custom Fields:** Some Project files may have invalid characters in the custom fields. Though MS Project does not allow invalid character, such files can be created or manipulated with automation or some other tools. If these are tried to be loaded using the API, they may lead to exception. In order to ignore such invalid characters, the overloaded constructor of Project class can be used with the delegate method _ParseErrorCallBack_. More Info

# Other Improvements

This month’s release also includes other improvements by fixing a number of bugs such as wrong calculation of assignment units after changing the task duration. This, combined with other internal improvements in the API, lead to further improvements in API functionality.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/06/aspose-Tasks-for-net_1001.png "aspose-Tasks-for-net_100"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.tasks-for-.net/entry637735.aspx
[3]: http://www.aspose.com/community/forums/aspose.tasks-product-family/96/showforum.aspx




