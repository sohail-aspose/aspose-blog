---
title: 'Remove Comment Reply and Set Base Document for Comparison using Aspose.Words for Java 17.10'
date: Wed, 18 Oct 2017 06:15:27 +0000
draft: false
url: /2017/10/18/improved-document-comparison-add-remove-comment-reply-footnote-layout-columns-and-use-machine-fonts-in-htmlfixed-in-aspose.words-for-java-17.10/
author: Tilal Ahmad
summary: ''
tags: ['Add or Remove Comment Reply in Word in Java', 'Java Word API', 'Word document comparison in Java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-Java.png" alt="">}}


We are pleased to announce new release of [Aspose.Words for Java 17.10][1]. The release of this month contains number of new features, enhancements and bug fixes of the issues reported by our users in previous versions.  Please check the detailed [release notes of this version][2] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from [release notes folder][3], to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Set Base Document for Document Comparison

A new feature has been added in this release to use the base document during the comparison of documents. This feature is related to Microsoft Word “Show changes in” option in the “Compare Documents” dialog box. We have added Public property CompareOptions.setTarget to the CompareOptions class to provide the ability to determine base document upon document comparison. Please read the following article for more detail:  
[Set Target Document for Comparison Differences][4]

```
Document docA = new Document(pathA);
Document docB = new Document(pathB);
CompareOptions options = new CompareOptions();
options.setIgnoreFormatting(true);
options.setTarget(ComparisonTargetType.NEW);
docA.compare(docB, "am", new Date(), options);
```

## Dynamic Chart Series Removal Support in LINQ Reporting Engine

We have added a new feature in LINQ Reporting Engine to remove chart series dynamically. In particular, this feature is useful when you need to restrict access to sensitive data in chart series for some users of your application. We have introduced a new tag **<<**_**removeif \[conditional Expression\]>>** _for the purpose, please read more detail from here.  
[Using Charts to Represent Sequential Data][5]

## Add and Remove Comment Reply

We have introduced new features to add a reply to a comment and remove a reply.  Two new public methods Comment.AddReply and Comment.RemoveReply is implemented in the new version of Aspose.Words for Java to [add and remove comment’s reply][6]. As per MS Office limitations Aspose.Words for Java supports only 1 level of replies in the document.

```
Document doc = new Document(dataDir + "TestFile.doc");
Comment comment = (Comment)doc.getChild(NodeType.COMMENT, 0, true);
//Remove the reply
comment.removeReply(comment.getReplies().get(0));
//Add a reply to comment
comment.addReply("John Doe", "JD", new Date(), "New reply");
dataDir = dataDir + "TestFile_Out.doc";
// Save the document to disk.
doc.save(dataDir);
```

## Added Feature to Get and Set Number of Footnote Layout Columns

We have added public property FootnoteOptions.Columns to set or get the [number of columns with which the footnotes area is formatted][7]. The default value is 0. If this property has a value of 0, then the footnotes area is formatted with a number of columns based on the number of columns of the related page.

```
Document doc = new Document(dataDir + "TestFile.docx");
//Specify the number of columns with which the footnotes area is formatted.
doc.getFootnoteOptions().setColumns(3);
dataDir = dataDir + "TestFile_Out.doc";
// Save the document to disk.
doc.save(dataDir);
```

## Sign Word document using Signature Provider Identifier

We have added public properties SignOptions.ProviderId and SignatureLine.ProviderId in this version of Aspose.Words for Java to sign Word document using signature provider identifier. Please refer to the following articles.  
[Signing Word Document using Signature Provider Identifier][8]  
[Create New Signature Line Sign Word Document using Provider Identifier][9]

## Get Relative Alignment of Table

A new feature has been added in this release [to get alignment of a Table][10]. You can get the relative alignment of a Table using Table.getRelativeHorizontalAlignment() and Table.getRelativeVerticalAlignment() properties when its text wrapping is “Around”.

```
Document doc = new Document(dataDir + "Table.Document.doc");
// Retrieve the first table in the document.
Table table = (Table) doc.getChild(NodeType.TABLE, 0, true);
if (table.getTextWrapping() == TextWrapping.AROUND) {
	System.out.println("RelativeHorizontalAlignment: " + table.getRelativeHorizontalAlignment());
	System.out.println("RelativeVerticalAlignment: "   + table.getRelativeVerticalAlignment());
} else {
	System.out.println("Alignment: " + table.getAlignment());
}
```

## Prevent Embedding Fonts while Saving into HTML Fixed Format

By default, Aspose.Words for Java embed fonts in HtmlFixed format. We have introduced HtmlFixedSaveOptions.UseTargetMachineFonts property to prevent embedding fonts while saving Documents into HTML Fixed Format and use fonts from the target machine. For more detail, please check the following link.   
[Prevent Embedding Fonts while saving Document into HtmlFixed][11]

```
// Load the document
Document doc = new Document(filePath);
HtmlFixedSaveOptions options = new HtmlFixedSaveOptions();
options.setUseTargetMachineFonts(true);
dataDir = dataDir + "Test File_out.html";
// Save the document to disk.
doc.save(dataDir, options);
```

## Other Improvements

There are 83 improvements and fixes in this regular monthly release. The most notable are:

*   "Don't add extra space for raised/lowered characters" compatibility option is supported.
*   Multiple improvements in RTL and Asian text handling.
*   LINQ Reporting Engine supports dynamic chart series removal.
*   An option to prevent the fonts embedding into HTML Fixed output implemented. Introduced HtmlFixedSaveOptions.UseTargetMachineFonts property.
*   Rendering of HTML fixed documents with “PRC” encoding fonts has been improved.
*   An algorithm, which mimics the behavior of MS Word when rendering of rotated VML shapes with text boxes.
*   Rendering of “Surface” and “Stock” DrawingML Charts has been improved.
*   Added CompareOptions.Target property and enumeration ComparisonTargetType.
*   Added public methods to add and remove replies to comment.
*   Ability to get and set the number of footnote layout columns.
*   Provide API similar to SignatureSet.AddSignatureLine Method (Office).
*   Expose Table.HorizontalAlignment property public.

## Aspose.Words for Java Resources

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][12]
*   [Download Aspose.Words for Java][13]
*   [Install Aspose.Words for Java from Maven][14]
*   Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][15]
    *   [Paid Support Forum][16]
*   [Words for Java online documentation][17]– Help documentation.
*   [Words for Java online API reference][18]– API reference documents.
*   [Enable Blog Subscription][19]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][20] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-17.10/
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.10+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.10+Release+Notes
[4]: https://docs.aspose.com/display/wordsjava/How+to+Compare+Two+Word+Documents#HowtoCompareTwoWordDocuments-SetTargetDocumentforComparisonDifferences
[5]: https://docs.aspose.com/display/wordsjava/Using+Charts+to+Represent+Sequential+Data
[6]: https://docs.aspose.com/display/wordsjava/Working+with+Comments#WorkingwithComments-HowtoAddandRemoveComment'sReply
[7]: https://docs.aspose.com/display/wordsjava/Working+with+Document#WorkingwithDocument-HowtoSetNumberofFootnoteLayoutColumns
[8]: https://docs.aspose.com/display/wordsjava/Working+with+Digital+Signatures#WorkingwithDigitalSignatures-SigningWordDocumentusingSignatureProviderIdentifier
[9]: https://docs.aspose.com/display/wordsjava/Working+with+Digital+Signatures#WorkingwithDigitalSignatures-CreateNewSignatureLineSignWordDocumentusingProviderIdentifier
[10]: https://docs.aspose.com/display/wordsjava/Applying+Formatting+to+Table%2C+Row+and+Cell#ApplyingFormattingtoTable,RowandCell-HowtoGettheTable'sAlignment
[11]: https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-PreventEmbeddingFontswhilesavingDocumentintoHtmlFixed
[12]: https://www.aspose.com/products/words/java
[13]: https://downloads.aspose.com/words/java
[14]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-words/
[15]: https://forum.aspose.com/c/words
[16]: https://helpdesk.aspose.com/
[17]: https://docs.aspose.com/display/wordsjava/Home
[18]: https://apireference.aspose.com/java/words
[19]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[20]: https://github.com/aspose-words/Aspose.Words-for-Java




