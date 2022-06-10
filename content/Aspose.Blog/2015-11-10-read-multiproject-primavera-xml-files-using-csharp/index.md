---
title: 'Read MultiProject Primavera XML Files using C#'
date: Tue, 10 Nov 2015 12:53:08 +0000
draft: false
url: /2015/11/10/read-multiproject-primavera-xml-files-using-csharp/
author: Muhammad Waqas
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/aspose-Tasks-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Tasks for .NET 8.9.0][1]. This month’s release includes new features, enhancements, and bug fixes that further improve the overall functionality of the API. Our documentation section, Public API changes in Aspose.Tasks for .NET 8.9.0, lists all the changes that are part of this month’s release.

## Read Primavera XML File with Multiple Projects

A Primavera XML project file may contain more than one project where each project is represented by its unique project id. Aspose.Tasks API now provides the capability to read a specific project from such an XML file using its unique id. This is achieved using the new class, PrimaveraXMLReadingOptions, which provides the option to specify the project unique id to be loaded.

## XML Save Options

It is common for Primavera XML file not to have any WBS inside i.e. contains only activities. Aspose.Tasks can’t read properly such type of file as it needs a root task to create a tree of tasks. In this case, the API creates a Root task even if it doesn’t exist in the file in order to be able to read these particular files. The API now provides PrimaveraXmlOptions to save the XML file with or without the created root task. By default, this value is set to true.

## Add Images to a Page’s Header/Footer

This month’s release also introduces an enhancement of working with a page’s header/footer. Microsoft Project has the feature of adding image to a page’s header/footer that is part of the output then. Aspose.Tasks API now provides the same capability of including image in a page header/footer.

## Other Improvements

This month’s release also fixes a number of bugs related to various functional areas of the API. These include:

*   Loss of split tasks while saving MPP project file
*   Issue with reading outline value properties
*   Problems reading information from Primavera XML files such as wrong dates, calendar exceptions, and durations
*   Exception while loading certain Primavera XML files

# API Resources

You may visit the following API resources for getting started and working with the API.

*   [Product Documentation][2] – Detailed API documentation with code examples and details about API functional areas
*   [API Reference Guide][3] - Detailed information about the API namespaces and classes
*   [GitHub Examples][4] – Ready to run code samples in downloadable form
*   [Aspose.Tasks Forum][5] – Our online support forum where we address your queries and inquiries




[1]: https://products.aspose.com/tasks/net
[2]: https://docs.aspose.com/tasks/net
[3]: https://apireference.aspose.com/tasks/net
[4]: https://github.com/asposetasks/Aspose_Tasks_NET
[5]: http://www.aspose.com/community/forums/aspose.tasks-product-family/96/showforum.aspx




