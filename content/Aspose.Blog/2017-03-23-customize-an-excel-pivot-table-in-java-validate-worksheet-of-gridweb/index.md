---
title: 'Customize an Excel Pivot Table and Validate the Entire Worksheet of GridWeb in Java'
date: Thu, 23 Mar 2017 18:30:49 +0000
draft: false
url: /2017/03/23/customize-an-excel-pivot-table-in-java-validate-worksheet-of-gridweb/
author: Imran Rafique
summary: ''
tags: ['Client-side Script for GridWeb', 'Entire Worksheet of GridWeb', 'Excel Pivot Table', 'Validate Worksheet']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


The Aspose team is pleased to announce the availability of [the next version 17.3.0 of Aspose.Cells for Java API][1]. With this release, we have opened up a new set of scenarios for developers, which they can utilize in their Java applications. It covers the new feature to enhance the API control over the pivot tables. Developers can retrieve and set globalization settings of a pivot table. They can also call the client-side script on the page change event of GridWeb control. GridWeb has support to validate the entire Excel worksheet instead of the updated cells. All the regular bug fixes and enhancements are also included. We recommend our clients [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. For details on API fixes, please visit the product [Release Notes][3] section for this new version. The release notes page highlights any implication made to the public API as well as any non-backward compatible change. Let's go into the more details of each feature one by one.

## Customizing a Pivot Table by Using Globalization Settings

Using Aspose.Cells API, developers can apply various filters to build the corresponding pivot table. After they create a pivot table report and have added the fields that they require, they often want to enhance the layout and format of the report to improve readability and to make it more attractive. To achieve this, Aspose.Cells API allows developers to customize the globalization settings of a pivot table to deal with such scenarios. They can customize the Pivot Total, Sub Total, Grand Total, All Items, Multiple Items, Column Labels, Row Labels, Blank Values text as per the requirements.

Developers can derive a class from the base GlobalizationSettings class. GlobalizationSettings class has various methods to further enhance the Pivot Total, Sub Total, Grand Total, All Items, Multiple Items, Column Labels, Row Labels and Blank Values text. This article shows a code example which works with the layout and format of a report: [Customize Globalization Settings for Pivot Table][4]

## Call a Client Side Script on Page Change Event of GridWeb

Aspose.Cells for Java includes an independent web-based grid control (com.aspose.cells.GridWeb) which is designed to work with the web applications. Developers can load an existing Excel file into its grid matrix, manipulate it and save it back. The GridWeb control can hold data in multiple pages via its paging feature. Developers might require to call a client side script on page index change event of GridWeb. This feature covers various scenarios. Developers may require to display the page number in their Java applications, so they can call client side script to get the page number. To achieve this, EnablePaging property of the GridWeb should be set as True. This article shows a code example which uses the OnPageChangeClientFunction property of GridWeb control to display the page number: [Execute client side function on GridWeb page change][5]

## Validate the Entire Worksheet of GridWeb

In the past, GridWeb control was validating the updated cells and not validating the entire Excel worksheet. Using the recent version 17.3.0 of Aspose.Cells API, developers can now validate the entire worksheet on client side before the GridWeb requests to the server. They need to set the needValidateall variable inside the acwmain.js to true. This article explains about how to validate the entire Excel worksheet of GridWeb: [Validate entire worksheet instead of only the updated cells][6]

## Other Enhancements and Fixes

Aspose.Cells for Java API improvement work never stops because we are listening to the requests of our clients and gradually integrating their needs. Aspose team has made an important enhancement along with other behind the scenes enhancements. It is about to set the long string literals inside the formula.

Several other bug fixes make the API more reliable and functional. It brings quality in rendering the borders of the cells while saving an Excel in other supported formats. The rendering speed of charts has been increased, especially with large data sets. The formula calculation engine is also further enhanced in the new release.

## Public API Changes

This revision of Aspose.Cells for Java has made some changes to the Public API. A few of the worth mentioning changes are listed here:

*   GlobalizationSettings.getPivotTotalName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.getPivotGrandTotalName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.getMultipleItemsName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.getAllName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.getColumnLablesName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.getRowLablesName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.getEmptyDataName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.getSubTotalName(PivotFieldSubtotalType subTotalType) method is added to the GlobalizationSettings class.
*   OnPageChangeClientFunction property is added to the GridWeb Control.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][7].
*   [Aspose.Cells for Java Download Section][8].
*   [Aspose.Cells for Java Documentation][9] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][10] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][11] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][12] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][13] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/diagram/java/new-releases/aspose.diagram-for-java-17.3.0/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/cells/java/aspose-cells-for-java-17-3-0-release-notes/
[4]: https://docs.aspose.com/cells/java/customize-globalization-settings-for-pivot-table/
[5]: https://docs.aspose.com/cells/java/execute-client-side-function-on-gridweb-page-change/
[6]: https://docs.aspose.com/cells/java/validate-entire-worksheet-instead-of-only-the-updated-cells/
[7]: https://products.aspose.com/cells/java/
[8]: https://downloads.aspose.com/cells/java/
[9]: https://docs.aspose.com/cells/java/
[10]: https://apireference.aspose.com/cells/java/
[11]: https://forum.aspose.com/
[12]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[13]: https://github.com/asposecells/Aspose_Cells_Java




