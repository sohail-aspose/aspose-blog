---
title: 'Series: Aspose.Words Feature Overview, Part 3: Support for the DOCX Format'
date: Fri, 13 Jul 2007 03:25:00 +0000
draft: false
url: /2007/07/13/series-aspose-words-feature-overview-part-3-support-for-the-docx-format/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

This is the 3rd post in the series. Previous post see here.

#### Microsoft Office Open XML (DOCX)

###### Office Open XML Overview

[Office Open XML][1] is the new XML-based format introduced in Microsoft Office 2007 applications. Office Open XML is a container format for several specialized XML-based markup languages. WordprocessingML is the markup language used by Microsoft Office Word 2007 to store its documents.

Note that WordprocessingML defined in Office Open XML is different from the [Microsoft Word 2003 XML][2] format, but they both are called WordprocessingML. The fact that the two formats have exactly the same name, but mean different things is confusing. To avoid confusion, in this documentation, we will refer to the new WordprocessingML format as Office Open XML or DOCX. We will call the old format WordprocessingML or WordML.

###### Office Open XML in Aspose.Words

Currently, Aspose.Words does not support Office Open XML, but we are working on it. First, DOCX export will be released (Q3 2007), followed by DOCX import (Q1 2008) in Aspose.Words for .NET. After that, exactly the same functionality will become available in Aspose.Words for Java.

As with other Microsoft Word document formats, Aspose.Words will provide extensive support for DOCX features. Such all-embracing implementation is possible because Aspose.Words was designed with the structure of Microsoft Word documents in mind.

###### DOCX is Open, Why Use Aspose.Words?

Being XML-based, Office Open XML is heralded as an enabling technology. It is true, Office Open XML makes it possible to build document processing and generating applications using just the XML classes without relying on third-party libraries such as Aspose.Words.

However, we strongly believe it is still very beneficial to use Aspose.Words when you have to deal with DOCX documents, rather than work through XML or other libraries.

The DOCX specification is several thousand pages long. Being open and standard does not mean being simple. To correctly process or generate DOCX documents one must invest in learning the format well.

In addition to making it simpler to correctly process and generate valid documents, Aspose.Words provides the following important features you wouldn’t have when working with DOCX files directly via XML or other third-party libraries:

· High-quality conversions between many document formats (DOC, RTF, WordML, HTML, PDF).

· Ability to build documents from fragments from one or multiple documents, while automatically merging per-document structures such as styles and lists.

· Access to flat Range-like operations such as find and replace, get/set text of a bookmark, form field, document field or a node.

Consider the following example. It is a simple paragraph that contains text “Hello World” and the word “Hello” is bold. Now imagine you need to write a program that will search for all “Hello World” phrases in the document and replace them with “Goodbye Earth”.

What started out is a seemingly simple task of loading, modifying and saving an XML file does not look so simple anymore. In fact, it has become very complex. It takes a non-trivial algorithm to find and replace flat text across an XML tree. Have you ever wondered why standard XML classes such as XmlDocument do not offer find and replace functionality.

<w:p w:rsidR\="**00C07F31**" w:rsidRDefault\="**003F6D7A**">

<w:r w:rsidRPr\="**003F6D7A**">

<w:rPr\>

<w:b />

</w:rPr\>

<w:t\>**Hello**</w:t\>

</w:r\>

<w:r\>

<w:t xml:space\="**preserve**">**World.**</w:t\>

</w:r\>

</w:p\>

**A fragment of an Open Office XML document.**

Implementing even a simple find and replace operation over an Open Office XML document yourself is far from easy. It might be that your boss will enjoy you coding this yourself, bit it might be she will not. Our advice: remember that open and standard does not mean simple and use Aspose.Words.




[1]: http://en.wikipedia.org/wiki/Office_Open_XML
[2]: http://en.wikipedia.org/wiki/Microsoft_Office_2003_XML_formats




