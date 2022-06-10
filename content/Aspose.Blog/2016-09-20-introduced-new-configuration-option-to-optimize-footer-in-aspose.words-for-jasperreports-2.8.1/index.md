---
title: 'Introduced New Configuration Option to Optimize Footer in Aspose.Words for JasperReports 2.8.1'
date: Tue, 20 Sep 2016 12:22:19 +0000
draft: false
url: /2016/09/20/introduced-new-configuration-option-to-optimize-footer-in-aspose.words-for-jasperreports-2.8.1/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/jasperreports/word-component.aspx)We are pleased to announce a new release of Aspose.Words for JasperReports that includes new configuration option to optimize footer distance. You can download the latest release of Aspose.Words for JasperReports from the following link:

[Download Aspose.Words for JasperReports 2.8.1][1]

Starting from release **1.9.0** there are several versions of jar library (necessary for better support of older versions of JasperReports). These include:

*   for JasperReports 6.3.0 and higher (**aspose.words.jasperreports-6.3.0.jar**)
*   for JasperReports 5.6.0 ... 6.2.0 (**aspose.words.jasperreports-6.2.0.jar**)
*   for JasperReports 4.7.0 ... 5.5.0 (**aspose.words.jasperreports-5.5.0.jar**)
*   for JasperReports 3.7.2 ... 4.5.0 (**aspose.words.jasperreports-4.5.0.jar**)
*   for JasperReports 3.7.1 and lower (**aspose.words.jasperreports-3.7.1.jar**)

Please copy **only one** jar library according to the version of installed JasperReports.

## Bug Fixes and Features

*   WORDSJSP-188 (Introduce new config option for footer optimization distance)

Optimize Footers

By default, Aspose.Word for JasperReports tries to optimize footer contents for better fitting footer on the page. This optimization takes place when a bottom-most page element is too low on page by a) decreasing font size of last paragraph break of the footer and b) decreasing footer distance. If you do not like the view of footers, you can disable this footers optimization by setting **OPTIMIZE\_FOOTERS** parameter to **false**.

**In JasperReports:**

```
 import com.aspose.words.jasperreports.*;

   AWDocExporter exporter = new AWDocExporter();
   exporter.setParameter(AWExporterParameter.OPTIMIZE_FOOTERS, false);
   exporter.exportReport(); 
```

**In JasperServer:**

```
<bean id="aw_exportParameters" class="com.aspose.words.jasperreports.AWExportParametersBean">
    <property name="optimizeFooters" value="false"/>
</bean> 
```

You can also set explicit minimal distance between bottom-most element and bottom page margin. This is controlled by **OPTIMIZE\_FOOTER\_DISTANCE** parameter. By default, its value is **12.0**. However, you can set any value between **12.0** and **36.0**. Therefore, if the distance between bottom margin of the bottom-most element and page bottom margin is less or equal to this parameter value – then footer is optimized, otherwise nothing happens.

**In JasperReports:**

```
 import com.aspose.words.jasperreports.*;

   AWDocExporter exporter = new AWDocExporter();
   exporter.setParameter(AWExporterParameter.OPTIMIZE_FOOTER_DISTANCE, 16);
   exporter.exportReport(); 
```

**In JasperServer:**

```
<bean id="aw_exportParameters" class="com.aspose.words.jasperreports.AWExportParametersBean">
    <property name="optimizeFooterDistance" value="16"/>
</bean> 
```




[1]: http://www.aspose.com/downloads/words-family/jasperreports




