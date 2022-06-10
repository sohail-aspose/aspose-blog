---
title: 'Detect OOXML File Format using Aspose.Cells for Java 19.2'
date: Sat, 30 Mar 2019 05:33:56 +0000
draft: false
url: /2019/03/30/detect-ooxml-file-format-using-aspose.cells-for-java-19.2/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-java.jpg" alt="">}}


The wait is over! The latest version of [Aspose.Cells for Java][1] is here. I'm going to walk you through all the exciting features, improvements, and fixes. Don't worry, you'll know where you can find everything related to this latest update in a bit, but for now, let's talk about this new version and see [what the team has been up to][2]! Shall we?

Microsoft Excel supports a feature to insert a row using one of the three different options. The objective of these options is to adopt settings from other rows. These three options include the following:

*   **Format Same as Above** (copy formatting from the above row)
*   **Format Same as Below** (copy formatting from the row below)
*   **Clear Formatting** (add new row but without any formatting)

You can also see these three options in the following screenshot:



{{< figure align=center src="images/InsertTypes-2.png" alt="Insert a row with one of the three formatting options">}}


The good news is, using [Aspose.Cells for Java 19.2][3] and onwards, you can use this feature in your code as well. You can programmatically create new rows with the specified formatting option. Now, you must be wondering, hmm, how exactly do I do that in my Java application? Here is a code sample for you to do just that along the [documentation to insert row with formatting][4]:

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-RowsAndColumns-InsertingARowWithFormatting-1.java" >}}

There was a high demand, from you guys, that just like Excel, [Aspose.Cells][5] supports [replacing special characters while opening a CSV file][6]. So, we're very excited to break the news that this feature is now supported in the API. Just have a look at the below example to see how easy it is to achieve this with Aspose.Cells for Java.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-LoadingSavingConvertingAndManaging-OpeningCSVFilesAndReplacingInvalidCharacters-1.java" >}}

As you must already have some idea that Office Open XML, which is also known as OOXML or Microsoft Open XML (MOX), is a very common format used for files. It is an XML-based format developed by Microsoft for representing office documents like spreadsheets, charts, presentations, and word processing documents. Aspose.Cells already allowed to open and detect type of this format. But now, our team has gone a step forward and supported to [detect type of encrypted OOXML files][7]. Check out the sample code below:

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-TechnicalArticles-DetectFileFormatOfEncryptedFiles-1.java" >}}

## 3 Major Enhancements in Aspose.Cells for Java

In addition to the features highlighted above, you can now improve your products with the help of these 4 major improvements:

*   API Reference (JavaDocs) has been updated along with improving the process of _**attaching JavaDocs to our API in the IDEs**_. Now, you should be able to utilize the API up to its full capacity with the help of the updated [API Reference of Aspose.Cells for Java][8].
*   Based on our user's demand to **a_ccess all the hyperlinks in a range of cells and delete_** anyone if required, we have supported this feature in this release. You can use [Range.getHyperlinks()][9] to get all the hyperlinks from a range, and then delete those using [Hyperlink.delete()][10] method.
*   A small integer variable was available to get the number of cells in the Worksheet. In the newer versions of Excel, when the number of cells was increased, it was not possible to get a large number of cells. This shortcoming is corrected by providing appropriate data type which can be evaluated using [sample code in this topic][11].

## A Few Minor Improvements in the API

The following is a list of some minor changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible changes made to Aspose.Cells for Java:  

*   Added **ListObject.AlternativeDescription** and **ListObject.AlternativeText** properties to get and set the alternative text and description of the table
*   Added **Line.ThemeColor property** to get and set the theme color of the line
*   Added **Mode3d** and **MsoModel3dFormat** class which encapsulates the object that represents a single 3D model in a spreadsheet
*   Added **ImageType.Gltf enum** which represents the type of 3D model

Alright! by now, you must have got a pretty good idea of what we have been working on, since the last release, to help you improve and speed up your development efforts. Well, where you go from here on? The choice is yours!

You can take a little break and come back for more, or if you have already taken your cup of coffee, then let's talk further about this release in our [forums][12]. You can also check out [API examples at GitHub][13], or go ahead and download the [latest version of Aspose.Cells for Java][14] to play with it. And stay tuned for more exciting features and news!




[1]: https://products.aspose.com/cells/java
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+19.2+Release+Notes
[3]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/19.2/
[4]: https://docs.aspose.com/display/cellsjava/Inserting+and+Deleting+Rows+and+Columns#InsertingandDeletingRowsandColumns-InsertaRowwithFormatting
[5]: https://products.aspose.com/cells
[6]: https://docs.aspose.com/display/cellsjava/Opening+Files+with+Different+Formats#OpeningFileswithDifferentFormats-OpeningCSVfilesandreplacinginvalidcharacters
[7]: https://docs.aspose.com/display/cellsjava/Detect+File+Format+of+Encrypted+Office+Open+XML+-+OOXML+Files
[8]: https://apireference.aspose.com/java/cells
[9]: https://apireference.aspose.com/java/cells/com.aspose.cells/range#Hyperlinks
[10]: https://apireference.aspose.com/java/cells/com.aspose.cells/hyperlink#delete()
[11]: https://docs.aspose.com/display/cellsjava/Count+number+of+cells+in+the+Worksheet
[12]: https://forum.aspose.com/c/cells
[13]: https://github.com/aspose-cells/Aspose.Cells-for-Java
[14]: https://downloads.aspose.com/cells/java




