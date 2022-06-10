---
title: 'Calculate Excel Formulas and Implement Custom or User Defined Functions in C++'
date: Sun, 26 Feb 2017 14:06:00 +0000
draft: false
url: /2017/02/26/calculate-excel-formulas-and-implement-custom-or-user-defined-functions-in-c/
author: Mshakeel Faiz
summary: ''
tags: ['Calculate Excel formulas', 'User Defined Excel Function', 'define custom excel formulas', 'user defined formula in excel', 'user defined functions in excel']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-cpp.png" alt="create user defined function in excel">}}


Aspose Team is pleased to announce the release of [Aspose.Cells for C++ 17.02.0][1]. This release includes some new features and enhancements that further improve the overall feature set of the API. Please check the [release notes][2] in order to get an idea about what is new and what has been enhanced with this revision of Aspose.Cells for C++. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the [Public API Changes][3] section to know what has been changed since your current revision of the API.

While you are downloading the API build to give it a try, here is a list of added features along with some code snippets for quick testing.

## Improvements and Flexibility in the Calculation of Excel Formulas

Aspose.Cells for C++ has added more overloads of workbook calculation which provide users more control and flexibility to calculate the excel functions on runtime. Users can also implement their own custom functions if needed.

## Different Ways to Calculate Formulas

There are different ways to calculate excel formulas on runtime using Aspose.Cells for C++.  Please check the following article that explains all of them with sample code.

*   [Ways to Calculate Formulas][4]

Here are these three different ways to calculate excel formulas on runtime using the Aspose.Cells for C++.

*   Adding Formulas and Calculating Results
*   Direct Calculation of Formula
*   Calculating Formulas Once Only

## Implement Custom Functions with Aspose.Cells

Aspose.Cells for C++ now supports **ICustomFunction** interface that allows you to define custom (i.e. user defined) functions in a template file or in a code where the custom function can be implemented and evaluated using Aspose.Cells APIs like any other default Microsoft Excel function. Please see the following article that explains how to make use of this feature

*   [Using ICustomFunction Feature][5]

Here is the simplest implementation of **ICustomFunction** interface in Aspose.Cells for C++.

```
//Implement ICustomFunction interface
class CustomFunction : public ICustomFunction
{
public:
    //Evalaute and return the values of your custom functions
    intrusive_ptr 
        CalculateCustomFunction(
        intrusive_ptr functionName, 
        intrusive_ptr paramsList, 
        intrusive_ptr contextObjects)
    {
            if (functionName->Equals(new String("MySampleFunc")))
            {
                return new String("MY sample function was called successfully.");
            }
 
            if (functionName->Equals(new String("YourSampleFunc")))
            {
                return new String("YOUR sample function was called successfully.");
            }
 
            return NULL;
    }
 
};
```

## Aspose.Cells for C++ Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for C++ API][6].
*   [Aspose.Cells for C++ Download Section][7].
*   Aspose.Cells for C++ Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells Product Family Forum][8] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][9] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Cells for C++ API by posting your suggestions and concerns in the Aspose.Cells support forum.




[1]: https://downloads.aspose.com/cells/cpp/new-releases/aspose.cells-for-c---17.02.0/
[2]: https://docs.aspose.com/display/cellscpp/Aspose.Cells+for+CPP+17.02.0+Release+Notes
[3]: https://docs.aspose.com/display/cellscpp/Migrating+from+Earlier+Versions+of+Aspose.Cells
[4]: https://docs.aspose.com/display/cellscpp/Ways+to+Calculate+Formulas
[5]: https://docs.aspose.com/display/cellscpp/Using+ICustomFunction+Feature
[6]: http://www.aspose.com/products/cells/cpp
[7]: http://downloads.aspose.com/cells/cpp
[8]: https://forum.aspose.com/c/cells
[9]: https://blog.aspose.com/category/cells/




