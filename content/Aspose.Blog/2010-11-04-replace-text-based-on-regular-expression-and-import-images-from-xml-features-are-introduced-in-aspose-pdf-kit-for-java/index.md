---
title: 'Replace Text Based on Regular Expression and Import Images From XML Features are Introduced in Aspose.Pdf.Kit for Java.'
date: Thu, 04 Nov 2010 00:14:00 +0000
draft: false
url: /2010/11/04/replace-text-based-on-regular-expression-and-import-images-from-xml-features-are-introduced-in-aspose-pdf-kit-for-java/
author: Shahzad Latif
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

We have released a new version of Aspose.Pdf.Kit for Java with some new features and fixes. In Aspose.Pdf.Kit for Java 3.5.0, we have introduced a new feature to replace text based on the regular expression. If the criteria specified in the regular expression is met, the first instance of the text will be replaced. In order to replace a string like 09.11.2010, you can use the following regular expression: "\\\\d{2}\\\\.\\\\d{2}\\\\.\\\\d{4}"; whereas, a string like 2034-3490-8 can be replaced using "\\\\d{4}-\\\\d{4}-\\\\d{1}". You also need to set the regular expression mode using setRegularExpressionUsed method. The following code snippet can help you understand this new feature:  
  

  
//create an object of PdfContentEditor class  
  
PdfContentEditor contentEditor = new PdfContentEditor();  
  
//bind input PDF file  
  
contentEditor.bindPdf("input.pdf");  
  
//set regular expression mode  
  
contentEditor.getReplaceTextStrategy().setRegularExpressionUsed(true);  
  
//replace string which satisfies to regular expression  
  
contentEditor.replaceText("\\\\d{2}\\\\.\\\\d{2}\\\\.\\\\d{4}", "New text");  
  
//save the output file  
  
contentEditor.save("output.pdf");  
  
contentEditor.close();  
  
  

This version also allows you to import the images from XML file. You only need to specify a valid path to the image file along with other field values; following is a short example of the XML containing path to an image file:  
  
<?xml version="1.0" encoding="utf-8"?>  
  
<fields>  
  
<field name="Telephone">  
<value>888.277.6734</value>  
</field>  
  
<field name="Name">  
<value>Mike</value>  
</field>  
  
<field name="Lodging">  
<value>Off</value>  
</field>  
  
<field name="Gender">  
<value>Male</value>  
</field>  
  
<field name="Photo">  
<value>c:\\files\\butterfly.jpg</value>  
</field>  
  
</fields>  
  
  
You can simply import the image file along with other data using the following code snippet:  
  

  
//create a Form object  
  
Form pdfForm = new Form("input.pdf", "output.pdf");  
  
//create input stream for XML  
  
FileInputStream inStream = new FileInputStream("data.xml");  
  
//import data to the PDF form  
  
pdfForm.importXml(inStream);  
  
//close input stream and Form object  
  
inStream.close();  
  
pdfForm.close();  
  

  
In addition to the above two features, we have improved file encryption, viewer preference, replace text and Form related issues. You can see the complete list of changes and download the latest version from the [Aspose.Pdf.Kit for Java download section][1].




[1]: http://www.aspose.com/community/files/72/java-components/aspose.pdf.kit-for-java/default.aspx




