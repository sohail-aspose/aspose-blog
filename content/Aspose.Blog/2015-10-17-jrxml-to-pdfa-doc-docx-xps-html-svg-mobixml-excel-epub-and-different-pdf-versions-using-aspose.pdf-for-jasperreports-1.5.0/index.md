---
title: 'JRXML to PDF/A, DOC, DOCX, XPS, HTML, SVG, MobiXML, Excel, ePUB and different PDF versions using Aspose.Pdf for JasperReports 1.5.0'
date: Sat, 17 Oct 2015 20:07:06 +0000
draft: false
url: /2015/10/17/jrxml-to-pdfa-doc-docx-xps-html-svg-mobixml-excel-epub-and-different-pdf-versions-using-aspose.pdf-for-jasperreports-1.5.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Convert JasperReport JRXML to DOC', 'Convert JasperReport JRXML to Excel', 'Convert JasperReport JRXML to HTML', 'Convert JasperReport JRXML to PDF', 'Convert JasperReport JRXML to SVG', 'Convert JasperReport JRXML to XPS', 'PDF API for JasperReports']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-JasperReports_100.png" alt="JRXML to PDF, DOC, Excel, SVG">}}


A new release with some new features has hit the download section. Likewise every release, we always strive to introduce auspicious features which help our customers to fulfill their requirements. So we are pleased to announce the release of [Aspose.PDF for JasperReports 1.5.0][1] in which we have introduced inter file format conversion features. So now you get the option to transform JRXML file to PDF as well as various other file formats (which are already supported in Aspose.Pdf for Java).

## Convert JRXML to Other File Formats

In this new release, we have implemented some new classes and methods to support conversion of .JRXML file to various other file formats. The following changes have been introduced.

*   Implemented classes: **SavingFormatType** and **PdfFormatType**

**Implemented methods in the class JrPdfExporter:**

*   public void setPdfFormat(int format)/PdfFormatType/
*   public int getPdfFormat()
*   public void setSavingFormat(int type)/SavingFormatType/
*   public int getSavingFormat()

Following are the details regarding newly implemented feature to save the report in the non-pdf file format. For this purpose, we have implemented methods in the class **com.aspose.pdf.jr.jasperreports.JrPdfExporter:**

*   public void setSavingFormat(int type) //SavingFormatType constant
*   public int getSavingFormat()

We also have Implemented a class: **com.aspose.pdf.jr.PdfFormatType** With specified below constants:

*   PDF
*   DOC
*   XPS
*   HTML
*   DOCX
*   SVG
*   MOBIXML
*   EXCEL
*   EPUB

Code Snippet:

```
 JasperReport jasperReport = JasperCompileManager
    .compileReport("input.jrxml");
JasperPrint jasperPrint = JasperFillManager.fillReport(jasperReport,
            new HashMap(), new JREmptyDataSource(10));

JrPdfExporter exporter = new JrPdfExporter();
exporter.setParameter(PdfExporterParameter.JASPER_PRINT, jasperPrint);
String fileName = "output_Pdf_A.pdf";
exporter.setParameter(PdfExporterParameter.OUTPUT_FILE_NAME, fileName);

JrPdfExportParametersBean exportParameters = new JrPdfExportParametersBean();

exportParameters.setPdfAMode(true);
//configure the result file format type
exporter.setSavingFormat(SavingFormatType.DOC);

exportParameters.setSecuredMode(false);

exportParameters.setLicenseFile("Aspose.Pdf.JasperReports.lic");
exporter.setParameter(PdfExporterParameter.LICENSE,
            exportParameters.getAsposePdfLicenseMap());

exporter.exportReport(); 
```

## Convert Report to Specific PDF Format

We have implemented different features to save the report in the specific PDF format. Therefore we have implemented methods in the class **com.aspose.pdf.jr.jasperreports.JrPdfExporter:**

*   public void setPdfFormat(int format)//PdfFormatType constant
*   public int getPdfFormat()

Implemented class: **com.aspose.pdf.jr.PdfFormatType** with following constants.

*   PDF\_A\_1A
*   PDF\_A\_1B
*   PDF\_A\_2A
*   PDF\_A\_3A
*   PDF\_A\_2B
*   PDF\_A\_3B
*   v\_1\_3
*   v\_1\_4
*   v\_1\_5
*   v\_1\_6
*   v\_1\_7
*   PDF\_X\_1A
*   PDF\_X\_3
*   DEFAULT

code snippet.

```
 JasperReport jasperReport = JasperCompileManager
                .compileReport("input.jrxml");
JasperPrint jasperPrint = JasperFillManager.fillReport(jasperReport,
            new HashMap(), new JREmptyDataSource(10));

JrPdfExporter exporter = new JrPdfExporter();
exporter.setParameter(PdfExporterParameter.JASPER_PRINT, jasperPrint);
String fileName = "output_Pdf_A.pdf";
exporter.setParameter(PdfExporterParameter.OUTPUT_FILE_NAME, fileName);

JrPdfExportParametersBean exportParameters = new JrPdfExportParametersBean();

exportParameters.setPdfAMode(true);
//configure the result pdf format type
exporter.setPdfFormat(PdfFormatType.PDF_A_1A);

exportParameters.setSecuredMode(false);

exportParameters.setLicenseFile("Aspose.Pdf.JasperReports.lic");
exporter.setParameter(PdfExporterParameter.LICENSE,
            exportParameters.getAsposePdfLicenseMap());

exporter.exportReport(); 
```

## Synchronization with JasperReports-6.1.0

This new release is synchronized with latest JasperReport version 6.1.0 and earlier versions. For compatibility with new versions of JasperReports, we have created a new package named com.aspose.pdf.jr6\_1\_0. However the name of the package must be considered when setting up the connection library in Jasperreport-Server in files applicationContext.xml and viewReportBeans.xml. So for each JasperReports version, we have specific product binaries.

*   aspose.pdf.jasperreports.jr3.1-1.5.0.jar
*   aspose.pdf.jasperreports.jr3.7-1.5.0.jar
*   aspose.pdf.jasperreports.jr4.5-1.5.0.jar
*   aspose.pdf.jasperreports.jr5.5-1.5.0.jar
*   aspose.pdf.jasperreports.jr5.6-1.5.0.jar
*   aspose.pdf.jasperreports.jr6.1-1.5.0.jar

Aspose.Pdf for JasperReports offers exciting report features such as tables, charts and images and enables you to export reports from JasperReports and JasperServer to Portable Document Format (PDF). In this release, there have been other fixes related to component and we recommend you to please download and start exploring the exciting new release of [Aspose.PDF for JasperReports 1.5.0][2].




[1]: https://downloads.aspose.com/pdf/jassperreport
[2]: https://downloads.aspose.com/pdf/jassperreport




