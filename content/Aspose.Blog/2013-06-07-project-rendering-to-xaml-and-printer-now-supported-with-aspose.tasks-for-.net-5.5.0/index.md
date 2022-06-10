---
title: 'Rendering Projects to XAML and Printer Supported by Aspose.Tasks for .NET 5.5.0'
date: Fri, 07 Jun 2013 16:54:18 +0000
draft: false
url: /2013/06/07/project-rendering-to-xaml-and-printer-now-supported-with-aspose.tasks-for-.net-5.5.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

[![Aspose.Tasks for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Tasks-for-net_100.png)

Aspose.Tasks for .NET 5.5.0 has been released with a number of enhancements and bug fixes.

As part of our continuous efforts to make the API rich of useful features, this month's release includes two new features. We now support exporting project to XAML format with the facility to set various rendering options such as setting legends on output pages, applying timescale options and individual Presentation formats. This month's release also supports printing a project to a default or custom printer with different Print options and printer settings.

This month's release also includes an easy way of deep cloning a source project to a target project via a single API call as follow:

```
Project original = new Project("NewProductDev.xml");
string resFile = blank.Replace("New", "Copied");
Project blankMpp = new Project(blank);
original.CopyTo(blankMpp);
blankMpp.Save(resFile, SaveFileFormat.MPP);
```

This month's release also includes a number of bug fixes reported by our value customers/users from time to time. For more details on new features and bug fixes, please visit the [Product Release Page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Tasks-for-net_100.png "Aspose.Tasks for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.tasks-for-.net/default.aspx




