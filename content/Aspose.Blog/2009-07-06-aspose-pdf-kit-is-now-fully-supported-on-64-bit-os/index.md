---
title: 'Aspose.Pdf.Kit is now fully supported on 64-bit OS'
date: Mon, 06 Jul 2009 14:43:00 +0000
draft: false
url: /2009/07/06/aspose-pdf-kit-is-now-fully-supported-on-64-bit-os/
author: Shahzad Latif
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

A new release of Aspose.Pdf.Kit is published on Sunday, July 05, 2009. The good news is that 64-bit OS is now fully supported by [Aspose.Pdf.Kit 3.5.0.0][1]. Previously, some unmanaged code was used to support certain features, which caused problems on 64-bit OS; however, now the code has been completely converted to the managed code which provides the freedom. The resource file, previously included in the installer, is no more required. Only the DLL needs to be deployed.

That's not all in the package! In addition to some bug fixes, we have added some new features. PdfFileInfo class provides a new static property KitVersion, which allows you to get the version of the Aspose.Pdf.Kit currently being used in the application.

Some new features have been added in the Form, FormEditor, and PdfExtractor classes. GetFieldLimit method allows you to get the length limit of the text field; while previously, you could only set the limit of the field. Now, GetRichText method of the Form class can be used to get the text from a rich text box along with the formatting information.

GetAttachmentInfo method providing the detailed information about the attachment and [SetFieldAlignmentV][2] method aligning the field text vertically are also the part of this release. Some improvements have also been made in text extraction, bookmarks and annotation areas.

We believe the new release is going to help you a lot providing more features and flexibility. If you need any further help or find questions, we're here to help you out; post your questions at [Aspose.Pdf.Kit forums][3].




[1]: http://www.aspose.com/community/files/51/file-format-components/aspose.pdf.kit-for-.net-and-java/entry186896.aspx
[2]: https://docs.aspose.com/display/cellsjava/Home
[3]: http://www.aspose.com/community/forums/aspose.pdf.kit-for-.net-java-and-reporting-services/215/showforum.aspx




