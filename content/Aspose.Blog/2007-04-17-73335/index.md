---
title: 'Aspose.Words for Reporting Services Featuring AWesomeExport Technology'
date: Tue, 17 Apr 2007 01:43:00 +0000
draft: false
url: /2007/04/17/73335/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

It's been around 10 days since we released Aspose.Words for Reporting Services, the only solution on the market that enables so desperately requested export of reports to Microsoft Word documents. Now it's time to speak about what this unique product actually can do :)

We started working on this product several months ago and from the very beginning we've been keeping in mind one important thing. We intended to not only implement high-fidelity export without any losses or changes, but also to make the resulting documents convenient to edit and manage. This task is actually very difficult to accomplish because normally the output is either very exact to the design of the original reports **or** easy to modify... The goals seem to be mutually exclusive.

As you know, report items are absolutely positioned. Microsoft Word does support absolute positioning along with inline objects; and each type of layout has its own benefits and drawbacks. Nothing is better or worse. Apparently exporting to absolutely positioned objects is much more straightforward and that is what we have published in the first release of Aspose.Words for Reporting Services.

However, using this approach not always results in producing documents that allow easy add or remove text and objects. For example, while absolutely positioned images are surely acceptable, more complex report items may require further processing to appear editable in Word documents. We had to invent a smart conversion algorithm to be involved in such processing.

Given this, we decided to implement a technology we named _AWesomeExport_ (to maintain our AWesome line introduced last year). The ultimate goal of this technology is making the exported reports as close to common and habitual Microsoft Word documents as possible. That means the exported reports should not cause any difficulties when editing; ideally they should not differ from documents created directly in Word. We will be improving this technology and it will be evolving together with the product.

But initially we had to decide what to start with. What report items contain most of the data conveyed by reports? What report items are the most complex? The answer is obvious - those are tables and matrices. That's why we decided to apply the _AWesomeExport_ technology to those report items in the first place.

We have implemented the possibility of converting tables and matrices directly to floating tables in Word documents. That is a really unique feature. It is much simpler to export contents of tables and matrices to a rectangular set of textboxes or whatever those report items contain… but it is not always acceptable by the end users. I can see at least three major benefits provided by the "tables to tables" approach as compared to "tables to textboxes":

1.  Tables are much easier to edit than a bunch of drawing objects. Imagine you need to add or delete a row of cells and just compare the efforts required to accomplish this action in Word when dealing with a table which has a built-in support or with a large array of textboxes.
2.  Tables seem "lighter" for Word than hundreds or thousands of textboxes when loading, rendering, or scrolling documents. It is noticeable when exporting reports that contain huge tables or matrices.
3.  Reports are exported faster when tables are converted to tables rather than to a bunch of textboxes. Again, it is especially noticeable when exporting huge tables or matrices.

Of course, this type of conversion is not a panacea, as there is nothing ideal in our world. In rare cases there may occur some minor drawbacks. I have noticed the following:

1.  It's not allowed to set different top padding values for different cells in one row of the table whereas it is possible in RDL.
2.  It's not possible to explicitly set the Z-order for tables in Word (which may be an issue when the table is contained in a rectangle; perhaps we will fix this in the future).
3.  Floating tables may look slightly garbled when rendered or scrolled in Word (practically confirmed by Microsoft - refer to this article for tips and tricks).

However, as you can see, there are no serious trade-offs actually. That is why we have decided to make the "tables to tables" option enabled by default starting with the recently released Aspose.Words for Reporting Services v1.0.1. We hope this will satisfy most of you. If however you require to force the renderer to export tables and matrices to a set of textboxes (or other objects they contain), it is fairly easy to accomplish. All you need to do is edit the _rsreportserver.config_ file normally located in the _C:\\Program Files\\Microsoft SQL Server\\MSSQL.x\\Reporting Services\\ReportServer_ directory. Locate the **<Extension>** element that corresponds to the renderer you want to configure and add the following lines into it:

<Render>  
…  
<Extension Name="AWDOC" Type="Aspose.Words.ReportingServices.DocRenderer,Aspose.Words.ReportingServices">  
 <Configuration>  
  <DeviceInfo>  
   <UseFloatingTables>False</UseFloatingTables>  
  </DeviceInfo>  
 </Configuration>  
</Extension>

</Render>

Repeat this for all renderers whose behavior you want to alter. Voila :)

We have intentionally made this an option. Making rendering flexible and configurable is another goal of ours. While improving the _AWesomeExport_ technology, we will be adding various configuration options so that any big and complex report could be exported in the most suitable way.

We really hope you will enjoy our work. As always, we are looking forward to your reports and requests in our support forum. Yet another AWesome family member is growing :)

P.S. I have attached an archive containing two RTF files that show the two ways of exporting tables and matrices to Word documents. Notice the appearance is identical, but it's up to you to decide which document is easier to work with... By the way, _Matrix2FloatingTables.rtf_ is almost 1.5 times smaller than _Matrix2Textboxes.rtf_ - it seems to be the 4th benefit provided by the _AWesomeExport_ technology I forgot to mention :)








