---
title: 'Create, Parse and Validate XBRL and iXBRL Financial Reports using C#'
seoTitle: ""
description: ""
date: Wed, 29 Apr 2020 13:35:51 +0000
draft: false
url: /2020/04/29/create-xbrl-instances-and-parse-and-validate-xbrl-and-ixbrl-files-in-csharp-asp.net/
author: Usman Aziz
summary: 'This article provides information about business reporting using the **XBRL standard**, the purpose of XBRL, and how to automate the process of **creating XBRL-based business reports in** .NET applications. Furthermore, it contains step by step methods to **parse XBRL and iXBRL** files and retrieve data programmatically using C#.'
tags: ['Create XBRL Instance in csharp asp.net', 'Parse XBRL in csharp', 'Parse iXBRL in csharp', 'Validate XBRL files in csharp', 'Validate iXBRL files in csharp']
categories: ['Aspose.Finance Product Family']
---



{{< figure align=center src="images/aspose_finance.png" alt="aspose.finance">}}


This article provides information about business reporting using the **XBRL standard**, the purpose of XBRL, and how to automate the process of **creating XBRL-based business reports in** .NET applications. Furthermore, it contains step by step methods to **parse XBRL and iXBRL** files and retrieve data programmatically using C#. Last but not the least, it provides some simple ways to **validate XBRL and iXBRL** files using C#.

## eXtensible Business Reporting Language (XBRL)

[XBRL][1] is a globally used XML-based standard and file format for business reporting. It makes it easier for various companies and accounting organizations to efficiently and accurately organize, compile, and communicate financial statements or other finance-related information/data. Since XBRL is based on XML (Extensible Markup Language), it uses tags to keep and parse every piece of financial data. [iXBRL][2] (inline XBRL) is another variant that makes it possible to keep financial data in a human-readable and machine-readable form at the same time. In contrast with XBRL, iXBRL uses the HTML standard along with some extra tags for figures and statements.

The tags in both, XBRL and iXBRL, are parsed using XBRL-compatible software to retrieve the data. In order to automate XBRL parsing, Aspose offers [Aspose.Finance for .NET][3] API. It is a .NET class library that makes it even easier to **create XBRL instances** programmatically using **C# or VB.NET**. In addition, it allows you to **parse and validate the XBRL or iXBRL** files within the .NET applications. Aspose.Finance for .NET provides the following XBRL/iXBRL manipulation features that you will learn in this article.

*   [Create XBRL instance from scratch][4]
*   [Parse XBRL or iXBRL files][5]
*   [Validate XBRL or iXBRL files][6]

You can install Aspose.Finance for .NET from [NuGet][7] or [download][8] its DLL to manually reference it in your project.

## Create XBRL Instance from Scratch in C# {#create}

Aspose.Finance for .NET makes it simple to create XBRL instances from scratch. You can also add the schema reference, context, units, items, footnote links, role references, and arc role references in the newly created XBRL instance. The following are the steps to create an XBRL instance:

*   Create an instance of the [XbrlDocument][9] class.
*   Access instances' collection from _XbrlDocument_ object into [XbrlInstanceCollection][10] object.
*   Add a new XBRL instance using [XbrlInstanceCollection.Add()][11] method.
*   Save the XBRL file using [XbrlDocument.Save(string)][12] method.

The following code sample shows how to create an XBRL instance in C#.

{{< gist aspose-com-gists d3d183d03a9cc8e4ce248a95919a6cff "CreateXbrlDocument.cs" >}}

Once you have created the instance of XBRL, you can insert objects to it which are discussed in the following articles:

*   [Specify schema reference in XBRL][13]
*   [Add contexts in XBRL][14]
*   [Insert units in XBRL][15]
*   [Add items in XBRL][16]
*   and [more][17].

## Parse XBRL or iXBRL Files in C# {#parse}

Aspose.Finance for .NET provides an easy way of parsing XBRL files and retrieving their content within a few lines of code. The following sections contain the steps and code samples of how to parse XBRL and iXBRL files.

### Parse XBRL Files in C#

The following are the steps to parse an XBRL file using Aspose.Finance for .NET.

*   Create an instance of the [XbrlDocument][18] class and initialize it with the path of an XBRL file.
*   Get the instances in the XBRL into an [XbrlInstanceCollection][19] object using [XbrlDocument.XbrlInstances][20] property.
*   Access the desired XBRL instance from the collection using the [XbrlInstance][21] class.
*   Parse the content of the XBRL instance.

The following code sample demonstrates how to parse an XBRL file in C#.

{{< gist aspose-com-gists d3d183d03a9cc8e4ce248a95919a6cff "ReadXbrlDocument.cs" >}}

### Parse iXBRL Files in C#

Parsing an iXBRL file is comparatively easier and can be done using the following steps.

*   Create an object of the [InlineXbrlDocument][22] class and initialize it with the iXBRL file's path.
*   Access the content of the file using the _InlineXbrlDocument_ object, i.e. [InlineXbrlDocument.Facts][23] etc.

The following code sample shows how to parse and read an iXBRL file in C#.

{{< gist aspose-com-gists d3d183d03a9cc8e4ce248a95919a6cff "ReadIxbrlDocument.cs" >}}

## Validate XBRL or iXBRL Files in C# {#validate}

The XBRL and iXBRL files must comply with the validation rules in the [XBRL specification][24] and [iXBRL specification][25] respectively. Disobeying the specification rules may invalidate the files. Aspose.Finance for .NET also lets you validate XBRL or iXBRL files in order to find out the errors. The following sections demonstrate how to validate XBRL and iXBRL files.

### Validate XBRL Files in C#

The following are the steps to validate an XBRL file:

*   Create an instance of the [XbrlDocument][26] class.
*   Access the instance to be validated from the [XbrlInstanceCollection][27].
*   Validate XBRL instance using [XbrlInstance.Validate()][28] method.

The following code sample shows how to validate an XBRL file in C#.

{{< gist aspose-com-gists d3d183d03a9cc8e4ce248a95919a6cff "ValidateXbrlInstance.cs" >}}

### Validate iXBRL Files in C#

The below steps are used to validate an Inline XBRL file.

*   Create an instance of the [InlineXbrlDocument][29] class and initialize it with the iXBRL file's path.
*   Call [InlineXbrlDocument.Validate()][30] method.

The following code sample shows how to validate an iXBRL file in C#.

{{< gist aspose-com-gists d3d183d03a9cc8e4ce248a95919a6cff "ValidateIxbrlInstance.cs" >}}

Learn more about the validation error codes and error messages from [here][31].

## Explore the API

You can learn more about how to create, parse, and validate XBRL and iXBRL files from the following resource:

*   [Documentation][32]
*   [Source code examples][33]
*   [Support forum][34]

## Try Aspose.Finance for .NET for Free

Aspose offers a temporary license to evaluate its APIs free of cost. You may also post your request and [get a temporary license][35].

## See Also

*   [Word Automation and Report Generation in C#][36]




[1]: https://en.wikipedia.org/wiki/XBRL
[2]: https://en.wikipedia.org/wiki/XBRL#iXBRL
[3]: https://products.aspose.com/finance/net
[4]: #create
[5]: #parse
[6]: #validate
[7]: https://www.nuget.org/packages/Aspose.Finance
[8]: https://downloads.aspose.com/finance/net
[9]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument
[10]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstancecollection
[11]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstancecollection/methods/add
[12]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/methods/save
[13]: https://docs.aspose.com/display/financenet/Create+XBRL+files#CreateXBRLfiles-Addschemareference
[14]: https://docs.aspose.com/display/financenet/Create+XBRL+files#CreateXBRLfiles-Addcontext
[15]: https://docs.aspose.com/display/financenet/Create+XBRL+files#CreateXBRLfiles-Addunit
[16]: https://docs.aspose.com/display/financenet/Create+XBRL+files#CreateXBRLfiles-Additem
[17]: https://docs.aspose.com/display/financenet/Create+XBRL+files
[18]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument
[19]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstancecollection
[20]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/properties/xbrlinstances
[21]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance
[22]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument
[23]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument/properties/facts
[24]: http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html
[25]: http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html
[26]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument
[27]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstancecollection
[28]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/methods/validate
[29]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument
[30]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument/methods/validate
[31]: https://docs.aspose.com/display/financenet/Validate+XBRL+and+iXBRL+files#ValidateXBRLandiXBRLfiles-Validationerrorcodes
[32]: https://docs.aspose.com/display/financenet/Product+Overview
[33]: https://github.com/aspose-finance/Aspose.Finance-for-.NET
[34]: http://forum.aspose.com
[35]: https://purchase.aspose.com/temporary-license
[36]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/





