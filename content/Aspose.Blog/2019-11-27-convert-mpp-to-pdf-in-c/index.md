---
title: 'Convert MPP Files to PDF using C++'
date: Wed, 27 Nov 2019 08:20:59 +0000
draft: false
url: /2019/11/27/convert-mpp-to-pdf-in-c/
author: Muzammil Khan
summary: ''
tags: ['Convert Microsoft Project to PDF', 'convert MPP to PDF', 'ms project c++ api']
categories: ['Aspose.Tasks Product Family']
---

This article demonstrates how to convert a Microsoft Project data to a PDF file using [Aspose.Tasks for C++][1] which is an easy to use API for manipulating project files. This API provides reading and writing of MPP files without using Microsoft Project. If you do not have Aspose.Tasks for C++ API installed, please follow the instructions given on [installation][2] page.

The [.mpp][3] is the default file extension introduced by Microsoft Project. It typically contains a list of tasks that make up a particular project and allow the critical path of a project to be defined. [PDF][4] is a "multi-platform" file type supported by all existing platforms like Windows, Linux and MAC etc.

## Convert a Project MPP to PDF using C++

[Aspose.Tasks for C++][5] simplifies the functionality of exporting any project data to PDF in your C++ based applications with a two-step process:

1.  Load a project file
2.  Save it as a PDF

The following code snippet demonstrates the conversion of a project file to a single PDF file.

```
// Read the input Project file
System::SharedPtr<Project> project = System::MakeObject<Project>(dataDir + u"Project.mpp");
    
// Save the Project as PDF
project->Save(dataDir + u"SaveProjectAsPDF_out.pdf", Aspose::Tasks::Saving::SaveFileFormat::PDF);
```

## Convert a Project MPP to Multiple PDF Files using C++

Aspose.Tasks for C++ also allows to render complete project data into multiple PDF files by setting the **SaveToSeparateFiles** flag to **TRUE** as demonstrated below:

```
System::SharedPtr<Project> project = System::MakeObject<Project>(dataDir + u"Software Development Plan.mpp");
System::SharedPtr<PdfSaveOptions> saveOptions = System::MakeObject<PdfSaveOptions>();
saveOptions->set_SaveToSeparateFiles(true);
saveOptions->set_Pages(System::MakeObject<System::Collections::Generic::List<int32_t>>());
saveOptions->get_Pages()->Add(1);
saveOptions->get_Pages()->Add(4);
project->Save(dataDir + u"SaveToMultiplePDFFiles_out.pdf", System::StaticCast<Aspose::Tasks::Saving::SaveOptions>(saveOptions));
```

For more information regarding adjusting the column size and font settings while converting any MPP to a PDF, you may go through [Convert Project to PDF in the C++][6] section of the API documentation.




[1]: https://products.aspose.com/tasks/cpp
[2]: https://docs.aspose.com/display/taskscpp/Installation
[3]: https://wiki.fileformat.com/project-management/mpp/
[4]: https://wiki.fileformat.com/view/pdf/
[5]: https://docs.aspose.com/display/taskscpp/Home
[6]: https://docs.aspose.com/display/taskscpp/Convert+Project+to+PDF+in+CPP




