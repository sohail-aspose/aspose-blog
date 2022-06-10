---
title: 'Access and Update Portion of Rich Text in Excel using Java'
date: Mon, 02 Nov 2015 10:04:10 +0000
draft: false
url: /2015/11/02/set-link-target-type-for-html-conversion-access-update-portion-of-rich-text-and-detect-if-vbaproject-is-signed-with-aspose.cells-for-java-8.6.1/
author: Babar Raza
summary: ''
tags: ['Aspose.Cells', 'Babar Raza', 'Excel File Formal APIs', 'Hyperlink Target Type', 'Rich Text', 'Spreadsheet Creator', 'Spreadsheet Manipulator', 'VBA Projects']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


Aspose.Cells for Java API has been upgraded to 8.6.1, and we are pleased to announce, this month's release contains many useful features and improvements along with some critical bug fixes. Please refer to the release notes of [Aspose.Cells for Java 8.6.1][1] for a full list of enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the [Public API Changes][2] section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Access and Update Portion of Rich Text in Excel using Java

Aspose.Cells for Java API provides easy to use a mechanism to access the format related properties of each character from a cell containing Rich Text. The API has exposed the getCharacters & setCharacters methods for the Cell class that allows to access & update the portion of the Rich Text in a cell. The Cell.getCharacters method returns an array of FontSetting objects where each object represents the styling of an individual character. The Cell.setCharacters method also accepts an array of FontSetting objects to set the styling for individual characters of a cell.

The following sample code explains the usage of Cell.getCharacters & Cell.setCharacters methods to access and manipulate the styling of Rich Text.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-AccessAndUpdatePortions-AccessAndUpdatePortions.java" >}}

## Set Link Target Type for HTML Conversion

Aspose.Cells APIs are capable of converting all supported spreadsheet formats to HTML with the highest fidelity. The conversion process is efficient as well as configurable, that is; users can customize the HTML generation process as per their application requirement. Aspose.Cells APIs have exposed the HtmlSaveOptions class that is mainly responsible for the conversion process and provides a vast array of features to influence the HTML generation.

This release of Aspose.Cells for Java API has exposed an enumeration namely HtmlLinkTargetType along with a new property HtmlSaveOptions.LinkTargetType that together allows to set the target type for the links in spreadsheet while conversion to HTML format. The possible values of the HtmlLinkTargetType enumeration are as follow where the default value is SELF.

*   HtmlLinkTargetType.BLANK: Opens the linked document/page in a new window or tab.
*   HtmlLinkTargetType.PARENT: Opens the linked document/page in parent frame.
*   HtmlLinkTargetType.SELF: Opens the linked document/page in the same frame where the link was clinked.
*   HtmlLinkTargetType.TOP: Opens the linked document/page in the full body of the window.

Here is the simplest usage scenario of newly exposed APIs to [set the link target type][3].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-ChangeHTMLLinkTargetType-ChangeHTMLLinkTargetType.java" >}}

## Detect If VbaProject is Signed

Aspose.Cells for Java 8.6.1 has exposed the VbaProject.isSigned property that can be used to test if a VbaProject in a Workbook is signed or not. Boolean type property returns true if the project is signed.

Following is the simple usage scenario.

```
//Load a spreadsheet
Workbook workbook = new Workbook(inputFilePath);

//Retrieve the VbaProject from the Workbook
VbaProject project = workbook.getVbaProject();

//Test if VbaProject is signed
if (project.isSigned())
{
    System.out.println("VBA Project is Signed");
}
else
{
	System.out.println("VBA Project is not Signed");
}

```

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Exposed RangeCollection.add method that can be used to add Range objects to the collection of ranges for a particular Worksheet.
*   Exposed an overload of the VbaModuleCollection.remove method that can now accept an instance of Worksheet to remove all the VBA modules associated with the specified Worksheet.
*   Modified Cell.getFormatConditions method that now returns an array of type FormatConditionCollection.
*   Enhanced the PDF & image rendering engines to properly handle the long hyphens.
*   Provided support for WebQuery type of external data source.
*   Handled calculation problem while calculating formula based on Named Range.
*   Improved the chart rendering for PDF & image formats.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Cells for Java API][4].
*   [Download Aspose.Cells for Java][5].
*   [Aspose.Cells for Java online documentation][6] – help documentation and API reference documents.
*   [Aspose.Cells Product Family Forum][7] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable blog Subscription][8] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java
[2]: https://docs.aspose.com/display/cellsjava/Migrating+from+Earlier+Versions+of+Aspose.Cells
[3]: https://docs.aspose.com/display/cellsjava/Change+the+HTML+Link+Target+Type
[4]: https://products.aspose.com/cells/java
[5]: https://downloads.aspose.com/cells/java
[6]: http://docs.aspose.com/display/cellsjava/home
[7]: https://forum.aspose.com/
[8]: https://blog.aspose.com/
[9]: https://github.com/asposecells/Aspose_Cells_Java




