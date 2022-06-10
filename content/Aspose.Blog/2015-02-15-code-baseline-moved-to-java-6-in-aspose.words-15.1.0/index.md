---
title: 'Code Baseline Moved to Java 6 in Aspose.Words 15.1.0'
date: Sun, 15 Feb 2015 09:21:06 +0000
draft: false
url: /2015/02/15/code-baseline-moved-to-java-6-in-aspose.words-15.1.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](https://blog.aspose.com/)[Aspose.Words for Java][1] 15.1.0 has been released. This month’s release contains over 81 useful new features, enhancements, and bug fixes to the Aspose.Words products.

You can download the latest release of Aspose.Words from the following link:

*   [Aspose.Words for Java 15.1.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Moved main codebase to Java 6 (Java 7 and 8 are also supported). Dropped support for Java 5 and 1.4
*   Fields Public API
*   New public API members for structured document tags
*   OpenDocument (ODT) import/export fidelity improvements
*   Rendering of spacing and kerning in WordArt supported
*   HTML export/import improved for better round-tripping
*   Comment numbering in rendering

## Code Baseline Moved to Java 6

### JDK Options

JDK 1.5 32-bit had been used as Aspose.Words Java baseline for long long time. Even JDK 1.4 version had been generated for users with ancient environment. Both JDKs are discontinued by Sun/Oracle. Even commercial (non-open) support of JDK 1.5 is dropped about year ago. Starting from January release 15.1 of Aspose.Words, we dropped support of Java 1.4 and 1.5.

Oracle currently supports jdk 1.6, 1.7 and 1.8. Open support of jdk 1.6 is closed about year ago, but commercial support is still here. There are also few environments (like not very last but still popular versions of Mac OS) that don’t support 1.7 and 1.8, they work on jdk 1.6 only.

### JDK 1.6-1.7-1.8 Small Differences.

Byte code of 1.6, 1.7 and 1.8 is very close. There is no global difference like in 1.4 vs 1.5 vs 1.6. Few language constructs are added in 1.7 and 1.8. Few libraries are updated/bug fixed. Few fonts are rendered differently. Few image formats are rendered differently too due to updated codecs. There are many hidden changes like JVM optimization.

As a result, we do not need in different JARs for JDK 1.6, 1.7, 1.8 as it was for JDK 1.4, 1.5 and 1.6. The single JDK 1.6 jar is enough for all current java versions.

### Code Baseline

The very last available Java JDK is 1.8 64-bit which is chosen for development and test baseline. This is becuause of two reasons: 1) it is faster than older versions, so tests and development will be slightly faster. 2) It is stricter than older versions so some bugs we can catch under 1.8 but the bugs don't show under 1.6. However, we use only 1.6 language options, language constructs added in 1.7 and 1.8 are not used. So we can compile 1.8 baseline to 1.6 production JAR for release publication.

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

## HtmlSaveOptions.ExportRoundtripInformation Property Added

We have now added a new public property HtmlSaveOptions.ExportRoundtripInformation:

This option allows to convert Word document to HTML format with round-trip information. Saving of the round-trip information allows to restore document properties such as tab stops, comments, headers and footers during the HTML documents loading back into a Document object.

## Spacing and Kerning in WordArt Objects is Supported

Aspose.Words now takes spacing and kerning in WordArt objects into account during rendering to fixed page formats such as PDF.




[1]: https://products.aspose.com/words/java
[2]: https://downloads.aspose.com/words/java




