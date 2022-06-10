---
title: 'Support of JasperServer 6.1.1 and Document export with specific paper size in Aspose.Words for JasperReports 2.4.0'
date: Wed, 25 Nov 2015 15:56:47 +0000
draft: false
url: /2015/11/25/support-of-jasperserver-6.1.1-and-document-export-with-specific-paper-size-in-aspose.words-for-jasperreports-2.4.0/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/jasperreports/word-component.aspx)We are pleased to announce a new release of Aspose.Words for JasperReports that includes a number of fixes for issues reported by our customers and some improvements. You can download the latest release of Aspose.Words for JasperReports from the following link:

*   [Download Aspose.Words for JasperReports 2.4.0][1]

Starting from release 1.9.0 there are several versions of jar library (necessary for better support of older versions of JasperReports). These include:

*   for JasperReports 5.6.0 ... 6.1.1 (aspose.words.jasperreports-6.0.1.jar)
*   for JasperReports 4.7.0 ... 5.5.0 (aspose.words.jasperreports-5.5.0.jar)
*   for JasperReports 3.7.2 ... 4.5.0 (aspose.words.jasperreports-4.5.0.jar)
*   for JasperReports 3.7.1 and lower (aspose.words.jasperreports-3.7.1.jar)

Please copy only one jar library according to the version of installed JasperReports.

## Bug Fixes and Features

*   WORDSJSP-169 (Support JasperServer 6.1.1)
*   WORDSJSP-162 (Export output document with specific paper size)
*   WORDSJSP-163 (Text formatting of empty text field is lost in output Docx)
*   WORDSJSP-164 (Charts do not export in output documents)
*   WORDSJSP-167 (AWDocxExporter.setParameter is deprecated now)
*   WORDSJSP-168 (Issue with scaling of svg images in word documents)
*   WORDSJSP-170 (Section breaks are inserted in output Docx)

## Support JasperServer 6.1.1

Aspose.Words for JasperReports 2.4.0 supports JasperServer 6.1.1

## Export output document with specific paper size

New config options are introduced - PAGE\_SIZE and PAGE\_ORIENTATION to export document with specific page size. You can change the default values by specifying what page size/orientation the exporter should enforce. Use the following parameter for that:  
**JasperReports:**

```
 import com.aspose.words.jasperreports.*;

   AWDocExporter exporter = new AWDocExporter();
   exporter.setParameter(AWExporterParameter.PAGE_SIZE, “Letter”);
   exporter.setParameter(AWExporterParameter.PAGE_ORIENTATION, “Landscape”);
   exporter.exportReport(); 
```

You can also find these bug fixes and improvements in the download page link above.



[1]: http://www.aspose.com/community/files/67/jasperreports-exporters/aspose.words-for-jasperreports/default.aspx




