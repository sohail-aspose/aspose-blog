---
title: '.NET Standard 1.3 version Discontinued in Aspose.BarCode for .NET 19.7'
seoTitle: ".NET Standard 1.3 version Discontinued in Aspose.BarCode for .NET 19.7"
description: ""
date: Wed, 25 Sep 2019 15:17:24 +0000
draft: false
url: /2019/09/25/.net-standard-1.3-version-discontinued-in-aspose.barcode-for-.net-19.7/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="">}}


Process of up-gradation and performance improvement is going on and on for Aspose.BarCode and here we are with a new version of [Aspose.BarCode for .NET 19.7][1]/). We have removed the support for older versions of .NET standard 1.3 and compact version also which is very less used nowadays. You can get a list of all the changes and upgradations in the [release notes][2] for this new version.

## Discontinue support for .NET Standard 1.3

We have discontinued the support for .NET Standard 1.3 and have removed it from our DLL to make it lighter and manageable. You can use Aspose.BarCode for .NET for all the .NET standard versions after v1.3. All the legacy code, function calls and features are removed for this version.

## Remove compact version support

In this new release support for compact version is also removed as it is very less used and requires to keep the least used code in our code base. These changes has made the product little lighter and also the code management is quite easy now.

## Remove Obsolete Code

There was obsolete code which was not required as all the alternatives were provided in the past for them. Announcements were also made to remove them along with the warnings while programming with these obsolete APIs. You may go through the release notes to get list of all such obsolete APIs which are no more the part of our latest versions.

## Suggestion for decoding ISMN and ISSN

Along with cleaning the product we have also addressed different issues which are faced by users. Some users were decoding ISMN and ISSN image files using BarCodeReader and getting one character less than the expected. It is suggested that out of ISSN, ISBN, ISMN and EAN13, better to use EAN13 to get barcode without any changes or post-processing like ISSN because for other types the code text and checksum are slitted. In this case use is suggested to use one of the following ways as per his ease.

*   GetCodeText() + GetCheckSum() methods
*   GetCodeText(true) - true means add checksum to codetext.

So this all about this release. Go through the release notes to get detailed description of all the changes mention above.




[1]: https://downloads.aspose.com/barcode/net/new-releases/aspose.barcode-for-.net-19.7-(dlls-only
[2]: https://docs.aspose.com/display/barcodenet/Aspose.BarCode+for+.NET+19.7+Release+Notes




