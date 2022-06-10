---
title: 'ArisGlobal Uses Aspose.Words to Manipulate, Format and Save 100+ Word Documents'
date: Fri, 04 Jun 2010 12:28:05 +0000
draft: false
url: /2010/06/04/manipulate-format-and-save-100-word-documents-using-apis/
author: Gopal H R
summary: ''
tags: ['Aspose.Words', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About ArisGlobal



{{< figure align=center src="images/AG_Logo_RGB_042617_rs.png" alt="">}}


[ArisGlobal][1] aims to digitally transform drug development through simple, intelligent and unified technology. A pharmaceutical company is required to submit to the authorities on a regular basis a Periodic Safety Update Report (PSUR). The information required in this PSUR needs to be gathered from different locations in the company (Safety, Regulatory, Medical Information, Medical Affairs, Sales and Marketing). Information can come from other departments within the organization. This information might come through Word or PDF documents so the applications should be able to upload these types of documents and insert them into the PSUR which is being generated. Collecting, formatting as well as analyzing the information included in this PSUR and including a conclusion on the safety of the product is time-consuming and labor-intensive especially in paper format. Additionally, signing off approval copies on various sections and the whole document for global PSURs is a logistical difficulty placing greater pressure on timeline submissions.

The proposed application will not fully automate the generation of the PSUR as a lot of the work relates to the interpretation of the information and preparing the correct conclusions. However, a lot of the formatting, processing, and collection of the information required for the PSUR can as such reduce the time required to prepare this PSUR.

## Problem

A template will be created with different sections and each section will have many bookmarks and the same will be uploaded into the application. All the sections in the template are displayed as a tree structure in the UI.

Based on the section selected in the tree the respective section bookmarks will be displayed to the user. For each bookmark in the section, the user has an option to insert a file data or write an SQL query to load the data from the database. The key options in the application are as following

*   Inserting query data in tabular format at bookmark location
*   Inserting Query data as a text at bookmark location
*   Inserting file data like Text, Microsoft Word at bookmark location.
*   Merging of documents and building one single report.

Once data is inserted into the bookmark location, the final report will be built by updating TOC (table of contents), TOF (table of figures), TOT (table of tables), Appendix data, etc.

## Solution

agComposer is an application that is tightly integrated with Microsoft Word, We need to do a lot of Word manipulations from the application. Following is the current usage of [Aspose.Words][2]’ API within our application:

*   Listing all the bookmarks from the section document in the UI.
*   Creating tables and inserting data fetched from database / SQL queries.
*   Importing external word document into an application generated Report.
*   Merging more than one document into a single report, which may be of thousands of pages.

agComposer has several ~100+ documents and templates and the content of these documents is dynamically populated and loaded into the Aspose document. Using Aspose API’s these documents are manipulated, formatted and saved.

### Listing of Bookmarks from a Document



{{< figure align=center src="images/arisglobal-case-study-aspose-words.png" alt="" caption="The output of bookmarks read from a section &amp; displaying.">}}


## Benefits

The primary benefit we observed is minimal memory utilization for processing. The features provided for Microsoft Word manipulation are very good and the tools support very large documents with respect to size. These are the key benefits we have using Aspose.Words:

*   Fast development integration.
*   Platform independent.
*   Very good technical support.
*   Support for multiple versions of the Microsoft Office suite.

## Next Steps

Planning to design new reports using Aspose tools for [JasperReports][3] and call those reports from the application and insert the output into the report. We are planning to use [Aspose.PDF][4] to convert Word reports into PDF format.

## Summary

Overall satisfied with the product and technical support. A very good tool to manipulate word documents using Java application & able to handle most of the features of the word through APIs of [Aspose.Words][5]. We are looking forward to using other [Aspose products][6] in the near future.

**Gopal H R  
**Arisglobal Software Pvt. Ltd.




[1]: https://www.arisglobal.com/company-details/
[2]: https://products.aspose.com/words
[3]: https://products.aspose.com/total/jasperreports
[4]: https://products.aspose.com/pdf
[5]: https://products.aspose.com/words/family
[6]: https://products.aspose.com/




