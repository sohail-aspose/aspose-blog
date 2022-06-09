---
title: 'Create OFX Request or Response Programmatically with C# API'
seoTitle: "Create OFX Request or Response Programmatically with C# API"
description: "You can parse or create OFX Request or Response Programmatically using C#. Save file as OFX 1.03 or 2.2 format specifications."
date: Tue, 23 Feb 2021 19:51:00 +0000
draft: false
url: /2021/02/23/create-parse-ofx-request-or-response-programmatically-csharp-api/
author: Farhan Raza
summary: 'OFX, Open Financial Exchange, files are popularly used for exchanging financial information. It is used in client-server as well as Cloud-based systems. So the request-response model is implemented for exchanging financial information. Financial service providers like banks, data aggregators, etc. often use OFX for creating, analyzing, or aggregating financial data. Likewise, they utilize it for managing financial data exchange in their products and services.'
tags: ['OFX 2.2', 'OFX Request', 'OFX Response', 'Parse OFX', 'Parse OFX in C#']
categories: ['Aspose.Finance Product Family']
---



{{< figure align=center src="images/parse-ofx-request-response.png" alt="parse ofx request response">}}


[OFX][1], Open Financial Exchange, files are used for exchanging financial information. It is used in client-server as well as Cloud-based systems. So the request-response model is used for exchanging financial information. Let us learn the OFX request and response:

*   [Parse OFX Request and Response – C# API Installation][2]
*   [Create OFX Request Programmatically using C#][3]
*   [Create OFX Response Programmatically with C#][4]

## Parse OFX Request and Response – C# API Installation {#section1}

[Aspose.Finance for .NET][5] API supports several features for processing and parsing financial data. You can download it from the [Downloads][6] section or install via [NuGet][7] gallery with the following command:

```
PM> Install-Package Aspose.Finance
```

Moreover, the evolution of OFX is worth mentioning here. OFX version 1 through 1.6 is based on [SGML][8] syntax. The later versions rely on XML specifications. For better understanding, we will create OFX request and response files in both formats (1.03 & 2.2).

## Create OFX Request Programmatically using C# {#section2}

OFX protocol is a standard for a two-way exchange of financial data. You can easily create a request by following the steps below:

1.  Initialize [Ofx Request Document][9] object
2.  Create [Sign on Request][10] instance
3.  Set different properties
4.  Save OFX request in 1.03 and 2.2 format

The code snippet below explains how to create OFX Request programmatically using C# language:

{{< gist aspose-com-gists 8c846b821b082fd82bf1df3960b49786 "Create-OFX-request.cs" >}}

## Create OFX Response Programmatically with C# {#section3}

You can create an OFX response in .NET based applications programmatically using C#. The following steps explain OFX response creation process:

1.  Initialize [Ofx Response Document][11] class object
2.  Declare [Sign on Response][12] and set values
3.  Save response with [Ofx Version Enum][13] Enumeration

The following code snippet shows how to create OFX response programmatically using C#:

{{< gist aspose-com-gists 8c846b821b082fd82bf1df3960b49786 "Create-OFX-response.cs" >}}

## Conclusion

OFX standard is platform-independent so the users can choose the system environment or platform to use financial processing features. It enables the banks, brokerages, and payroll processing companies to create tailored solutions. You can get in touch via the [Free Support Forum][14]. We will be glad to help you!

## See Also

[Convert XBRL to XLSX or iXBRL Programmatically in C#][15]




[1]: https://en.wikipedia.org/wiki/Open_Financial_Exchange
[2]: #section1
[3]: #section2
[4]: #section3
[5]: https://products.aspose.com/finance/net
[6]: https://releases.aspose.com/
[7]: https://www.nuget.org/packages/Aspose.Finance/
[8]: https://en.wikipedia.org/wiki/Standard_Generalized_Markup_Language
[9]: https://apireference.aspose.com/finance/net/aspose.finance.ofx/ofxrequestdocument
[10]: https://apireference.aspose.com/finance/net/aspose.finance.ofx.signon/signonrequest
[11]: https://apireference.aspose.com/finance/net/aspose.finance.ofx/ofxresponsedocument
[12]: https://apireference.aspose.com/finance/net/aspose.finance.ofx.signon/signonresponse
[13]: https://apireference.aspose.com/finance/net/aspose.finance.ofx/ofxversionenum
[14]: https://forum.aspose.com/c/finance
[15]: https://blog.aspose.com/2021/02/15/convert-xbrl-xlsx-excel-ixbrl-inline-csharp/





