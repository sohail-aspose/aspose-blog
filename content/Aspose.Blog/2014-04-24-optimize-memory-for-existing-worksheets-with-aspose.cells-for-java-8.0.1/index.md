---
title: 'Optimize Memory for Existing Worksheets with Aspose.Cells for Java 8.0.1'
date: Thu, 24 Apr 2014 08:55:02 +0000
draft: false
url: /2014/04/24/optimize-memory-for-existing-worksheets-with-aspose.cells-for-java-8.0.1/
author: Babar Raza
summary: ''
tags: ['Aspose.Cells for Java', 'Babar Raza', 'Optimize Memory for Excel Worksheets in Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java logo">}}


Aspose.Cells for Java 8.0.1 has been released, and we are pleased to announce that this month’s release has brought many useful improvements and features. You can immediately download the latest Aspose.Cells for Java release from the [download section][1], and start exploring the features & enhancements we've added.

Here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download page in the link above.

## Optimize Memory for Existing Worksheets

With [release 8.0.0][2], Aspose.Cells for Java provided memory optimization settings for newly created worksheets by exposing the setMemorySetting method for the Workbook.Settings class. The previously provided approach was useful for minimizing the overall memory cost while working with existing large Excel spreadsheets containing huge data sets.

With this release, we have enhanced this feature for existing worksheets by exposing a similar property for the Cells class. Now you may use setMemorySetting method provided by the Cells class to cope with the memory issues for situations where large data sets have to be built in memory. The setMemorySetting method accepts a parameter of type MemorySetting with the default value NORMAL. In order to properly utilize this newly introduced feature, memory optimization settings have to be explicitly specified for existing worksheets. Please check the detailed technical article on how to [optimize the memory while working with large data sets][3].

## Enhancements for the License Class

The Aspose.Cells for Java API has enhanced the licensing mechanism with the release of 8.0.1. Now when a license file name is passed to the License.setLicense method without specifying in which directory it resides, the API will search for the license in the same folder that the Aspose.Cells Jar is in. This enhancement was made in order to meet the standards set by Aspose components.

## Identify Corrupted Excel Files

We have also enhanced the CellsException class to identify potentially damaged or corrupted files when loaded with the Workbook constructor. Previously, the API could load any corrupted file but would sometimes throw an error when saving it after performing manipulation. With the new enhancements integrated, Aspose.Cells for Java API now throws an error of type CellsException whenever it encounters a damaged file.

The CellsException class can also handle irrelevant file formats (other than spreadsheets) while loading them into an instance of Workbook.

## Bug Fixes

Aspose.Cells for Java 8.0.1 has provided fix for several important issues, such as a couple of problems related to the PDF rendering engine, rendering & manipulating charts, retrieving & removing OleObjects. Last but not least, we have just integrated an overhaul of our existing formula engine which improves the overall performance as well as the accuracy of results when working with Excel formulas.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Cells support forum][4] for a chat.




[1]: https://downloads.aspose.com/cells/java
[2]: https://blog.aspose.com/2014/04/01/memory-usage-optimized-and-set-the-creation-time-in-the-generated-pdf-using-aspose.cells-for-java-8.0.0
[3]: http://docs.aspose.com/display/cellsjava/Optimizing+Memory+Usage+while+Working+with+Big+Files+having+Large+Datasets
[4]: http://forum.aspose.com




