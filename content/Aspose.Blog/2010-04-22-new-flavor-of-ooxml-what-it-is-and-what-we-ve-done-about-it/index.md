---
title: 'New flavor of OOXML: what it is and what we’ve done about it'
date: Thu, 22 Apr 2010 08:00:00 +0000
draft: false
url: /2010/04/22/new-flavor-of-ooxml-what-it-is-and-what-we-ve-done-about-it/
author: Dvdarkin
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Not so long ago International Organization for Standardization has accepted newer OOXML standard ISO/IEC 29500:2008 (supported by MS Word 2010) that became an extension of the older ECMA-376:2006 standard (supported by MS Word 2007). 

Now we're happy to confirm that Aspose.Words for .NET 9.0 supports ISO/IEC 29500:2008 Transitional. The implementation contains some limitations which should not affect your document workflow but if you think they do please let us know. Read on for more details.

# Strict vs. Transitional

The main question is how the older OOXML spec differs from the new one. The answer lies in two spec subsets: Transitional and Strict. In Transitional subset the new features are added only (except a few minor removals) and all the older stuff is valid too. The Strict subset not only adds features but also removes older features from OOXML. For example all VML schemas are removed. So we can regard the Strict as Transitional minus some ECMA-376:2006 features.

# The new stuff

A quick look over new features of ISO/IEC 29500:2008 can yield us several areas in which new stuff can be categorized. These areas should be regarded as coarse view but not a formal and strict description of all the changes (which are defined in the spec as annexes anyway).

· **New data schemas for older elements**. This category includes more flexible or more intuitive ways to write data. Per new spec data involving twips (twentieth of a point) or half points now can be specified using cm/mm/inch/pica/point units. Some values stored as bit flags within integer can now be written as true/false values. Percentage values can be written with % sign. Some data types include new enum values.

· **Additional information provided for existing elements.**  Tables now can contain description and caption and also header elements/information linking cells to their headers. Additional info is provided for linked and embedded objects through new elements objectEmbed and objectLink.

· **Elaborated support for RTL/LTR languages**. A number of additions improve Right-To-Left (RTL) and Left-To-Right (LTR) languages area. New elements such as dir, bdo are added. Elements start and end now carry semantics of older left and right.

· **New document settings**. Some new elements added to document settings and web settings including custom compatibility settings.

# What’s implemented

Aspose.Words 9.0 supports reading and writing ISO/IEC 29500:2008 Transitional conformant documents, including the majority of almost 80 additions or enhancements introduced. Our approach to implementing features was to look how MS Word 2010 Beta supported these. If feature was quite complex and MS Word didn’t provide functionality to use it, we put it on the “to be supported later” list. 

The list of “to be supported later” features includes:

· RTL/LTR elements bdo and dir;

· Table header/headers elements;

· Custom pictures for page borders;

· Custom number format for list numbering levels;

· Additional properties for linked/embedded objects.

As usual we’re open to your questions/comments and feature requests, so please let us know what you think.








