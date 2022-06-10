---
title: 'Added new Configuration Option to Control Table Position in Aspose.Words for JasperReports 2.7.2'
date: Thu, 21 Jul 2016 17:19:34 +0000
draft: false
url: /2016/07/21/added-new-configuration-option-to-control-table-position-in-aspose.words-for-jasperreports-2.7.2/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/jasperreports/word-component.aspx)We are pleased to announce a new release of Aspose.Words for JasperReports that includes fix of issues related to hyperlinks and subreports in exported documents. You can download the latest release of Aspose.Words for JasperReports from the following link:

[Download Aspose.Words for JasperReports 2.7.2][1]

Starting from release **1.9.0** there are several versions of jar library (necessary for better support of older versions of JasperReports). These include:

*   for JasperReports 5.6.0 ... 6.2.0 (**aspose.words.jasperreports-6.2.0.jar**)
*   for JasperReports 4.7.0 ... 5.5.0 (**aspose.words.jasperreports-5.5.0.jar**)
*   for JasperReports 3.7.2 ... 4.5.0 (**aspose.words.jasperreports-4.5.0.jar**)
*   for JasperReports 3.7.1 and lower (**aspose.words.jasperreports-3.7.1.jar**)

Please copy **only one** jar library according to the version of installed JasperReports.

## Bug Fixes and Features

*   WORDSJSP-179 (Hyperlinks are not exported in output Word document)
*   WORDSJSP-180 (Subreport contents are exported incorrectly in Docx)
*   WORDSJSP-181 (java.lang.NullPointerException is thrown while exporting list of .Jrprint files to Doc/Docx)

## Added new Configuration Option to Control Table Position

We have introduced a new configuration option USE\_POSITIONING\_TABLES to control table position. By default, its value is false. This means that Aspose Words for JasperReports will try to avoid positioning tables where possible. However, you can enable this option (set to true) if you need to force usage of positioning tables (for example, for complex reports with hierarchy of subreports, frames etc).

**In JasperReports:**

```
 import com.aspose.words.jasperreports.*;

   AWDocExporter exporter = new AWDocExporter();
   exporter.setParameter(AWExporterParameter.USE_POSITIONING_TABLES, true);
   exporter.exportReport(); 
```

**In JasperServer:**

```
<bean id="aw_exportParameters" class="com.aspose.words.jasperreports.AWExportParametersBean">
    <property name="usePositioningTables" value="true"/>
</bean> 
```




[1]: http://www.aspose.com/downloads/words-family/jasperreports




