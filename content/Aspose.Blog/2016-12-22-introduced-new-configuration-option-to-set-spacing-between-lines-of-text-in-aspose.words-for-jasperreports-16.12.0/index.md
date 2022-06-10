---
title: 'Introduced New Configuration Option to Set Spacing Between Lines of Text in Aspose.Words for JasperReports 16.12.0'
date: Thu, 22 Dec 2016 08:19:10 +0000
draft: false
url: /2016/12/22/introduced-new-configuration-option-to-set-spacing-between-lines-of-text-in-aspose.words-for-jasperreports-16.12.0/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](https://www.aspose.com/products/words/jasperreports)We are pleased to announce a new release of Aspose.Words for JasperReports that includes fix of issues reported by our customers. You can download the latest release of Aspose.Words for JasperReports from the following link:

[Download Aspose.Words for JasperReports 16.12.0][1]

Starting from release **1.9.0** there are several versions of jar library (necessary for better support of older versions of JasperReports). These include:

*   for JasperReports 6.3.0 and higher (**aspose.words.jasperreports-6.3.0.jar**)
*   for JasperReports 5.6.0 ... 6.2.0 (**aspose.words.jasperreports-6.2.0.jar**)
*   for JasperReports 4.7.0 ... 5.5.0 (**aspose.words.jasperreports-5.5.0.jar**)
*   for JasperReports 3.7.2 ... 4.5.0 (**aspose.words.jasperreports-4.5.0.jar**)
*   for JasperReports 3.7.1 and lower (**aspose.words.jasperreports-3.7.1.jar**)

Please copy **only one** jar library according to the version of installed JasperReports.

## Bug Fixes

*   WORDSJSP-195 (Multiple appearance of elements in exported Docx)
*   WORDSJSP-196 (Extra section break is appeared in output Docx)

## Use Line Spacing

By default, value of **USE\_LINE\_SPACINGS** parameter is “smart” (set to **2**). This means that Aspose Words for JasperReports will try to analyze current context and set spacings between lines of texts only where this is required. However, you can forcibly enable this option (set to **1**) and in this case, line spacings will be set for each text. Alternatively, you can forcibly disable this option (set to **0**) and in this case, no explicit line spacings will be set.

You can also use following parameters in Java code:

*   AWExporterParameter.USE\_LINE\_SPACINGS\_NONE (0)
*   AWExporterParameter.USE\_LINE\_SPACINGS\_ALWAYS (1)
*   AWExporterParameter.USE\_LINE\_SPACINGS\_SMART (2)

**In JasperReports:**

```
 import com.aspose.words.jasperreports.*;

   AWDocExporter exporter = new AWDocExporter();
   exporter.setParameter(AWExporterParameter.USE_LINE_SPACINGS, AWExporterParameter. USE_LINE_SPACINGS_NONE);
   exporter.exportReport(); 
```

**In JasperServer:**

```
<bean id="aw_exportParameters" class="com.aspose.words.jasperreports.AWExportParametersBean">
    <property name="useLineSpacings" value="0"/>
</bean> 
```




[1]: http://www.aspose.com/downloads/words-family/jasperreports




