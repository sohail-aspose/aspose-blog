---
title: 'Convert MS Excel Spreadsheet to PDF and Image Formats using Aspose.Cells for C++ v18.5'
date: Fri, 08 Jun 2018 09:02:29 +0000
draft: false
url: /2018/06/08/convert-ms-excel-spreadsheet-to-pdf-and-image-formats-using-aspose.cells-for-c-v18.5/
author: Amjad Sahi
summary: ''
tags: ['Convert Excel to PDF or Images in Cpp', 'Excel to PNG or JPG', 'XLS to PDF', 'XLSX to PDF']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-cpp-150x150.png" alt="">}}


Aspose Team is pleased to announce the release of [Aspose.Cells for C++ 18.5.0][1]. This release supports converting MS Excel spreadsheets to PDF file format and rendering worksheets/workbook to image formats, the two most valuable features demanded by many developers. It also includes other enhancements and fixes that further improve the overall stability of the API. Please check the detailed [release notes][2] in order to get an idea about what is new and what has been enhanced with this revision of Aspose.Cells for C++.

While you are downloading the API build to give it a try, here is a list of added features along with a few code snippets for quick testing.

## Converting Excel Workbook to PDF

As we know, PDF files are widely used to exchange documents between organizations, government sectors, and individuals. It is a standard document format and software developers are often asked to find a way to convert Microsoft Excel files into PDF documents. Aspose.Cells for C++ now supports converting Excel files to PDF and maintains good visual fidelity in the conversion.

The following code demonstrates the use of Aspose.Cells for C++ API to convert an Excel spreadsheet to the PDF file format.

```
// Source directory path.
StringPtr srcDir = new String("..\\Data\\01_SourceDirectory\\");
 
// Output directory path.
StringPtr outDir = new String("..\\Data\\02_OutputDirectory\\");
 
// Path of input Excel file
StringPtr sampleConvertExcelWorkbookToPDF = srcDir->StringAppend(new String("sampleConvertExcelWorkbookToPDF.xlsx"));
 
// Path of output Pdf file
StringPtr outputConvertExcelWorkbookToPDF = outDir->StringAppend(new String("outputConvertExcelWorkbookToPDF_DirectConversion.pdf"));
 
// Load the sample Excel file.
intrusive_ptr workbook = Factory::CreateIWorkbook(sampleConvertExcelWorkbookToPDF);
 
// Save the Excel Document in PDF format
workbook->Save(outputConvertExcelWorkbookToPDF, SaveFormat_Pdf);
```

See the document on how to [Convert Excel Workbook to PDF][3] for your reference.

## Converting Worksheet to Different Image Formats

You might need to present worksheets as series of images. For example, you require to use an image of a worksheet in an application or web page. You might want to insert an image into a Microsoft Word document, a PDF file, a PowerPoint presentation or some other document type. Aspose.Cells for C++ now supports converting Excel worksheets to images. Several image formats are supported, for example BMP, PNG, GIF, JPG, JPEG, TIFF, EMF.

The following code demonstrates the use of Aspose.Cells for C++ API to convert worksheet to image format.

```
// Source directory path.
StringPtr srcDir = new String("..\\Data\\01_SourceDirectory\\");
 
// Output directory path.
StringPtr outDir = new String("..\\Data\\02_OutputDirectory\\");
 
// Path of input Excel file.
StringPtr sampleConvertingWorksheetToDifferentImageFormats = srcDir->StringAppend(new String("sampleConvertingWorksheetToDifferentImageFormats.xlsx"));
 
// Create an empty workbook.
intrusive_ptr workbook = Factory::CreateIWorkbook(sampleConvertingWorksheetToDifferentImageFormats);
 
// Access first worksheet.
intrusive_ptr worksheet = workbook->GetIWorksheets()->GetObjectByIndex(0);
 
// Create image or print options object.
intrusive_ptr imgOptions = Factory::CreateIImageOrPrintOptions();
 
// Specify the image format.
imgOptions->SetImageFormat(Aspose::Cells::System::Drawing::Imaging::ImageFormat::GetPng());
 
// Specify horizontal and vertical resolution
imgOptions->SetHorizontalResolution(200);
imgOptions->SetVerticalResolution(200);
 
// Render the sheet with respect to specified image or print options.
intrusive_ptr sr = Factory::CreateISheetRender(worksheet, imgOptions);
 
// Get page count.
Aspose::Cells::System::Int32 pageCount = sr->GetPageCount();
 
// Create string builder object for string concatenations.
intrusive_ptr sb = new Aspose::Cells::System::Text::StringBuilder();
 
// Render each page to png image one by one.
for (int i = 0; i < pageCount; i++)
{
    // Clear string builder and create output image path with string concatenations.
    sb->Clear();
    sb->Append(outDir);
    sb->Append((StringPtr)new String("outputConvertingWorksheetToImagePNG_"));
    sb->Append(i);
    sb->Append((StringPtr)new String(".png"));
 
    // Get the output image path.
    StringPtr outputPNG = sb->ToString();
 
    // Convert worksheet to png image.
    sr->ToImage(i, outputPNG);
}
```

See the document on how to [convert worksheet to different image formats][4] for your reference.

## Aspose.Cells for C++ Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for C++ API][5].
*   [Aspose.Cells for C++ Downloads][6].
*   [Aspose.Cells for C++ Documentation][7] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells Product Family Forum][8] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][9] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Cells for C++ API by posting your suggestions and concerns in the Aspose.Cells support forum.




[1]: https://www.nuget.org/packages/Aspose.Cells.Cpp/18.5.0
[2]: https://docs.aspose.com/display/cellscpp/Aspose.Cells+for+CPP+18.5+Release+Notes
[3]: https://docs.aspose.com/display/cellscpp/Convert+Excel+Workbook+to+PDF
[4]: https://docs.aspose.com/display/cellscpp/Converting+Worksheet+to+Different+Image+Formats
[5]: https://products.aspose.com/cells/cpp
[6]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[7]: https://docs.aspose.com/display/cellscpp/Home
[8]: https://forum.aspose.com/c/cells
[9]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/




