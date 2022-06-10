---
title: 'Fields Public API, new Members Added to Structured Document Tags, OpenDocument and HTML Import Export Fidelity Improvements in Aspose.Words 15.1.0'
date: Wed, 11 Feb 2015 16:57:00 +0000
draft: false
url: /2015/02/11/fields-public-api-new-members-added-to-structured-document-tags-opendocument-and-html-import-export-fidelity-improvements-in-aspose.words-15.1.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words for .NET 15.1.0 has been released. This month’s release contains over 75 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest release of Aspose.Words from the following link:

*   [Aspose.Words for .NET 15.1.0][1]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Fields Public API
*   New public API members for structured document tags
*   OpenDocument (ODT) import/export fidelity improvements
*   Rendering of spacing and kerning in WordArt supported
*   HTML export/import improved for better round-tripping
*   Comment numbering in rendering

## HtmlSaveOptions.ExportRoundtripInformation Property Added

We have now added a new public property HtmlSaveOptions.ExportRoundtripInformation:

```
 /// <summary>
/// Specifies whether to write the roundtrip information when saving to HTML, MHTML or EPUB.
/// Default value is <c>true</c> for HTML and <c>false</c> for MHTML and EPUB.
/// </summary>
/// <remarks>
/// Saving of the roundtrip information allows to restore document properties such as tab stops,
/// comments, headers and footers during the HTML documents loading back into a <see cref="Document"/>object.
/// When <c>true</c>, the roundtrip information is exported as -aw-* CSS properties
/// of the corresponding HTML elements.
/// When <c>false</c>, causes no roundtrip information to be output into produced files.
/// </remarks>
public bool ExportRoundtripInformation
{
    get { return mExportRoundtripInformation; }
    set { mExportRoundtripInformation = value; }
} 
```

This option allows to convert Word document to HTML format with round-trip information. Saving of the round-trip information allows to restore document properties such as tab stops, comments, headers and footers during the HTML documents loading back into a Document object.

## Spacing and Kerning in WordArt Objects is Supported

Aspose.Words now takes spacing and kerning in WordArt objects into account during rendering to fixed page formats such as PDF.

## Public API for SDT Checkbox

We have now opened programmatic access to Checked/Unchecked state of SDT (StructuredDocumentTag) Checkbox through StructuredDocumentTag.Checked property. We have also added capability to create StructuredDocumentTag of type SdtType.Checkbox in the public API.

We have added a couple of usage examples in documentation. Please check out "shows how to set the current state of check box" and "shows how to create content control of type check box" examples in documentation.

## Public Fields API v1.0 Announced

We are proud to announce public fields API v1.0 that will be exposed starting from 15.1 release of Aspose.Words. Initially, we have added the following new classes and properties to this API:

### Field Classes and Properties

All FieldXXX classes are now public. Each class corresponds to a certain MS Word field type and provides a number of properties corresponding to arguments, switches and switch arguments of that field. All field types and arguments/switches listed in the specification (except the newest ones appeared in MS Word 2013) are covered that makes it a unique solution on the market.

We have introduced two property types i.e. boolean for stand-alone switches and string for arguments and arguments of switches. In defense of this approach, we can adduce the following: if we treat UI of MS Word as a visual analogue of its API, the field insertion dialog also provides checkboxes for simple switches and textboxes (without any format verification) for the rest. The following rules apply when setting field properties:

*   A string property is null when the corresponding argument (or a switch with argument) is missing. A boolean property is true or false depending on whether the corresponding switch is present/absent.
*   The engine automatically inserts empty strings if a property affects, say, the third argument and the previous two are missing.
*   The engine automatically detects if an argument should be enclosed in double quotes (e.g. it contains whitespace). A user should explicitly define a double quote in a string being assigned only if it is a part of the string.

### FieldFormat class

We have also exposed access to field format switches common for all field types via the Field.Format, Field.Format.NumericFormat, Field.Format.DateTimeFormat, and Field.Format.GeneralFormats properties. The user is now able to read or modify field format.

### New Overload of DocumentBuilder.InsertField Method Added

We have introduced the new overload DocumentBuilder.InsertField(FieldType fieldType, bool updateField) which allows to insert a field by its type.

### New Paragraph.AppendField Method Added

We have introduced three overloads of the Paragraph.AppendField() method, each corresponding to a DocumentBuilder.InsertField() method with similar signatures. This is basically to address WORDSNET-3225 (Make it possible to create Fields using DOM (without using DocumentBuilder)). We hope, this will meet the requirement where customers ask for the capability of inserting a field without document builder. Since Field is a facade that bunches up three document nodes (which have other nodes in between), all we managed to come up with is the Paragraph.AppendField() method that enables to avoid the use of DocumentBuilder but basically just duplicates its field insertion functionality. Therefore, we are closing this issue for now, but the customers are welcome to suggest how they would like to see this feature implemented, unless they are satisfied with the aforementioned one. We will consider they suggestions for implementation then.

### New FieldToc.UpdatePageNumbers Method Added

We have added the FieldToc.UpdatePageNumbers() method. Since the FieldToc class, like other field classes, were initially internal, we had to wait until the rest of public fields API is ready.

### Usage Examples

You can find usage examples for this new Public Fields API in Aspose.Words documentation page: Inserting Fields using DOM.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx




