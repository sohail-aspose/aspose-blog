---
title: 'Nested Mail Merge Regions in Word Documents using C#'
date: Fri, 13 Nov 2009 02:47:00 +0000
draft: false
url: /2009/11/13/aspose-words-for-net-8-0-supports-nested-mail-merge-regions-and-more/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

You might be wondering, Aspose.Words for .NET 7.0 is barely 2 months old and we already have 8.0, a major version change? Yes, and that change reflects the importance of one feature that we have finally added.  

You now can just design a template document like this:  

```
MERGEFIELD TableStart:Orders
…
    MERGEFIELD TableStart:OrderDetails
    …
    MERGEFIELD TableEnd:OrderDetails
MERGEFIELD TableEnd:Orders
```

and then call  

```
doc.MailMerge.ExecuteWithRegions(myDataSet); <br>
```

and Aspose.Words will do its magic to produce an order document. Then you can of course  

```
doc.Save(myStream, SaveFormat.Pdf);<br>
```

etc.

Aspose.Words' new support for nested mail merge regions allows you to generate reports from master-detail (parent-child) data with ease. If your data is inside a .NET **DataSet** object that has a proper **DataTable** and **DataRelationship** objects set up, then all you need to do is pass a **DataSet** to the Aspose.Words mail merge engine. It will automatically figure out data relationships and generate a report with the required data. On the other hand, it is also easy to implement your own mail merge data source interfaces **IMailMergeDataSource** and **IMailMergeDataSourceRoot** to generate a report from any data source be it a LINQ query, XML file or a set of business objects. We will be writing more in the blog and in the documentation about this great new feature. This release is "nested mail merge V1.0" and includes only the features mentioned above. There is a lot more we plan to add to the reporting functionality in Aspose.Words in the future. Feel free to submit your requests via the Support Forums.

There are more great new features, see the download page [https://downloads.aspose.com/words/net][1]




[1]: https://downloads.aspose.com/words/net




