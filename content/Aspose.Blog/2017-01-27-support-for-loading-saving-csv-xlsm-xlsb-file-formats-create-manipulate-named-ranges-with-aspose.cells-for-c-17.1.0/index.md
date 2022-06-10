---
title: 'Support for Loading &amp; Saving CSV, XLSM &amp; XLSB File Formats, Create &amp; Manipulate Named Ranges with Aspose.Cells for C++ 17.1.0'
date: Fri, 27 Jan 2017 05:54:34 +0000
draft: false
url: /2017/01/27/support-for-loading-saving-csv-xlsm-xlsb-file-formats-create-manipulate-named-ranges-with-aspose.cells-for-c-17.1.0/
author: Babar Raza
summary: ''
tags: ['API to Convert Spreadsheets', 'API to Manipulate Spreadsheets', 'C++ Excel', 'Cpp Library for Excel', 'Named Ranges']
categories: ['Aspose.Cells Product Family']
---

Aspose Team is pleased to announce the release of [Aspose.Cells for C++ 17.1.0][1]. This release includes many new features and enhancements that further improve the overall feature set of the API. Please check the detailed release notes in order to get an idea about what is new and what has been enhanced with this revision of Aspose.Cells for C++. If you are planning to upgrade the API from any previous version, we strongly suggest you check the [Public API Changes][2] section to know what has been changed since your current revision of the API.

While you are downloading the API build to give it a try, here is a list of added features along with a few code snippets for quick testing.

## Support for More File Formats

This release of Aspose.Cells for C++ has provided the support for more file formats including CSV, Tab-Delimited, XLSM (macro enabled spreadsheet format since Excel 2007) and XLSB (binary spreadsheet format since Excel 2007). Developers can now load these file formats in Aspose.Cells' object model as well as save the result back after manipulation.

The process to load any of the supported file format is simple as passing the file path (or an object of the FileStream) to the Factory::CreateIWorkbook method, however, in order to save the result in a particular file format requires explicit directive, that is; by passing appropriate second parameter from the Aspose::Cells::SaveFormat enumeration to the IWorkbook.Save method.

In order to get more in-depth knowledge of these newly supported file formats, please check the detailed articles as follow.

*   [Load & save CSV files][3]
*   [Load & save Tab-Delimited files][4]
*   [Load & save XLSM spreadsheet files][5]
*   [Load & save XLSB spreadsheet files][6]

## Support for Named Ranges

Aspose.Cells for C++ API now supports the creation of named ranges. The simplest approach to create a named range is to first create an object of the IRange class, and then set its _Name_ property while using the IRange.SetName method. This makes the named range to appear in the Microsoft Excel's **Name Manager** interface.

The following code demonstrates the use of Aspose.Cells for C++ API to [create a named range][7] in a newly created spreadsheet.

```
Append(new String("outCreateNamedRange.xlsx"));

//Create a workbook
intrusive_ptr wb = Factory::CreateIWorkbook();

//Access first worksheet
intrusive_ptr ws = wb->GetIWorksheets()->GetObjectByIndex(0);

//Create a range
intrusive_ptr rng = ws->GetICells()->CreateIRange((intrusive_ptr)new String("A5:C10"));

//Set its name to make it named range
rng->SetName((intrusive_ptr)new String("MyNamedRange"));

//Read the named range created above from names collection
intrusive_ptr nm = wb->GetIWorksheets()->GetINames()->GetObjectByIndex(0);

//Print its FullText and RefersTo properties
printf("Full Text: %s\n", nm->GetFullText()->charValue());
printf("Refers To: %s\n", nm->GetRefersTo()->charValue());

//Save the workbook in xlsx format
wb->Save(outCreateNamedRange, SaveFormat_Xlsx); 
```

Besides creating new named ranges, Aspose.Cells for C++ API also supports to manipulate existing named ranges. Please note, if an object of the IRange has the _Name_ property set, that is; IRange object has a name then it becomes the part of the INameCollection which can be accessible via the IWorksheetCollection class object. If the application requirement is to retrieve a specific named range, it can be get via the INameCollection.GetObjectByIndex method.

The following code snippet uses the Aspose.Cells for C++ API to [manipulate an existing named range][8].

```
//Path of your directory where you want to read or write files from
StringPtr dirPath = new String("D:\\Downloads\\");

//Path of source excel file
StringPtr srcManipulateRange = (new String(dirPath))->Append(new String("srcManipulateRange.xlsx"));

//Path of output excel file
StringPtr outManipulateRange = (new String(dirPath))->Append(new String("outManipulateRange.xlsx"));

//Create a workbook
intrusive_ptr wb = Factory::CreateIWorkbook(srcManipulateRange);

//Read the named range created above from names collection
intrusive_ptr nm = wb->GetIWorksheets()->GetINames()->GetObjectByIndex(0);

//Print its FullText and RefersTo properties
printf("Full Text: %s\n", nm->GetFullText()->charValue());
printf("Refers To: %s\n", nm->GetRefersTo()->charValue());

//Manipulate the RefersTo property of NamedRange
nm->SetRefersTo((intrusive_ptr)new String("=Sheet1!$D$5:$J$10"));

//Save the workbook in xlsx format
wb->Save(outManipulateRange, SaveFormat_Xlsx);
```

## Aspose.Cells for C++ Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for C++ API][9].
*   [Aspose.Cells for C++ Download Section][10].
*   [Aspose.Cells for C++ Documentation][11] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells Product Family Forum][12] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][13] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Cells for C++ API by posting your suggestions and concerns in the Aspose.Cells support forum.




[1]: https://downloads.aspose.com/cells/cpp/new-releases/aspose.cells-for-c---17.1.0/
[2]: http://docs.aspose.com/display/cellscpp/Public+API+Changes+in+Aspose.Cells+17.1.0
[3]: https://docs.aspose.com/display/cellscpp/Home
[4]: https://docs.aspose.com/display/cellscpp/Home
[5]: https://docs.aspose.com/display/cellscpp/Home
[6]: https://docs.aspose.com/display/cellscpp/Home
[7]: https://docs.aspose.com/display/cellscpp/Home
[8]: https://docs.aspose.com/display/cellscpp/Home
[9]: http://www.aspose.com/products/cells/cpp
[10]: http://downloads.aspose.com/cells/cpp
[11]: https://docs.aspose.com/display/cellscpp/Home
[12]: http://forum.aspose.com
[13]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/




