---
title: 'Protect VBA Project of Excel with Password using Java'
date: Tue, 02 May 2017 13:21:35 +0000
draft: false
url: /2017/05/02/protect-vba-project-of-excel-with-password-using-java/
author: Mshakeel Faiz
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


Aspose team is pleased to announce the release of [Aspose.Cells for Java 17.4.0][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the API. Please check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. Here is a look at the major features in this release.

## Protect VBA Project of Excel Workbook with Password

Aspose.Cells now supports the feature of protecting the VBA (Visual Basic for Applications) Project of Excel Workbook and locking it for viewing. Besides, you can also find if the existing VBA project is already protected or locked for viewing. Please see these articles for a reference.

*   [Password Protect the VBA Project of Excel Workbook][3]
*   [Check if VBA Project is Protected and Locked for Viewing][4]
*   [Find out if VBA Project is Protected][5]

The following snippet demonstrates how to protect your Excel Workbook VBA Project dynamically using Aspose.Cells and lock it for viewing.

```
//Load your source Excel file.
Workbook wb = new Workbook(dirPath + "samplePasswordProtectVBAProject.xlsm");
  
//Access the VBA project of the workbook.
VbaProject vbaProject = wb.getVbaProject();
  
//Lock the VBA project for viewing with password.
vbaProject.protect(true, "11");
  
//Save the output Excel file.
wb.save(dirPath + "outputPasswordProtectVBAProject.xlsm");
```

## Specifying Sort Warning While Sorting Data

Aspose.Cells already supports Data Sorting, however earlier you could not specify that you want to sort your textual data as numerical data. For this purpose, Aspose.Cells implemented the **DataSorter.SortAsNumber** property. Whenever you sort textual data that looks like a number, MS-Excel shows this warning. **DataSorter.SortAsNumber** property implements this MS-Excel warning.



{{< figure align=center src="images/sort-textual-data-as-numbers-300x208.png" alt="">}}


Please see this article for more help relating to this topic.

*   [Specifying Sort Warning While Sorting Data][6]

## Specifying DBNum Custom Pattern Formatting

Aspose.Cells supports the **DBNum** custom pattern formatting. For example, if your cell value is **123** and you specify its custom formatting as **\[DBNum2\]\[$-804\]General** then it will be displayed like **壹佰贰拾叁**. You can specify custom formatting of your cell using Cell.getStyle() and Style.setCustom() methods.

*   [Specifying DBNum Custom Pattern Formatting][7]

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][8].
*   [Aspose.Cells for Java Download Section][9].
*   [Aspose.Cells for Java Documentation][10] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][11] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][12] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][13] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/cells/java
[2]: https://docs.aspose.com/cells/java/aspose-cells-for-java-17-4-0-release-notes/
[3]: https://docs.aspose.com/cells/java/password-protect-the-vba-project-of-excel-workbook/
[4]: https://docs.aspose.com/cells/java/check-if-vba-project-is-protected-and-locked-for-viewing/
[5]: https://docs.aspose.com/cells/java/find-out-if-vba-project-is-protected/
[6]: https://docs.aspose.com/cells/java/specifying-sort-warning-while-sorting-data/
[7]: https://docs.aspose.com/cells/java/specifying-dbnum-custom-pattern-formatting/
[8]: https://products.aspose.com/cells/java
[9]: https://downloads.aspose.com/cells/java
[10]: https://docs.aspose.com/cells/java
[11]: https://apireference.aspose.com/java/cells
[12]: http://forum.aspose.com
[13]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[14]: https://github.com/asposecells/Aspose_Cells_Java




