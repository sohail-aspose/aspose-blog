---
title: 'Aspose.Words for Reporting Services 3.0.0.0 Released'
date: Tue, 16 Dec 2008 02:48:00 +0000
draft: false
url: /2008/12/16/aspose-words-for-reporting-services-3-0-0-0-released/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Following the recent release of Aspose.Words for .NET 6.0 (which introduced an outstanding rendering feature), we have just made public a new major version of another product from the Aspose.Words family. Please welcome Aspose.Words for Reporting Services 3.0!

**Full support for Microsoft SQL Server 2008 Reporting Services (final version)**

Starting with this version, the product fully supports Microsoft SQL Server 2008 Reporting Services (only SSRS 2008 CTP 3 was supported until now). Now you can export tablix, richly formatted textboxes and other SSRS 2008 features to a bunch of Microsoft Word formats as well as a number of additional formats.

**Improved Document Layout**

We have significantly improved the layout of the exported documents. It especially applies to the flow layout mode which is default. Namely, we put special attention to the use of page breaks. We have introduced the **PageBreaks** configuration setting that is perhaps the most important after **DocumentLayout**. With this setting, you can easily control how page breaks are placed in the document:

*   _Smart (default)_ - allows the exporter decide when to insert a page break. This mode provides the best balance between the precision of export and the "editability" of the document.
*   _None_ - no page breaks in the document at all, just like on an HTML page. Enabling this mode may lead to some layout issues (such as a title expected to appear at the beginning of the page appears somewhere in the middle), but makes the document very easy to post process.
*   _OnEachPage_ - yes, as the name states, a page break is inserted at the end of each page. This usually makes the document look identical to what was expected, but a drawback is that the "editability" normally suffers from too many page breaks inserted.

**Optimized Items Positioning**

In flow layout mode it is sometimes impossible to position several document items without using a trick. We use invisible tables (that without borders) to position the items properly. This approach is widely used in HTML pages design. However, such tables should be used as rarely as possible and structured as simple as possible, because heaps of complex nested tables make the document awkward and hard to edit.

Aspose.Words for Reporting Services 3.0 involves a number of optimization algorithms that build positioning tables only where they are really needed and make them no more complex than needed. If a report is not too complicated and is properly designed, the resulting document may contain no positioning tables whatsoever.

**New Export Format**

Aspose.Words for Reporting Services 3.0 has introduced the new ODT export format, which allows you to export your reports to OpenOffice/StarOffice OpenDocument.

Note that the MSI installer installs all of the supported export formats. If you need only some of them (for instance, to prevent unneeded formats from appearing on the Report Manager dropdown), please install the product manually or remove corresponding entries from the rsreportserver.config file (see product documentation for more details). We plan to develop a tool that will simplify this process in the future.

Please download Aspose.Words for Reporting Services 3.0 from [http://www.aspose.com/community/files/52/ssrs-rendering-extensions/aspose.words.reporting.services/default.aspx][1].




[1]: http://www.aspose.com/community/files/52/ssrs-rendering-extensions/aspose.words.reporting.services/default.aspx




