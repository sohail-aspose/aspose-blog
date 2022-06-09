---
title: 'Insert or Delete Comments in Word (DOCX/DOC) using Java'
seoTitle: ""
description: ""
date: Wed, 12 Aug 2020 23:50:22 +0000
draft: false
url: /2020/08/12/insert-delete-comments-in-word-using-java/
author: Farhan Raza
summary: ''
tags: ['delete comments in word', 'insert comments in word', 'insert comments in word java', 'remove comments in words']
categories: ['Aspose.Words Product Family']
---

Comments are used in word documents, [DOCX][1] or [DOC][2], for suggesting improvements and modifications. Let us explore how to insert comments as well as deleting or removing comments programmatically using Java. You can add author name, initials, comment text, date, and time based on your requirements. We will be performing all of these tasks using [Aspose.Words for Java][3] API.

Here we will be learning following use cases related to comments in word documents:

*   [Insert Comment in Existing Word Document using Java][4]
*   [Insert Comment in New Word Document using Java][5]
*   [Delete Specific Comments from Word Document using Java][6]
*   [Delete All Comments from Word Documents using Java][7]

## Insert or Delete Comments in Word files (DOCX/DOC) API – Installation

You can download the latest version of Aspose.Words for Java API from [Downloads][8] section or from Maven repository, as per the configurations mentioned below:

### Repository```
<repositories>
    <repository>
        <id>AsposeJavaAPI</id>
        <name>Aspose Java API</name>
        <url>https://repository.aspose.com/repo/</url>
    </repository>
</repositories>
```

### Dependency```
<dependencies>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-words</artifactId>
        <version>20.6</version>
        <classifier>jdk17</classifier>
    </dependency>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-words</artifactId>
        <version>20.7</version>
        <classifier>javadoc</classifier>
    </dependency>
</dependencies>
```

So the API has been configured now and we can proceed to explore different use cases of working with comments in Word documents.

## Insert Comment in Existing Word Document using Java {#section1}

You can insert or add comments in existing Microsoft Word files, DOCX or DOC, with Aspose.Words for Java API. This can be helpful when reviewing documents, like a supervisor can suggest several changes or improvements on a feasibility report. Moreover, anyone with edit permissions of a word document can work with comments. You need to follow the steps below to insert comments in word file (DOCX/DOC):

1.  Load existing DOCX file with Document class
2.  Create a comment
3.  Save DOCX file

The following code snippet shows how to insert a comment in Word document using Java:

{{< gist aspose-com-gists ef9c6086cf6e7030afda888475736625 "CommentsExisting.java" >}}

Below screenshot shows a sample comment added in existing Word documents:



{{< figure align=center src="images/CommentExisting-1024x535.png" alt="Insert comment in word">}}


## Insert Comment in new Word Document using Java {#section2}

Comments are also helpful when creating a new word document. For instance, some text may need elaboration which can be explained with the help of comment. Likewise, there could be hundreds of use cases where comments can assist while creating a new DOCX file. You can easily add or insert comments by following the steps below:

1.  Initialize DocumentBuilder object
2.  Add sample text
3.  Create a custom comment
4.  Save DOCX file

The code snippet below shows how to insert comments while creating a new word document from scratch, using Java:

{{< gist aspose-com-gists ef9c6086cf6e7030afda888475736625 "CommentsNew.java" >}}

The screenshot below shows the output where the comment is added on new word document:



{{< figure align=center src="images/CommentsNew-1024x415.png" alt="delete comment in word">}}


## Delete Specific Comments from Word Document using Java {#section3}

Comments are often deleted when suggested improvements or modifications are incorporated into the word document. When you need to delete specific comments then you can follow the steps below:

1.  Load source word document
2.  Specify author name
3.  Remove comments from the specified author

The code snippet below shows how to delete specific comments from word file using Java:

{{< gist aspose-com-gists ef9c6086cf6e7030afda888475736625 "DeleteSpecificComment.java" >}}

## Delete All Comments from Word Documents using Java {#section4}

All comments of Word document can be deleted at once. You can follow the steps below for removing all comments:

1.  Open word docx file
2.  Collect all comments in the file
3.  Delete all comments

Following code snippet elaborates how to delete all comments from Word documents using Java:

{{< gist aspose-com-gists ef9c6086cf6e7030afda888475736625 "DeleteAllComments.java" >}}

## Conclusion

To sum up, we have learned how to add, insert, delete, or remove comments from word documents programmatically with Java. If you have any doubts or confusion then please contact us at [Free Support Forum][9].

## See Also

[Word Document (DOC/DOCX) to HTML Conversion using Java][10]




[1]: https://docs.fileformat.com/word-processing/docx/
[2]: https://docs.fileformat.com/word-processing/doc/
[3]: https://products.aspose.com/words/java
[4]: #section1
[5]: #section2
[6]: #section3
[7]: #section4
[8]: https://releases.aspose.com/
[9]: https://forum.aspose.com/c/words
[10]: https://blog.aspose.com/2020/07/15/word-document-doc-docx-to-html-conversion-using-java/





