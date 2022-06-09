---
title: 'Handle Word Documents in Qt Applications in Visual Studio'
seoTitle: ""
description: ""
date: Wed, 15 Apr 2020 16:43:32 +0000
draft: false
url: /2020/04/15/create-or-modify-word-documents-in-qt-using-visual-studio/
author: Usman Aziz
summary: ''
tags: ['Create Word Documents in Qt', 'Modify Word Documents in Qt', 'Qt in Visual Studio', 'Word library for Qt']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Create-Word-Document-in-Qt-Small.png" alt="Create and edit DOCX in Qt">}}


In the [previous post][1], I have shown you how to integrate [Aspose.Words for C++][2] in a Qt application using Qt Creator. In this post, we'll check out how to set up and use Aspose.Words for C++ in Qt using Visual Studio. Later, we will create a Word document within the Qt application.

## Set Up Aspose.Words for C++ in Qt Application

For Qt application development in Visual Studio, I have used the following Visual Studio, Qt and Qt VS Tools versions:

*   Visual Studio 2017
*   Qt 5.14.2
*   [Qt VS Tools for Visual Studio 2017][3]

Once you have set up the required environment, you can proceed with the following steps for integrating Aspose' Word library in the Qt application.

*   Download and install [CMake][4].
*   Download and unpack [Aspose.Words for C++][5].
*   Create a new folder for your project files and copy/paste _Aspose.Words.Cpp_ and _CodePorting.Native.Cs2Cpp\_vc14\_20.3_ folders from unpacked package.
*   Create a new file named _CMakeLists.txt_ in the same folder.
*   Copy and paste the following content within the _CMakeLists.txt_ file.

```
cmake_minimum_required(VERSION 3.1.0 FATAL_ERROR)

project(Qt_AsposeWords_CMake)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

find_package(Qt5 COMPONENTS Widgets REQUIRED)
find_package(CodePorting.Native.Cs2Cpp REQUIRED CONFIG PATHS ${CMAKE_CURRENT_SOURCE_DIR} NO_DEFAULT_PATH)
find_package(Aspose.Words.Cpp REQUIRED CONFIG PATHS ${CMAKE_CURRENT_SOURCE_DIR} NO_DEFAULT_PATH)

add_executable(Qt_AsposeWords_CMake
    main.cpp
)

target_link_libraries(Qt_AsposeWords_CMake PRIVATE Qt5::Widgets Aspose::Words) 

set_directory_properties(PROPERTIES VS_STARTUP_PROJECT Qt_AsposeWords_CMake)

file(TO_NATIVE_PATH "${Aspose.Words.Cpp_DIR}/lib/${CMAKE_VS_PLATFORM_NAME}" Aspose.Words.Cpp_DLL_PATH)
file(TO_NATIVE_PATH "${CodePorting.Native.Cs2Cpp_DIR}/lib" CodePorting.Native.Cs2Cpp_DLL_PATH)
file(TO_NATIVE_PATH "${Qt5_DIR}/../../../bin" Qt5_DLL_PATH)

set_target_properties(Qt_AsposeWords_CMake PROPERTIES VS_DEBUGGER_ENVIRONMENT "PATH=${Aspose.Words.Cpp_DLL_PATH}\\$<CONFIG>;${CodePorting.Native.Cs2Cpp_DLL_PATH};${Qt5_DLL_PATH};$(Path)") 
```

*   Open _Command Prompt_ and _cd_ to the project folder.
*   Run the following command by replacing _<path-to-qt5>_ with the path to _Qt5Config.cmake_ file (i.e. C:\\QT\\5.14.2\\msvc2017\_64\\lib\\cmake\\Qt5).

```
cmake -G "Visual Studio 15 2017" -Thost=x64 -Ax64 -S . -B build -D"Qt5_DIR=<path-to-qt5>"
```

Once you have completed the above-mentioned steps, a Visual Studio solution will be created in the folder. You are now ready to use Aspose.Words for C++ features within the Qt application. Lets now check out how to create a Word document in this Qt project.

## Create Word Documents in Qt Application using Visual Studio

The following are the steps to create a Word document in the Qt application using Aspose.Words for C++:

*   Open the solution in Visual Studio.
*   Create a new _.cpp_ file named _main.cpp_ and include the following headers files in it.

```
#include <iostream>
#include <Aspose.Words.Cpp/Model/Document/Document.h>
#include <Aspose.Words.Cpp/Model/Document/DocumentBuilder.h>
```

*   Copy/paste the following code in the main function:

```
auto doc = System::MakeObject<Aspose::Words::Document>();
auto builder = System::MakeObject<Aspose::Words::DocumentBuilder>(doc);
builder->Writeln(u"Hello World!");
doc->Save(u"HelloWorld.docx");
std::cout << "Word document has been created.";
QCoreApplication a(argc, argv);	
return a.exec();
```

*   Build and run the application.

## Learn more about Aspose.Words for C++

Explore the [documentation][6] of Aspose.Words for C++ in order to learn how to create more complex and rich Word documents.

## See Also

*   [Create Word Documents in Qt Applications using Qt Creator][7]




[1]: https://blog.aspose.com/2020/04/14/generate-word-document-in-qt-applications-with-cpp-word-library/
[2]: https://products.aspose.com/words/cpp
[3]: https://marketplace.visualstudio.com/items?itemName=TheQtCompany.QtVisualStudioTools-19123
[4]: https://github.com/Kitware/CMake/releases/download/v3.17.1/cmake-3.17.1-win64-x64.msi
[5]: https://downloads.aspose.com/words/cpp
[6]: https://docs.aspose.com/display/wordscpp/Home
[7]: https://blog.aspose.com/2020/04/14/generate-word-document-in-qt-applications-with-cpp-word-library/





