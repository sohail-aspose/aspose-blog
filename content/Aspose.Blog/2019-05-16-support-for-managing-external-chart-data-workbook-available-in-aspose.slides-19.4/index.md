---
title: 'Manage Chart Data in External Workbook using C#, Java and C++'
date: Thu, 16 May 2019 17:44:41 +0000
draft: false
url: /2019/05/16/support-for-managing-external-chart-data-workbook-available-in-aspose.slides-19.4/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png) Good news guys! I like to share experience after using latest Aspose.Slides 19.4 which has been enriched with improved chart data support features. The good thing about Aspose.Slides is that it has a monthly release where .NET, Java, Android via Java and C++ based APIs are published together. So, whats available in .NET based API is also available for Java, Android via Java and C++ based APIs. This way the users feels comfortable with API they are using and with same features available across the board.

In the following sections, I am going to give you a walk through of what new features have been included and what improvements have been carried in API.

## Work with Chart Data in External Workbook

As all of you may be aware of the fact MSO (Microsoft Office) charts support is available in PowerPoint that display the chart in slides but maintain its data in chart data workbook. Usually, the chart data workbook is embedded inside PowerPoint presentation and linked with its respective chart. The other option is to maintain external workbook to hold chart data by linking chart with that external workbook.

Good news is that Aspose.Slides has also introduced the support for managing external chart data workbook in this new release. You can create an external chart data workbook for existing chart in presentation by accessing it chart data workbook stream and saving that as file. Here's how you can use this feature.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Charts-CreateExternalWorkbook-CreateExternalWorkbook.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Slides-Charts-CreateExternalWorkbook-CreateExternalWorkbook.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-CreateExternalWorkbook-CreateExternalWorkbook.cpp" >}}

You can also set the path to external workbook for existing chart. However, while doing so, you need to ensure that chart data is in accordance with chart categories and series. Otherwise, you need to point the chart categories and series data to respective cells in new external chart workbook. Here's how you can use this feature:

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Charts-SetExternalWorkbook-SetExternalWorkbook.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Slides-Charts-SetExternalWorkbook-SetExternalWorkbook.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-SetExternalWorkbook-SetExternalWorkbook.cpp" >}}

Moreover, you can also modify the chart data in workbook as well. Here's how you can use this feature:

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Charts-EditChartDatainExternalWorkbook-EditChartDatainExternalWorkbook.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Slides-Charts-EditChartDatainExternalWorkbook-EditChartDatainExternalWorkbook.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-EditChartDatainExternalWorkbook-EditChartDatainExternalWorkbook.cpp" >}}

Wait, there's many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][2]

When time allows you can check out API [examples at Github][3], talk about this release and other API related issues in our [forum][4].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png "Aspose.Slides or .NET logo"
[2]: https://docs.aspose.com/display/slidesnet/Aspose.Slides+for+.NET+19.4+Release+Notes
[3]: https://github.com/aspose-slides/
[4]: https://forum.aspose.com/c/slides




