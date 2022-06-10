---
title: 'Write Metadata and Formulas in MS Project Files using C# and Java'
date: Mon, 26 Aug 2019 08:38:43 +0000
draft: false
url: /2019/08/26/metadata-and-formulas-writing-support-in-aspose.tasks/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

[![aspose-tasks-for-net][1]](https://products.aspose.com/tasks/net)Hi friends! In today's blog, I will be giving you tour of latest [Aspose.Tasks][2] API. The good thing about Aspose team is that it publishes both .NET and Java-based API for Aspose.Tasks simultaneously every month. Both .NET and Java based variants are at same level in terms of features and both API users may explore the new features in their respective environments. In following section, I will be discussing about new features and improvement carried in API.

## Writing Metadata to Microsoft Project Files in C# and Java

Aspose.Tasks provides a facility for writing metadata to MPP files for calendars, tasks, task links, resources and resource assignments. The following example describes how to write metadata information to MPP files.



The similar Java based implementation for the same is like as under:

{{< gist aspose-com-gists 472405ac9bab4502a485ee007b92074c "Examples-src-main-java-com-aspose-tasks-examples-Miscellaneous-WriteMetadata-WriteMetadata.java" >}}

## Reading and Writing Formulas

Aspose.Tasks API supports reading/writing formulas to MPP project files. The Formula property of the **ExtendedAttributeDefinition** provides the interface for reading the formula value. The following examples describe how to read formulas from local as well as Enterprise Extended Attributes from the MPP file. It also shows how to write formulas to MPP file.

### Reading Formulas in Local and Enterprise Extended Attributes from MPP file

The similar Java based implementation for the same is like as under:

{{< gist aspose-com-gists 472405ac9bab4502a485ee007b92074c "Examples-src-main-java-com-aspose-tasks-examples-Formulae-WriteReadFormula-readingFormulasInLocalAndEnterpriseExtendedAttributes.java" >}}

### Writing Formulas in Extended Attributes to MPP File Formats {#WritingandReadingFormulas-WritingFormulasinExtendedAttributestoMPPFileFormats}

The similar Java based implementation for the same is like as under:

{{< gist aspose-com-gists 472405ac9bab4502a485ee007b92074c "Examples-src-main-java-com-aspose-tasks-examples-Formulae-WriteReadFormula-writingFormulasInExtendedAttributes.java" >}}

## Implementing Resource Prefix for Nested Resources

Aspose.Tasks provides ResourceSavingArgs.NestedUri property which allows saving nested resources (e.g. PNG inside SVG files) in the separate folder. In the following examples, we have demonstrated the use case for using the feature.



The similar Java based implementation for the same is like as under:

{{< gist aspose-com-gists 472405ac9bab4502a485ee007b92074c "Examples-src-main-java-com-aspose-tasks-examples-Resources-ResourcePrefixForNestedResources-ResourcePrefixForNestedResources.java" >}}

## Working with Extended Attributes

Microsoft Project (MSP) has an extensive XML data interchange schema that makes exchanging information between applications and programming with project files easier. The schema allows you to add extended attributes to tasks, resources and assignments. This article shows how to work with Extended Attributes in Aspose.Tasks.

The ExtendedAttribute property exposed by the Resource class can be used to manage the extended attributes of a resource. This property reads and writes an ArrayList of the ExtendedAttribute objects to deal with a resource's extended attributes. The ExtendedAttribute object further exposes the relevant properties



The similar Java based implementation for the same is like as under:

{{< gist aspose-com-gists 472405ac9bab4502a485ee007b92074c "Examples-src-main-java-com-aspose-tasks-examples-Resources-ExtendedResourceAttributes-ExtendedResourceAttributes.java" >}}

## Rendering Improvements

In this release the focus has also been set on improvement of rendering performance of API. The PDF and HTML rendering issues have also been addressed. Other improvements include resolution of issue pertaining to opening and saving of MPP files, incorrect task Id's and timelines.

Hold on, there's many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][3]

We have also maintained the working sample examples for both .NET and Java based APIs on [Github][4] so that users may right away use different samples and explore API features. You may also talk about API related issues with us in our product support [forum][5].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/11/Aspose.Tasks-for-.NET_.png
[2]: https://products.aspose.com/tasks
[3]: https://docs.aspose.com/tasks/net/aspose-tasks-for-net-19-8-release-notes/
[4]: https://github.com/aspose-tasks/
[5]: https://forum.aspose.com/c/tasks




