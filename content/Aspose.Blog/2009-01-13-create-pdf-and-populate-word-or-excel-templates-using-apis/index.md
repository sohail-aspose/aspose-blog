---
title: 'ResWare performs Real estate Process flow by Populating Word or Excel Templates and Renders output in PDF using Aspose APIs'
date: Tue, 13 Jan 2009 17:54:00 +0000
draft: false
url: /2009/01/13/create-pdf-and-populate-word-or-excel-templates-using-apis/
author: Bryan Buus
summary: ''
tags: ['.NET APIs to process Word and Excel files', 'Aspose.Cells', 'Aspose.Words', 'Convert DOC and DOCX to PDF format', 'Convert XLSX to PDF format', 'Dynamically generate MS Excel files', 'Dynamically generate MS Word documents', 'Excel to PDF conversion API', 'Populate Word template with data and export to PDF', 'Render XLS file to PDF format', 'Single .dll to perform all Word document processing', 'Success Stories', 'Word document manipulation without MS Office Automation', 'Word to PDF conversion API']
categories: ['Aspose.Words Product Family', 'Aspose.Total Product Family', 'Aspose.Cells Product Family']
---

## About Adeptive Software



{{< figure align=center src="images/ResWare-logo_1046_272.png" alt="ResWare company logo">}}


[Adeptive's][1] leading product, ResWare™ V3.0, is a real estate process flow software package that can be customized to manage any workflow process in the industry. We were previously using Microsoft Word and Excel automation for generating templates and Ghostscript to generate PDFs. We began having serious performance problems recently, where Word would hang, causing all sorts of problems.

## Requirements Scenario

We were using Microsoft Word and Excel to dynamically generate documents by manually populating Word merge fields and Excel cells with data pulled from our database on the fly. This was implemented using COM interop objects with C#.

This was ugly to say the least, as the COM bridges cause memory issues (_every object needs to be explicitly released_). This would often cause Word and Excel instances to be left hanging around on the server, which was also not good. In addition, we were using Ghostscript to convert Word and Excel documents to PDF on the fly. The approach we were using did not exactly lend itself to a high-volume,multi-threaded, scalable approach.

We wanted to remove the server-side dependency on Word, Excel, and Ghostscript. In various technical bulletins, Microsoft has made it very clear that Word and Excel are not designed to be used in a server environment, and should not be used for that sort of thing.

We discovered this was the case when we tried to use Office to do just that, in a high-load environment. We managed to work around most of the issues with clever code, but Word and Excel still caused problems, especially as the load went up. Word would crash randomly or, even worse, generate a popup that would freeze the entire template generation. We eventually came to the conclusion that our approach was not scalable to the levels we needed. At this point, we did our homework and turned to the [Aspose product][2] suite.

## Solution Implementation

We recorded all of our PDF generation and Word and Excel template populations to use the [Aspose components][3].

Recoding did not take long at all. The APIs are very clean and intuitive, and the [documentation is excellent][4]. Redistribution was simple, as each component has a single DLL with no dependencies. It’s pretty much just plug-and-play! Re-writing the code, which would have taken several man-months to develop, took just two man-weeks to entirely swap out. We only wish that we had known about [Aspose][5] when we started developing the product five years ago!

When we were using Word and Excel, we had to start our server process on the console, since Word and Excel were occasionally throwing up pop-up dialogs. If the server process was running as a service, the pop-ups wouldn’t be visible, and the server would come to a screeching halt. In addition, the calls that had to be made to Ghostscript also generated DOS windows. Whereas [Aspose][6] is all DLLs and we finally don’t have pop-ups, windows, or other craziness to worry about and we were able to change the server into being a service, at last!

Lastly, the [support][7] provided by [Aspose][8] was exceptional, even before we had bought the product and were simply evaluating its use. Questions posted in their [support forum][9] were responded within hours, usually with a required solution. I can’t stress enough how important this is. Other 3rd party providers’ "support" is laughable compared to what we received. No waiting for months for a solution and a new build!

## Benefits

Once implemented, we immediately noticed a 4x speed increase in the [template population and PDF generation][10]. Our template generation is very reliable now, and we’re confident that we can handle the load that our larger clients demand.

We don’t even need Microsoft Office installed on the server anymore! Our clients are much happier and we receive fewer support calls, which obviously saves time and money.

I can honestly say that I haven’t had a better outcome with any 3rd party provider (_and we’ve had to use our fair share of them_)!

## ScreenShots



{{< figure align=center src="images/Adeptive-aspose-total-case-study.png" alt="Template administration preview" caption="Image 1:- **Template Administration**">}}




{{< figure align=center src="images/Adeptive-aspose-total-case-study-1.png" alt="Template fields in word preview" caption="Image 2:- **Template Fields in Word**">}}




{{< figure align=center src="images/Adeptive-aspose-total-case-study-2.png" alt="Preview to render merged document output to PDF format" caption="Image 3: - **Merge Multiple Document Types into a Single PDF**">}}





[1]: https://www.adeptivesw.com/
[2]: https://products.aspose.com/
[3]: https://products.aspose.com/
[4]: https://docs.aspose.com/display/totalnet/Home
[5]: https://www.aspose.com/
[6]: https://www.aspose.com/
[7]: https://forum.aspose.com/
[8]: https://www.aspose.com/
[9]: https://forum.aspose.com/
[10]: https://docs.aspose.com/display/wordsnet/Loading%2C+Saving+and+Converting




