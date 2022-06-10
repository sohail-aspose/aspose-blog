---
title: 'Field Update in Aspose.Words - The Killer Feature of 2009'
date: Sun, 13 Sep 2009 20:12:00 +0000
draft: false
url: /2009/09/13/field-update-in-aspose-words-the-killer-feature-of-2009/
author: Romank
summary: ''
tags: ['update date and time fields in Word doc', 'update formula fields in word document', 'update if and compare field in Word doc', 'update mail merge fields in word document']
categories: ['Aspose.Words Product Family']
---

# Overview

Aspose.Words for .NET 7.0 that will be released in the next few days include a new exciting feature: **Field Update**.

Fields in a document are like placeholders where some useful data can be inserted. For example, a field can be a page reference, formula or a mail merge field. A field in a Microsoft Word document consists of a field code and field result. The field code is an instruction about how the field result needs to be updated or calculated. An application that processes a document and encounters a field might have the functionality to interpret the instructions contained in the field code and update the field result with a new value. This is called field update.

Usually, a field, when inserted in Microsoft Word, already contains an up to date value. For example, if the field is a formula or a page number, it will contain a correct calculated value for the given version of the document. But if you have an application that generates or modifies a document with fields, for example, combines two documents or populates with data, then for the document to be useful, all fields should ideally be updated.

All applications that need to process Microsoft Word documents with fields face the task of supporting the fields. Having seen several solutions, I identify three main levels of support for fields:

*   Do not support all or some fields (skip, destroy during open/save)
*   Roundtrip (keep intact during open/save)
*   Fully support (roundtrip and update result when needed)

Fields in Microsoft Word documents are complex. There are over 50 field types (each needs its own result calculation procedure), formulas and expressions, bookmarks and references, functions and various switches. Fields can also be nested.

It is interesting to note that while the syntax and behavior of Microsoft Word fields is well documented (thanks to Office OpenXML), there is really no other software exists, except Microsoft Word itself, that can interpret and update all fields in Microsoft Word documents at level C.

Aspose.Words is a class library designed for server-side processing of Microsoft Word documents and the question of supporting fields is an important one. Aspose.Words earlier versions were standing at level B+. All fields in a document were preserved during open/save and conversions and it was possible to update results of some simple fields. Aspose.Words for .NET 7.0 with its new field update feature brings us much closer to level C.

# History of Fields in Aspose.Words

Since its first appearance at the end of 2003, Aspose.Words provided the ability to generate reports (populate documents with data) using the standard Microsoft Word mail merge fields.

The problem that we immediately noticed was that customers often already had template documents for mail merge and they contained complex expressions involving nested IF, MERGEFIELD, formulas and functions. Aspose.Words was only capable of processing the simple MERGEFIELD and NEXT fields, no nesting, no expressions. The customers had an ugly job of reworking their templates and we used to recommend “take the logic out of the document and put into the code”. We just could not offer anything else when the customers just wanted to start using Aspose.Words with existing templates.

Fast forward to end of 2009 and we’ve finally managed to find the time to do what you’ve been asking for so long.

Aspose.Words for .NET 7.0 includes what we call “Field Update Engine V1.0”. The main goal of this milestone is to support evaluation of the IF fields during mail merge. But we’ve done more than that, read on.

# Supported Fields

The calculation of the following fields is supported in Aspose.Words for .NET 7.0:

*   \= (formula field)
*   IF
*   COMPARE
*   DATE
*   TIME
*   MERGEFIELD
*   MERGEREC
*   MERGESEQ
*   NEXT
*   NEXTIF
*   DOCPROPERTY
*   DOCVARIABLE

There are also several fields that Aspose.Words can update, but they are calculated by the Layout Engine when Aspose.Words renders a document (converts to PDF, XPS, images or prints). These fields have been supported and have not changed with the release of this version; I just mention them for completeness:

*   PAGE
*   PAGES
*   PAGEREF
*   REF
*   SECTION
*   SECTIONS

# Sophisticated Parsing

Aspose.Words follows the way Microsoft Word processes fields and as a result it correctly handles:  

*   Nested fields  
    **IF { =OR({ COMPARE { =2.5 +PRODUCT(3,5 ,8.4) } > 4}, { =2/2 }) } = 1 "Credit not acceptable" "Credit acceptable"**

*   Spaces/no spaces, quotes/no quotes, escape characters in fields etc  
    **MERGEFIELD \\f"Text after""Field \\n\\ame with \\" and \\\\ and \\\*"\\bTextBefor\\e**

# \= (Formula) Fields

Aspose.Words now provides a very serious implementation of the formula engine and supports the following:  

*   Arithmetic and logical operators  
    **\=(54+4\*(6-77)-(5))+(-6-5)/4/5**

*   Functions  
    **\=ABS(-01.4)+2.645/(5.6^3.5)+776457 \\# "#,##0"**

*   References to bookmarks  
    **\=IF(C>4, 5,ABS(A)\*.76) +3.85**

*   Number formatting switches  
    **\=00000000 \\# "$#,##0.00;($#,##0.00)"**

The following functions in expressions are supported: ABS, AND, AVERAGE, COUNT, DEFINED, FALSE, IF, INT, MAX, MIN, MOD, NOT, OR, PRODUCT, ROUND, SIGN, SUM, TRUE.

# IF and COMPARE Fields

Just some of the IF expressions that Aspose.Words can easily calculate should give you an idea of how powerful this feature is:

*   **IF 3 > 5.7^4+MAX(4,3) True False**
*   **IF “abcd” > “abc” True False**
*   **IF “?ab\*” = “1abdsg” True False**
*   **IF 4 = “2\*2” True False**
*   **COMPARE 3+5/34 < 4.6/3/2**

# DATE and TIME Fields

Aspose.Words supports all date and time formatting switches available in Microsoft Word, some examples are:

*   **DATE  \\@ “d-MMM-yy”**
*   **DATE  \\@ “d/MM/yyyy h:mm am/pm”**

# Mail Merge Fields

It is fair to say that demand for field calculation in Aspose.Words was mostly driven by customers who use the Aspose.Words’ mail merge feature (a.k.a reporting).

Earlier versions of Aspose.Words only supported the basic usage of the MERGEFIELD and NEXT fields. Some advanced capabilities, not found in Microsoft Word’s mail merge, such as mail merge regions, inserting images and mail merge event handlers were also provided.

But many customers had template documents with various nested IF, MERGEFIELD and formulas and simply wanted an easy way to migrate from using Microsoft Word’s mail merge to Aspose.Words.

Aspose.Words for .NET 7.0 finally delivers this by providing an extensive implementation for fields that are most frequently encountered in mail merges.

There is now no limit to the complexity of mail merge fields in your documents. You can use IF, formulas, nest them and even calculate the merge field’s name using a formula.

Some examples of mail merge fields that Aspose.Words now supports:  

*   Mail merge field switches  
    **MERGEFIELD  FirstName \\\* FirstCap \\b "Mr. "**

*   Nested merge fields in a formula  
    **IF { MERGEFIELD Value1 } >= { MERGEFIELD Value2 } True False**

*   Calculate the name of the merge field at runtime  
    **MERGEFIELD { IF { MERGEFIELD Value1 } >= { MERGEFIELD Value2 } FirstName"LastName" }**

*   Conditional move to next record in the data source  
    **NEXTIF { MERGEFIELD Value1 } <= { =IF(-2.45 >= 6\*{ MERGEFIELD Value2 }, 2, -.45) }**

# How to Update Fields Programmatically in C#

The default behavior in Aspose.Words is to preserve fields in a document intact.

When you execute a mail merge, the all fields in the document will be automatically updated. This is because mail merge is, in fact, a case of a field update. The program encounters a mail merge field and needs to update its result, which involves grabbing the value from the data source and inserting it into the field. The logic is of course more complicated, for example, when reached the end of the document/mail merge region, but not the end of the data source, then duplicate the region and update the new set of fields.

To explicitly update fields in the whole document, simply call **Document.UpdateFields**.

To update fields contained in part of a document, obtain a **Range** object and call the **Range.UpdateFields** method. In Aspose.Words, you can obtain a **Range** for any node in the document tree, such as **Section**, **HeaderFooter**, **Paragraph** etc using the **Node.Range** property.

At the moment, using **UpdateFields** will not update fields that are related to the page layout algorithms (e.g. PAGE, PAGES, PAGEREF). The page layout-related fields are automatically updated when you render a document (save to PDF, XPS or print). You can explicitly update page layout-related fields by calling **Document.UpdatePageLayout**.  

# Format Switches

A field in a document can have formatting switches that specify how the resulting value should be formatted. Aspose.Words supports the following format switches:

*   \\@ – date and time formatting
*   \\# – number formatting
*   \\\* Caps
*   \\\* FirstCap
*   \\\* Lower
*   \\\* Upper
*   \\\* CHARFORMAT – format result according to the first character of the field code.
*   \\\* MERGEFORMAT – format result according to how the old result is formatted (limited support at the moment).

# Date and Number Formatting in Fields

When Aspose.Words calculates a field result, it often needs to parse a string into a number or date value and also to format it back to a string.

Aspose.Words always uses the current thread culture to perform parsing and formatting when calculating field values.

To control the culture used during field calculation, just set the **Thread.CurrentThread.CurrentCulture** property to a culture of your choice before invoking field calculation.

# Limitations

Here is a list of known limitations in the current version of the Aspose.Words field calculation engine:

*   Only the specified field types are calculated.
*   The \\\* MERGEFORMAT switch support is limited.
*   Update of fields that span across multiple sections is not supported.
*   References to values of cells in a table are not supported.
*   Range can represent only a node (with all its children) in a tree, not an arbitrary length of text.

# What’s Next

Now, when we’ve done the hardest part (implemented the field parsing and calculation engine), we will simply work to support calculation of all the remaining Microsoft Word document fields.  

In the next few releases expect to see exciting things like complete calculation of Table of Contents (TOC).








