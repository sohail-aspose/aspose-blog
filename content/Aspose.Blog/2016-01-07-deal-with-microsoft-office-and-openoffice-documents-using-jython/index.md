---
title: 'Deal with Microsoft Office and OpenOffice Documents using Jython'
date: Thu, 07 Jan 2016 10:56:47 +0000
draft: false
url: /2016/01/07/deal-with-microsoft-office-and-openoffice-documents-using-jython/
author: Masood Anwer
summary: ''
tags: ['Examples', 'Jython', 'MSWord', 'OpenOffice']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose_words-for-java.png" alt="">}}




{{< figure align=center src="images/jython.png" alt="">}}


We are pleased to announce “[Aspose.Words Java for Jython][1]”, a new project for Jython developers. Project is aimed to provide useful examples for [Jython][2] developers who want to utilize [Aspose.Words for Java API][3] in their Jython applications to deal with Microsoft Word and OpenOffice documents.

## Download, Installation, and Usage

Please check the links below to find instructions on downloading, installing and using Aspose.Words Java for Jython.

*   Downloads and Installation

OR

You can download the latest version from:

*   [CodePlex][4]
*   [GitHub][5]

## Quick Start Tutorial

The following example demonstrates how you can create HelloWorld document.

```
from asposewords import Settings
from com.aspose.words import Document
from com.aspose.words import DocumentBuilder

class HelloWorld:

    def __init__(self):
        dataDir = Settings.dataDir + 'quickstart/'

        doc = Document()

        builder = DocumentBuilder(doc)
        builder.writeln('Hello World!')

        doc.save(dataDir + 'HelloWorld.docx')

        print "Document saved."

if __name__ == '__main__':        
    HelloWorld()
```

## Aspose.Words Java for Jython Examples

*   [Check Format in Jython][6]
*   [Convert Document to Other Formats in Jython][7]
*   [Load Plain Text (TXT) File in Jython][8]
*   [Working with Digital Signatures in Jython][9]

*   [Append Documents in Jython][10]
*   [Apply License in Jython][11]
*   [Convert Document to PDF in Jython][12]
*   [Find And Replace in Jython][13]
*   [Hello World in Jython][14]
*   [Load And Save To Disk in Jython][15]
*   [Load And Save To Stream in Jython][16]
*   [Simple Mail Merge in Jython][17]
*   [Update Fields in Jython][18]
*   [Working With Nodes in Jython][19]

*   [Joining And Appending in Jython][20]
*   [Working With Bookmarks in Jython][21]
*   [Working With Comments in Jython][22]
*   [Working With Documents in Jython][23]
*   [Working With Fields in Jython][24]
*   [Working With Styles in Jython][25]
*   [Working With Tables in Jython][26]

*   [Render Shapes in Jython][27]
*   [Save Document as a Multipage TIFF in Jython][28]

## Aspose.Words Java for Jython Documentation

Aspose.Words Java for Jython [Documentation][29] is available to guide developers to get familiar with the specific resources and operations within the Aspose.Words Java for Jython.

## Start a Free Trial Today

Start a free trial today – all you need is to sign up with Aspose. Once you have signed up, you are ready to try powerful file processing features offered by Aspose file format APIs.




[1]: https://docs.aspose.com/
[2]: http://www.jython.org/
[3]: https://products.aspose.com/words/java
[4]: https://docs.aspose.com/
[5]: https://github.com/asposewords/Aspose_Words_Java/releases/tag/Aspose.Words_Java_for_Jython-v1.0.0
[6]: https://docs.aspose.com/words/java/check-format-in-jython/
[7]: https://docs.aspose.com/words/java/convert-document-to-other-formats-in-jython/
[8]: https://docs.aspose.com/words/java/load-plain-text-txt-file-in-jython/
[9]: https://docs.aspose.com/words/java/working-with-digital-signatures-in-jython/
[10]: https://docs.aspose.com/words/java/append-documents-in-jython/
[11]: https://docs.aspose.com/words/java/apply-license-in-jython/
[12]: https://docs.aspose.com/words/java/convert-document-to-pdf-in-jython/
[13]: https://docs.aspose.com/words/java/find-and-replace-in-jython/
[14]: https://docs.aspose.com/words/java/hello-world-in-jython/
[15]: https://docs.aspose.com/words/java/load-and-save-to-disk-in-jython/
[16]: https://docs.aspose.com/words/java/load-and-save-to-stream-in-jython/
[17]: https://docs.aspose.com/words/java/simple-mail-merge-in-jython/
[18]: https://docs.aspose.com/words/java/update-fields-in-jython/
[19]: https://docs.aspose.com/words/java/working-with-nodes-in-jython/
[20]: https://docs.aspose.com/words/java/joining-and-appending-in-jython/
[21]: https://docs.aspose.com/words/java/working-with-bookmarks-in-jython/
[22]: https://docs.aspose.com/words/java/working-with-comments-in-jython/
[23]: https://docs.aspose.com/words/java/working-with-documents-in-jython/
[24]: https://docs.aspose.com/words/java/working-with-fields-in-jython/
[25]: https://docs.aspose.com/words/java/working-with-styles-in-jython/
[26]: https://docs.aspose.com/words/java/working-with-tables-in-jython/
[27]: https://docs.aspose.com/words/java/render-shapes-in-jython/
[28]: https://docs.aspose.com/words/java/save-document-as-a-multipage-tiff-in-jython/
[29]: https://docs.aspose.com/words/java/aspose-words-java-for-jython/




