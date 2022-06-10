---
title: 'New Mail Merge Cleanup Options in Aspose.Words for .NET and Java'
date: Wed, 04 Jan 2012 16:14:12 +0000
draft: false
url: /2012/01/04/new-mail-merge-cleanup-options-in-aspose.words-for-.net-and-java/
author: DmitryV
summary: ''
tags: ['Aspose.Words', 'Remove empty paragraphs in mail merge', 'mail merge', 'mail merge .net or java', 'mail merge cleanup options in .NEt and Java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="Remove Empty Fields Mail Merge C# Java">}}


In Aspose.Words 10.8, released a few days ago, we introduced some new options that allow removing various items from the document while a mail merge is performed. Until this release two properties controlled whether empty paragraphs and regions were removed - [MailMerge.RemoveEmptyParagraphs][1] and [MailMerge.RemoveEmptyRegions][2], respectively. These properties are still there, but have been marked obsolete, so there is a new way to instruct the mail merge engine how to perform a cleanup.

We have introduced a [MailMergeCleanupOptions][3] enumeration whose members are flags, so that different options may be used simultaneously. The options are specified via the [MailMerge.CleanupOptions][4] property which should be used instead of the obsolete properties.

## MailMergeCleanupOptions Members

The new property takes a number of enumeration members, each described below.

### None

This is the default value. Nothing interesting here.

### RemoveParentParagraphs

This option is generally similar to the **RemoveParentParagraphs** property which is now obsolete. However, the option is slightly improved in comparison to the property. The property only treated a paragraph as empty if it had no child nodes at all, while the new option removes a paragraph even if it contains whitespace characters like spaces or tabs. Previously, a paragraph with a space character in it would not be removed. Now, it will.

### RemoveUnusedRegions

This option is almost identical to the obsolete **RemoveEmptyRegions** property, but, again, is slightly improved. First, as you may note, the name is changed a bit. “Unused” is more correct than “empty” because there are, in reality, no empty merge regions. However, mail merge regions that are ignored by the mail merge engine for some reason, are unused. Second, unlike the property, the option removes all unused merge regions regardless of why they were skipped. The **RemoveEmptyRegions** property only removed regions which had a corresponding data source (like a data table) that was empty, that is, contained no records. The **RemoveUnusedRegions** option removes such regions too, and also removes regions that have no corresponding data source.

### RemoveUnusedFields

This is a new option for removing merge fields that are left in the document after mail merge, for example, if a corresponding value was not found.

### RemoveContainingFields

This is a new and very useful option for removing not only the merge fields themselves, but also all containing fields when the merge field is nested. Merge fields are often designed as child fields of the IF fields or similar in order to perform conditional merge. While merge fields are always replaced with their values during mail merge, the containing (parent) fields stay intact unless the new **RemoveContainingFields** option is enabled.

Note that **RemoveContainingFields** also works in conjunction with **RemoveUnusedFields**. It removes fields that contain unused merge fields, when the latter ones are removed thanks to **RemoveUnusedFields** being enabled.

## Combining Cleanup Options

So, since the new cleanup options are flags, you can combine any of them to fit different cleanup scenarios. For example, if you want to see no merge regions or fields in the resulting document (and no containing fields as well, if present), you can combine the following three options together:

```
Document doc = new Document("CleanupOptions.docx");
doc.MailMerge.CleanupOptions = MailMergeCleanupOptions.RemoveUnusedRegions |
MailMergeCleanupOptions.RemoveUnusedFields |
MailMergeCleanupOptions.RemoveContainingFields;
doc.MailMerge.ExecuteWithRegions(dataSet);
```

Or, if you wish to get rid of empty paragraphs that are left after merging, regardless of the reason:

*   a paragraph contained a merge field whose value is empty, or
*   a paragraph contained an IF field with a merge field inside, and the IF field's computed value becomes an empty string after the child field is merged,

just instruct Aspose.Words remove containing fields and empty paragraphs:

```
Document doc = new Document("CleanupOptions.docx");
doc.MailMerge.CleanupOptions = MailMergeCleanupOptions.RemoveEmptyParagraphs |
MailMergeCleanupOptions.RemoveContainingFields;
doc.MailMerge.ExecuteWithRegions(dataSet);
```

## Downloads

*   [Aspose.Words for .NET][5]
*   [Aspose.Words for Java][6]




[1]: https://docs.aspose.com/display/wordsnet/How+to+Remove+Unmerged+Fields%2C+Empty+Paragraphs+and+Unmerged+Regions
[2]: https://docs.aspose.com/display/wordsnet/How+to+Remove+Unmerged+Fields%2C+Empty+Paragraphs+and+Unmerged+Regions
[3]: https://docs.aspose.com/display/wordsnet/About+Mail+Merge
[4]: https://docs.aspose.com/display/wordsnet/About+Mail+Merge
[5]: https://downloads.aspose.com/words/net
[6]: https://downloads.aspose.com/words/java




