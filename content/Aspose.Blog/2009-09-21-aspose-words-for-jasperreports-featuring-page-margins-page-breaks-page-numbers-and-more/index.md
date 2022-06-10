---
title: 'Set Page Margins, Page Breaks, and Page Numbers in Word Documents in JasperReports'
date: Mon, 21 Sep 2009 23:25:00 +0000
draft: false
url: /2009/09/21/aspose-words-for-jasperreports-featuring-page-margins-page-breaks-page-numbers-and-more/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We have just released Aspose.Words for JasperReports 1.3.0. The new version includes a number of features that we hope you will find useful. Those are page margins, page breaks of different types, and the support for Microsoft Word fields that allows, for example, export page numbers that will be dynamically updated while the generated document is being edited.

Let's discuss all of the features in details.

## Page Margins

Unfortunately, at the moment the JasperReports print model does not allow exporters to detect page margins specified in the report design. Hence, Aspose.Words for JasperReports uses a special algorithm to work this around.

The algorithm works as follows. All page margins are set to a default value that is used by Microsoft Word when creating a new document (1 inch). If some report elements are located closer to page edges, then the corresponding page margins are reduced appropriately. That is, page margins are set to the value of 1in or less, depending on the report design.

You can change the default 1in value by specifying what page margins the exporter should try to enforce. Use the following parameter for that:

**JasperReports:**

```
import com.aspose.words.jasperreports.*;
AWDocExporter exporter = new AWDocExporter();
exporter.setParameter(AWExporterParameter.PAGE_MARGINS, “1in;1in;0.5in;0.5in”);
exporter.exportReport();
```

**JasperServer:**

```
<bean id=“aw_exportParameters“ class=“com.aspose.words.jasperreports.AWExportParametersBean“>
    <property name=“pageMargins“ value=“1in;1in;0.5in;0.5in”/>
</bean>
```

The value of the parameter is a string of the form

_"left\_margin;right\_margin;top\_margin;bottom\_margin"_,

where the following units of measure are allowed:

*   **in** - inches (default, may be omitted)
*   **cm** - centimetres
*   **mm** - millimetres
*   **px** - pixels
*   **pt** - points

Note you can use different units of measure in the same string or omit some of margin values.

## Page Breaks

Aspose.Words for JasperReports supports three ways page breaks are inserted between document pages:

*   Normal page breaks
*   Section breaks (i.e. one section per page – default mode)
*   No page breaks in the document at all

The "section breaks" mode is chosen as default because there may be the headers and footers throughout the document that contain different data. Microsoft Word requires different headers/footers should be placed in different sections.

You can change the page breaks inserted to regular (not section) breaks by using the following parameter:

**JasperReports:**

```
import com.aspose.words.jasperreports.*;
AWDocExporter exporter = new AWDocExporter();
exporter.setParameter(AWExporterParameter.PAGE_BREAKS, AWExporterParameter.PAGE_BREAKS_NORMAL);
exporter.exportReport();
```

**JasperServer:**

```
<bean id=“aw_exportParameters“ class=“com.aspose.words.jasperreports.AWExportParametersBean“>
    <property name=“pageBreaks“ value=“0”/>
</bean>
```

You can instruct the exporter to avoid any usage of page breaks (so that report contents are simply exported continuously) by using the following parameter:

**JasperReports:**

```
import com.aspose.words.jasperreports.*;
AWDocExporter exporter = new AWDocExporter();
exporter.setParameter(AWExporterParameter.PAGE_BREAKS, AWExporterParameter.PAGE_BREAKS_NONE);
exporter.exportReport();
```

**JasperServer:**

```
<bean id=“aw_exportParameters“ class=“com.aspose.words.jasperreports.AWExportParametersBean“>
    <property name=“pageBreaks“ value=“2”/>
</bean>
```

Note that in these modes, since the generated document consists of one section, only the first pair of header and footer will be exported.

## Inserting Fields

Aspose.Words for JasperReports provides a unique feature that allows inserting Microsoft Word fields to any point of the document. This can be used to insert page numbers that are dynamically updated as the document is being edited, TOC (table of contents), and many other things.

To enable field code recognition, use the following parameter:

**JasperReports:**

```
import com.aspose.words.jasperreports.*;
AWDocExporter exporter = new AWDocExporter();
exporter.setParameter(AWExporterParameter.RECOGNIZE_FIELDS, true);
exporter.exportReport();
```

**JasperServer:**

```
<bean id=“aw_exportParameters“ class=“com.aspose.words.jasperreports.AWExportParametersBean“>
    <property name=“recognizeFields“ value=“true”/>
</bean>
```

Once this parameter is set to true, the exporter treats any text enclosed in curve brackets ({}) as a field code and exports it appropriately. For example, the following text

_Page { PAGE } of { NUMPAGES }_,

will contain two fields in the produced document, PAGE and NUMPAGES, whose are calculated to the current page number and the total number of pages in the document, respectively.

You can add any field arguments and switches supported by the field. For example, to insert a timestamp of document creation, insert the following text:

_{ DOCPROPERTY CreateTime }_

To download Aspose.Words for JasperReports 1.3.0, please visit [https://downloads.aspose.com/words/jasperreports][1]




[1]: https://downloads.aspose.com/words/jasperreports




