---
title: 'Convert Excel Chart to Image and PDF Formats using C++'
date: Thu, 30 Aug 2018 18:52:24 +0000
draft: false
url: /2018/08/30/convert-chart-to-image-and-pdf-formats-using-aspose.cells-for-c-18.8/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-cpp-150x150.png" alt="">}}


Aspose Team is pleased to announce the release of [Aspose.Cells for C++ 18.8.0][1]. This release supports rendering charts to image and PDF formats. It also includes a number of fixes and other enhancements that further improve the overall stability of the API. Please check the detailed [release notes][2] in order to get an idea about what is new and what has been enhanced with this revision of Aspose.Cells for C++.

While you are downloading the API build to give it a try, here is a list of added features along with a few code snippets for quick testing.

## Excel Chart to Image in C++

Aspose.Cells for C++ supports to create a verity of MS Excel charts. The **Chart.toImage** method has a verity of overloads to support simple as well as advanced rendering. In order to demonstrate the usage of Aspose.Cells APIs to render the charts in image format, we will create a Column chart first and then render it to image format as per the following snippet.

```
// Create a new workbook
intrusive_ptr workbook = Factory::CreateIWorkbook();
// Get first worksheet which is created by default
intrusive_ptr worksheet = workbook->GetIWorksheets()->GetObjectByIndex(0);
// Adding sample values to cells
worksheet->GetICells()->GetObjectByIndex(new String("A1"))->PutValue(50);
worksheet->GetICells()->GetObjectByIndex(new String("A2"))->PutValue(100);
worksheet->GetICells()->GetObjectByIndex(new String("A3"))->PutValue(150);
worksheet->GetICells()->GetObjectByIndex(new String("B1"))->PutValue(4);
worksheet->GetICells()->GetObjectByIndex(new String("B2"))->PutValue(20);
worksheet->GetICells()->GetObjectByIndex(new String("B3"))->PutValue(50);
// Adding a chart to the worksheet
int chartIndex = worksheet->GetICharts()->Add(Aspose::Cells::Charts::ChartType::ChartType_Column, 5, 0, 20, 8);
// Accessing the instance of the newly added chart
intrusive_ptr chart = worksheet->GetICharts()->GetObjectByIndex(chartIndex);
// Adding SeriesCollection (chart data source) to the chart ranging from "A1" cell to "B3"
chart->GetNISeries()->Add(new String("A1:B3"), true);

// Output directory path
StringPtr outDir = new String("..\\Data\\02_OutputDirectory\\");
// Path of output image file
StringPtr outputChartImage = outDir->StringAppend(new String("out1image.png"));
// Saving the chart to image file
chart->ToImage(outputChartImage, Aspose::Cells::System::Drawing::Imaging::ImageFormat::GetPng()); 
```

See the document on how to [convert a chart to image format][3] for your reference.

## Excel Chart to PDF in C++

In order to render the chart to PDF format, the Aspose.Cells APIs have exposed the **Chart.ToPdf** method with ability to store the resultant PDF on disc path or Stream.

```
// Path of output pdf file
StringPtr outputPdfFile = outDir->StringAppend(new String("out1pdf.pdf"));
// Saving chart to PDF
chart->ToPdf(outputPdfFile); 
```

See the document on how to [convert a chart to PDF file format][4] for your reference.

## Aspose.Cells for C++ Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for C++ API][5].
*   [Aspose.Cells for C++ Downloads][6].
*   [Aspose.Cells for C++ Documentation][7] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells Product Family Forum][8] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][9] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Cells for C++ API by posting your suggestions and concerns in the Aspose.Cells support forum.




[1]: https://www.nuget.org/packages/Aspose.Cells.Cpp/18.8.0
[2]: https://docs.aspose.com/display/cellscpp/Aspose.Cells+for+CPP+18.8+Release+Notes
[3]: https://docs.aspose.com/display/cellscpp/Chart+Rendering#ChartRendering-RenderingChartstoImages
[4]: https://docs.aspose.com/display/cellscpp/Chart+Rendering#ChartRendering-RenderingCharttoPDF
[5]: https://products.aspose.com/cells/cpp
[6]: https://downloads.aspose.com/cells/cpp
[7]: https://docs.aspose.com/display/cellscpp/Home
[8]: https://forum.aspose.com/c/cells
[9]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/




