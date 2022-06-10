---
title: 'Support for TAR and GZIP Added With Aspose.ZIP for .NET 19.1'
date: Fri, 18 Jan 2019 21:04:01 +0000
draft: false
url: /2019/01/18/support-for-tar-and-gzip-added-with-aspose.zip-for-.net-19.1/
author: Muzammil Khan
summary: ''
tags: ['.NET ZIP API', 'Work with TAR and GZIP in CSharp']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/aspose_zip-for-net-100.png" alt="aspose-zip-for-net">}}


We are pleased to announce the release of Aspose.ZIP for .NET 19.1. This release introduces support for working with [TAR][1] and [GZIP][2]. For a detailed note on what is new and fixed, you may visit the [release notes][3] section of API.

# Support For Unix Standard TAR Archive

Aspose.ZIP for .NET now supports USTAR archives as most modern TAR programs read and write archives in the UStar (Unix Standard TAR) format, introduced by the POSIX IEEE P1003.1 standard from 1988. It was introduced additional header fields and older TAR programs ignore the extra information (possibly extracting partially named files), while newer programs will test for the presence of the "ustar" string to determine if the new format is in use. The UStar format allows for longer file names and stores additional information about each file. The maximum filename size is 256, but it is split among a preceding path "filename prefix" and the filename itself, so it can be much less.

# Support For GZIP Archive

GZIP is a file format and a software application used for file compression and decompression which is now supported by Aspose.ZIP for .NET with this latest release.

# API Resources

We have detailed information available online for getting started with the Aspose.ZIP for .NET API. These are:

*   [Product Documentation][4] – Provides detailed examples of working with the API
*   [API Reference Guide][5] – Details all the packages and classes of the API
*   [GitHub Examples][6] – Provides ready to run API examples
*   [Aspose.ZIP Forum][7] – Feel free to contact us on Aspose.ZIP forum for your queries




[1]: https://docs.fileformat.com/compression/tar/
[2]: https://docs.fileformat.com/compression/gz/
[3]: https://docs.aspose.com/display/zipnet/Aspose.ZIP+for+.NET+19.1+Release+Notes
[4]: https://docs.aspose.com/display/zipnet/Home
[5]: https://apireference.aspose.com/net/zip
[6]: https://github.com/aspose-zip/Aspose.ZIP-for-.NET
[7]: https://forum.aspose.com/c/zip




