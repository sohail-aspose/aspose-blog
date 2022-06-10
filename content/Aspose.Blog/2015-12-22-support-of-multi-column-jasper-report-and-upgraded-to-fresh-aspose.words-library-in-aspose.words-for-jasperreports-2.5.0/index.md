---
title: 'Support of Multi Column Jasper Report and Upgraded to Fresh Aspose.Words Library in Aspose.Words for JasperReports 2.5.0'
date: Tue, 22 Dec 2015 14:47:03 +0000
draft: false
url: /2015/12/22/support-of-multi-column-jasper-report-and-upgraded-to-fresh-aspose.words-library-in-aspose.words-for-jasperreports-2.5.0/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/jasperreports/word-component.aspx)We are pleased to announce a new release of Aspose.Words for JasperReports that includes a number of fixes for issues reported by our customers and some improvements. You can download the latest release of Aspose.Words for JasperReports from the following link:

*   [Download Aspose.Words for JasperReports 2.5.0][1]

Starting from release 1.9.0 there are several versions of jar library (necessary for better support of older versions of JasperReports). These include:

*   for JasperReports 5.6.0 ... 6.1.1 (aspose.words.jasperreports-6.0.1.jar)
*   for JasperReports 4.7.0 ... 5.5.0 (aspose.words.jasperreports-5.5.0.jar)
*   for JasperReports 3.7.2 ... 4.5.0 (aspose.words.jasperreports-4.5.0.jar)
*   for JasperReports 3.7.1 and lower (aspose.words.jasperreports-3.7.1.jar)

Please copy only one jar library according to the version of installed JasperReports.

## Bug Fixes and Features

*   WORDSJSP-138 (Contents of Docx move to next page after conversion from .jrprint file to Docx)
*   WORDSJSP-166 (Problem is in direct left indent of paragraphs in output document)
*   WORDSJSP-171 (WORDSJSP-170 was not fully resolved not in resolved)
*   WORDSJSP-148 (Add configuring option to export multi column Jasper Report as two columns Word layout)

## Upgraded to Fresh Aspose.Words Library

Aspose.Words for JasperReports 2.5.0 has been upgraded to Aspose.Words v15.11.0

## New Configuring option is Added to Export Multi Column Jasper Report

By default Aspose.Words for JasperReports use 1 column in output report. But you can change the default value by specifying the required number of columns (between 1 and 4). Use the following parameter for that:  
**JasperReports:**

```
import com.aspose.words.jasperreports.*;

AWDocExporter exporter = new AWDocExporter();
exporter.setParameter(AWExporterParameter.COLUMNS_COUNT, 2);
exporter.exportReport(); 
```

You can also find these bug fixes and improvements in the download page link above.




[1]: http://www.aspose.com/community/files/67/jasperreports-exporters/aspose.words-for-jasperreports/default.aspx




