---
title: 'Aspose.PDF Supports Custom Fonts and Compatibility with Latest JasperReports'
date: Thu, 08 Jan 2015 13:07:51 +0000
draft: false
url: /2015/01/08/aspose.pdf-supports-custom-fonts-and-compatibility-with-latest-jasperreports/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-JasperReports_100.png" alt="Aspose.Pdf for SSRS icon">}}


We are very much excited to announce the release of [Aspose.PDF for JasperReports 1.4.0][1] which provides the capability to use custom fonts when exporting JasperReports to PDF format. In order to use custom fonts, we added the setTruetypeFontDirectoryPath(String) method to the JrPdfExporter class which is used to specify the path of the folder where custom fonts are placed. In order to access an appropriate font, the correct font name should be provided, and in order to use Bold/Italic/BoldItalic variant of these fonts, the respective font must be present. For example, for the font "Consolas" it is consola.ttf, consolab.ttf, consolai.ttf, consolaz.ttf.

```
JrPdfExporter exporter = new JrPdfExporter();
exporter.setTruetypeFontDirectoryPath("../LocalFonts/");
```

The font can be configured in \*.jrxml file as < font fontName="Consolas"> or can be replaced by using fontMap:

```
JrPdfExporter exporter = new JrPdfExporter();
HashMap fontMap = new HashMap();
fontMap.put("SansSerif", "Consolas");
fontMap.put("serif", "Times New Roman");
fontMap.put("monospaced", "Courier");
exporter.setFontsMap(fontMap);
exporter.setTruetypeFontDirectoryPath("../LocalFonts/");
```

## Synchronization with JasperReports-5.6.0

The latest release is synchronized with the latest JasperReport version 5.6.0 and JasperReports v.5.6.1. For compatibility with new versions of JasperReports, we have created a new package named com.aspose.pdf.jr5\_6\_0. However, the name of the package must be considered when setting up the connection library in Jasperreport-Server in files applicationContext.xml and viewReportBeans.xml.

Aspose.PDF for JasperReports offers exciting report features such as tables, charts, and images and enables you to export reports from JasperReports and JasperServer to Portable Document Format (PDF). In this release, there have been other fixes related to component and we recommend you to please download and start exploring the exciting new release of [Aspose.Pdf for JasperReports 1.4.0][2].




[1]: https://downloads.aspose.com/pdf/jassperreport
[2]: https://downloads.aspose.com/pdf/jassperreport




