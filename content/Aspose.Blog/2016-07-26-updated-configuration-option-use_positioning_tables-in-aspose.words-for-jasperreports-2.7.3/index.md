---
title: 'Updated Configuration Option (USE_POSITIONING_TABLES) in Aspose.Words for JasperReports 2.7.3'
date: Tue, 26 Jul 2016 11:52:08 +0000
draft: false
url: /2016/07/26/updated-configuration-option-use_positioning_tables-in-aspose.words-for-jasperreports-2.7.3/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/jasperreports/word-component.aspx)We are pleased to announce a new release of Aspose.Words for JasperReports that includes fix of issue related to section breaks in exported documents. You can download the latest release of Aspose.Words for JasperReports from the following link:

[Download Aspose.Words for JasperReports 2.7.3][1]

Starting from release **1.9.0** there are several versions of jar library (necessary for better support of older versions of JasperReports). These include:

*   for JasperReports 5.6.0 ... 6.2.0 (**aspose.words.jasperreports-6.2.0.jar**)
*   for JasperReports 4.7.0 ... 5.5.0 (**aspose.words.jasperreports-5.5.0.jar**)
*   for JasperReports 3.7.2 ... 4.5.0 (**aspose.words.jasperreports-4.5.0.jar**)
*   for JasperReports 3.7.1 and lower (**aspose.words.jasperreports-3.7.1.jar**)

Please copy **only one** jar library according to the version of installed JasperReports.

## Bug Fix

*   WORDSJSP-182 (Position of Section break (new page) is incorrect in output Docx/Doc)

## Updated Configuration Option to Control Table Position

Configuration option USE\_POSITIONING\_TABLES has been changed.

*   (USE\_POSITIONING\_TABLES\_NONE) : Aspose Words for JasperReports will never use positioning tables.
*   (USE\_POSITIONING\_TABLES\_ALWAYS) : This option forces usage of positioning tables (for example, for complex reports with hierarchy of subreports, frames etc).
*   (USE\_POSITIONING\_TABLES\_SMART) : Use this option to use adaptive algorithm – positioning tables will be used only where they are required.

**In JasperReports:**

```
 import com.aspose.words.jasperreports.*;

   AWDocExporter exporter = new AWDocExporter();
   exporter.setParameter(AWExporterParameter.USE_POSITIONING_TABLES, AWExporterParameter.USE_POSITIONING_TABLES_SMART);
   exporter.exportReport(); 
```

**In JasperServer:**

```
<bean id="aw_exportParameters" class="com.aspose.words.jasperreports.AWExportParametersBean">
    <property name="usePositioningTables" value="2"/>
</bean> 
```




[1]: http://www.aspose.com/downloads/words-family/jasperreports




