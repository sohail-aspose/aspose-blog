---
title: 'Use Smart Pointers in Aspose.PDF for C++ 18.3'
date: Sun, 29 Apr 2018 21:15:26 +0000
draft: false
url: /2018/04/29/implementation-of-smart-pointers-in-aspose.pdf-for-c-18.3/
author: Asad Ali
summary: ''
tags: ['Asad Ali']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-cpp-128x128.png" alt="aspose-pdf-for-cpp">}}


We at Aspose are very pleased to announce the availability of the next version of Aspose.PDF for C++. [Aspose.PDF for C++ 18.3][1] has been released and is available over NuGet Gallery for download and to be used in C++ Applications. Like every release of the API, we have made improvements in performance as well as in memory management. In case you are going to use Aspose.PDF for C++ 18.3, we recommend you to please visit [release notes][2] page in the API documentation.

In [Aspose.PDF for C++ 18.3][3], we have introduced Smart Pointers. Using smart pointers, we can make pointers to work in way that we do not need to explicitly call delete. Using smart pointers, improves memory usage as well as boost the performance of the program. They, however, look like normal pointer but they can do many things that a normal pointer cannot, like automatic destruction, reference counting and more. In Aspose.PDF for C++ 18.3, new pointer system SystemPtr is introduced instead of SharedPtr and WeakPtr. SharedPtr is alias for SmartPtr – whereas, WeakPtr is inherited from SmartPtr. Along with this new implementation we have also fixed asposecpplib, in order to improve performance.

## Miscellaneous Resources

Please visit the following links for information regarding latest release [Aspose.PDF for C++ 18.3][4] and [Release Notes][5] section. In case you have any question about Aspose.PDF for C++, you can post your inquiry in [Aspose.PDF forums][6]. We will be more than happy to assist you there.

*   [Homepage for Aspose.PDF for C++][7]
*   [Download Aspose.PDF for C++][8]
*   [Aspose.PDF product family forum][9]– Post your technical questions and queries, or any other problem you face while running Aspose.PDF APIs.
*   [Aspose.PDF for C++ online documentation][10]– help documentation on using Aspose.PDF for C++ API.
*   [Aspose.PDF for C++ API Reference][11]– Online public API reference for using the API.
*   [Enable Blog Subscription][12]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.




[1]: https://www.nuget.org/packages/Aspose.PDF.Cpp/18.3.0
[2]: https://docs.aspose.com/pdf/cpp/aspose-pdf-for-cpp-18-3-release-notes/
[3]: https://www.nuget.org/packages/Aspose.PDF.Cpp/18.3.0
[4]: https://www.nuget.org/packages/Aspose.PDF.Cpp/18.3.0
[5]: https://docs.aspose.com/pdf/cpp/aspose-pdf-for-cpp-18-3-release-notes/
[6]: https://forum.aspose.com/c/pdf
[7]: https://products.aspose.com/pdf/cpp
[8]: https://www.nuget.org/packages/Aspose.PDF.Cpp/18.3.0
[9]: https://forum.aspose.com/c/pdf
[10]: https://docs.aspose.com/pdf/cpp/
[11]: https://apireference.aspose.com/cpp/pdf
[12]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/




