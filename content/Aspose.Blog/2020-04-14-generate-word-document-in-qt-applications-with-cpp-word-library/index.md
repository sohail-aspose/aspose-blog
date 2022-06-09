---
title: 'Create Word Documents in Qt Applications using Aspose.Words for C++'
seoTitle: ""
description: ""
date: Tue, 14 Apr 2020 12:15:03 +0000
draft: false
url: /2020/04/14/generate-word-document-in-qt-applications-with-cpp-word-library/
author: Usman Aziz
summary: ''
tags: ['Generate Word document in Qt', 'Word library for Qt', 'create Word document in Qt']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Create-Word-Document-in-Qt-Application.png" alt="Create Word Document in Qt Application">}}


[Qt][1] is a popular cross-platform application development framework to develop a variety of applications for desktop, mobile, and embedded systems. C++ based Qt framework uses [MOC (Meta-Object Compiler)][2] to generate a standard C++ source from the Qt-extended C++. Since Qt supports a wide range of applications that may target various scenarios, integration of Word automation features (i.e. generating Word documents, Word to PDF, and etc.) within the Qt applications has a big scope.

[Aspose.Words for C++][3] provides nearly all basic and advanced Word automation features and it can positively serve the Word processing requirements within the Qt applications. So let's see how you can integrate and utilize our C++ Word library to create Word documents within Qt applications.

## Integrate Aspose.Words for C++ within Qt Application

In order to integrate Aspose.Words for C++, you are required to download and extract the library files from the [downloads][4] section. Once you have, you can proceed with one of the following options to develop Qt applications:

*   Using [Qt Creator][5]
*   Using Visual Studio ([read more][6]

In this blog post, I'll show you how to integrate and use Aspose.Words for C++ library within a Qt Console Application developed in Qt Creator.

## Steps to Add Word Library in Qt Application

I assume that you have properly set up the Qt development environment and installed Qt Creator. Once everything is up and running, you can follow the below steps:

*   Open Qt Creator and create a new _Qt Console Application_.



{{< figure align=center src="images/Qt-Console-Application.jpg" alt="Create Word in Qt Application">}}


*   Select the QMake option from the _Build System_ dropdown.



{{< figure align=center src="images/Qt-Console-Application-QMake.jpg" alt="select QMake build">}}


*   Select the appropriate kit and finish the wizard.
*   Copy _Aspose.Words.Cpp_ and _CodePorting.Native.Cs2Cpp\_vc14\_20.3_ folders from the extracted package of Aspose.Words for C++ into the root of the project.



{{< figure align=center src="images/Aspose.Words-lib-files.jpg" alt="Add Word library files">}}


*   In order to add paths to lib and include folders, right-click on the project in LHS panel and select _Add Library_.



{{< figure align=center src="images/Add-Word-Library.jpg" alt="Add Word Library in Qt">}}


*   Select the External Library option and browse paths to include and lib folders one by one.



{{< figure align=center src="images/Add-Word-Library-2.jpg" alt="Add external library in Qt">}}


*   Once done, your .pro project file will contain the following entries:



{{< figure align=center src="images/Qt-PRO-File-1024x372.png" alt="Qt Project File">}}


*   Build the application and you are done with the integration.

## Generate a Word Document in Qt Application

Now you are ready to use Aspose.Words for C++ features. Let's see how to generate a simple Word document in a Qt application. The following are the steps along with the code snippets required to create a Word document.

*   Include the following header files in _main.cpp_.

```
#include <Aspose.Words.Cpp/Model/Document/Document.h>
#include <Aspose.Words.Cpp/Model/Document/DocumentBuilder.h>
#include <iostream>
```

*   Insert the code to generate a Word DOCX document inside the _main_ function.

```
int main(int argc, char *argv[])
{
    auto doc = System::MakeObject<Aspose::Words::Document>();
    auto builder = System::MakeObject<Aspose::Words::DocumentBuilder>(doc);
    builder->Writeln(u"Hello World!");
    doc->Save(u"HelloWorld.docx");
    std::cout<<"Done..";

    QCoreApplication a(argc, argv);
    return a.exec();
}
```

*   Build and run the application.

## Learn more about Aspose.Words for C++

Aspose.Words for C++ also lets you create more complex and rich Word documents. Furthermore, you can perform various document conversions within the Qt applications. Learn more about Aspose.Words for C++ using the [documentation][7].

## Share your feedback

In case you would have any questions or queries regarding Aspose.Words for C++, feel free to post on our [forum][8].




[1]: https://www.qt.io/
[2]: http://doc.qt.io/qt-5/moc.html
[3]: http://products.aspose.com/words/cpp
[4]: https://downloads.aspose.com/words/cpp
[5]: https://en.wikipedia.org/wiki/Qt_Creator
[6]: https://blog.aspose.com/2020/04/15/create-or-modify-word-documents-in-qt-using-visual-studio/)
[7]: https://docs.aspose.com/display/wordscpp/Home
[8]: http://forum.aspose.com





