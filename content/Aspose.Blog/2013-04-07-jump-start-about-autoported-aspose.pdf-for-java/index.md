---
title: 'Structure of Autoported Aspose.Pdf for Java'
date: Sun, 07 Apr 2013 13:40:59 +0000
draft: false
url: /2013/04/07/jump-start-about-autoported-aspose.pdf-for-java/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---

![Aspose.Pdf icon][1]

Recently we shared some information regarding the autoported Aspose.Pdf for Java, in which most of the features that are currently present in Aspose.Pdf for .NET, will become available. In fact, the autoported version will be a merged API, that is, Aspose.Pdf for Java and Aspose.Pdf.Kit for Java, and a new DOM API. The reason we felt the need to port .NET code to Java is because our .NET product line is much stronger (in terms of functionality & features) than the Java product line. This year, our major objective is to strengthen our Java product lines so that they offer the same set of features as our .NET products.

## Requirement of an autoported Release

When we started working on improving our Java product line, we had two options: Either we start building the product from the ground up by restructuring its architecture and make it compatible with our .NET product line, or we port the current .NET code to Java. We decided to go with the second option because using this approach, we only have to maintain one code base where we can introduce new features & enhancements and will be available on both platforms. With this approach in mind, we started migrating Aspose.Pdf for .NET code to Java.  After months of effort, we have an autoported version of Aspose.Pdf for Java which is in fact a merged API release. This new release has three major parts

*   Current Aspose.Pdf for Java
*   Aspose.Pdf.Kit module ported from .NET
*   New DOM API approach

In the first release of the autoported version, you will get two JAR files. One is the current Aspose.Pdf for Java where you can access all classes and enumerations using the aspose.pdf package. The second JAR file contains the com.aspose.pdf.facades and com.aspose.pdf packages.

## Why two JARs?

You might be wondering why we will release two JAR files instead of one? We wanted to keep things simple for us as well as for our users. We thought to use the divide and conquer approach. So we divided the migration activity in two parts.

1.  Current Aspose.Pdf for Java
2.  Migrate Aspose.Pdf.Kit and DOM portion from .NET to Java.

The overall intent has been to minimize the ripple effects that might occur after product migration. In the first phase, users of the current version of Aspose.Pdf for Java are not impacted. Users of Aspose.Pdf.Kit for Java, however, have to make some small changes to their code to get the benefit of the revamped version. Don’t be afraid. The code change will be minimal: you don't have to rewrite the whole applications.

Nonetheless, the option of trying and taking benefit of the new DOM approach is open to all users and we recommend trying it because it’s a new and restructured approach built on top of Document Object Model, with a bit faster response compared to the legacy products.

## Is it backward compatible?

Before trying out the new version, the first question that pops up in user’s mind is “**Is the new product backward compatible?**”. We love to take the legacy throughout our journey towards future and we don’t want to disappoint our customers. So I would like to share that along with the intent of introducing new features and functionalities on the Java platform, one of our major objectives has been to maintain and keep the backward compatibility with current versions. As shared earlier, Aspose.Pdf for Java users might not be impacted with the first auto-ported version because it will contain the current Aspose.Pdf for Java (legacy) release. However, Aspose.Pdf.Kit for Java customers will have to migrate to the autoported version. During all our testing, we have tried to ensure that current Aspose.Pdf.Kit for Java customers experience minimal impact after migration and they will have to make small tweaks to their code (by updating class and package references).

## Structure of the autoported Release

The following image shows the structure of the autoported release.

![](https://blog.aspose.com/wp-content/uploads/sites/2/2013/04/PDFNEWJAVA.png)

Please stay tuned as more details about autoported release will be shared in the coming days.




[1]: http://www.aspose.com/Images/aspose.pdf-logo2.jpg




