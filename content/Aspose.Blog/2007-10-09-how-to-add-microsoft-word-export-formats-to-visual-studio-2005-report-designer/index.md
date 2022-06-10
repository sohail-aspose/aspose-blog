---
title: 'How to Add Microsoft Word Export Formats to Visual Studio 2005 Report Designer'
date: Tue, 09 Oct 2007 20:07:00 +0000
draft: false
url: /2007/10/09/how-to-add-microsoft-word-export-formats-to-visual-studio-2005-report-designer/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

It's a bit shameful but until recently I was almost sure that the Visual Studio 2005 Report Designer (Business Intelligence Development Studio) does not support custom rendering extensions and the export formats are hard coded :) Thanks to one of our customers, it turned out I was wrong. So, since Aspose.Words for Reporting Services is a rendering extensions allowing to export RDL reports to Microsoft Word formats, you can easily add those formats directly to your report designer. Moreover, starting with the version 1.4.2.0, the MSI installer adds the formats automatically if it detects Visual Studio 2005 Report Designer on your machine. If you need to do that manually though, just follow these simple steps:

1.  Open the C:\\Program Files\\Microsoft Visual Studio 8\\Common7\\IDE\\PrivateAssemblies folder. 
2.  Copy Aspose.Words.ReportingServices.dll to that folder. 
3.  Locate two files in the folder: RSReportDesigner.config and RSPreviewPolicy.config and edit them exactly as you do when installing Aspose.Words for Reporting Services manually, that is edit RSReportDesigner.config as rsreportserver.config and RSPreviewPolicy.config as rssrvpolicy.config. You can read how to edit these files [here][1].
4.  Reload Visual Studio.

Now you are able to export your reports to Word documents right at design time, without the need to upload them to Report Server first. This feature is very handy and will greatly save your time!




[1]: http://www.aspose.com/Products/Aspose.Words.Reporting.Services/Api/InstallManually.html




