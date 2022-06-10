---
title: 'Support for New Mail Merge Syntax in Aspose.Words 11.2.0'
date: Tue, 03 Apr 2012 12:53:46 +0000
draft: false
url: /2012/04/03/support-for-new-mail-merge-syntax-in-.net-and-java-word-processing-api/
author: Adam Skelton
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="">}}


This month’s release of Aspose.Words 11.2.0 comes with a massive 150 fixes and new features. We’ve been hard at work on all areas of Aspose.Words and the list of new features speak for itself.  For a full list of features and fixes head over to the downloads page and download Aspose.Words 11.2.0:

*   [Aspose.Words for .NET 11.2.0][1]
*   [Aspose.Words for Java 11.2.0][2]

Here’s a closer look at some of the bigger features in this month’s release:

## Performance Enhancements

This particular improvement started as a fix to speed up the conversion of large documents consisting of only a single section, however, we did not stop there,  we went on to make numerous speed improvements in other parts of Aspose.Words.

The latest release can now see up to 50% conversion speed improvements during document conversion. We are pleased with these performance improvements.

## Supported Features Lists for both Import and Export Now Available for All Formats

Aspose.Words is built primarily to work with Microsoft Word documents. These formats are complex and contain numerous numbers of features. Aspose.Words is renowned for its high level of support for Word document features and now we have the lists to prove it.

These lists which are available for both .NET and Java, describe the support for the most common features that you, the customer, look for during conversion of documents from one format to another. It describes any limitations (if there are any) during conversion either due to the document format not supporting the particular feature or any limitations to do with Aspose.Words.

You can find the full lists in our online documentation section:

*   [What Document Features are Supported in Aspose.Words for .NET][3]
*   [What Document Features are Supported in Aspose.Words for Java][4]

Here’s a look at the supported features section in the documentation:



{{< figure align=center src="images/Import-and-Export-Formats.jpg" alt="">}}


## Detailed Descriptions and Helpful Links for Each Feature

Not only do we describe the current level of support for each feature, but we also go one further and provide you with the helpful information in the form of an overview and tips for each feature.

You will find that most features on the import pages come with detailed information about how the feature is imported into Aspose.Words and how it is represented in the Aspose.Words Document Object Model. We also provide handy hyperlinks for features in the documentation for further reading. This allows you to gain more information on the features you are interested in.

## Find out what HTML Tag Corresponds to What Document Feature

We are often asked what HTML tags are loaded as what document features. We have listened and understand that users who work with HTML formats often want extra information such as this.

We now provide a list of what tags are loaded during HTML import and what feature they correspond to. There is also a list which describes the HTML tags that are written for a particular document feature during export to HTML. We have made these lists as accurate as possible and are continually improving them.

Stay tuned to see further improvements to these pages as we add further information and restructure some parts to make it even easier to use.

## Introduction of the “Mustache” Template Syntax for Mail Merge

This new syntax allows you to create templates for use with mail merge that use plain text markers instead of merge fields. These markers look like this:_{{FieldName}}_

You can enable mail merging into plain text fields by enabling the **MailMerge.UseNonMergeFields** property and can freely mix them in your template with the Microsoft Word fields such as IF or Formula fields.

There is also some additional syntax you can use with these new fields:

### Object.Attribute

You can now easily merge attributes of a field using the following syntax

_{{Address.Street}}_

This will merge the **street** name from an **address** when you have XML which looks like this:

_<Order> // <-- Current context is here. <Number>23</Number> <Address> <Street>Nelson Street</Street> <Suburb>Howick</Suburb> <City>Auckland</City> </Address> <PhoneNumber>543 1234</PhoneNumber> </Order>_

Note that the notation works for regular merge fields as well, simply structure the merge field name in the same way, for example “_MERGEFIELD Address.Street_”.

### Foreach Blocks

You can merge data from multiple records using the foreach tag. This is similar to mail merge regions with conventional merge fields. You can also nest foreach blocks just like nested mail merge.

_{{#foreach Order}} {{Number}} {{Address.Street}} {{#foreach Item}} {{Description}} {{Cost}} {{Total}} {{/foreach Item}} {{/foreach Order}}_




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: http://docs.aspose.com/display/wordsnet/What+Document+Features+are+Supported
[4]: http://docs.aspose.com/display/wordsjava/What+Document+Features+are+Supported




