---
title: 'Enhanced Formula Calculations and Evaluation of Functions in MS Project Files'
date: Tue, 31 Mar 2015 16:13:43 +0000
draft: false
url: /2015/03/31/enhanced-formula-calculations-evaluation-of-functions-in-ms-project/
author: Muhammad Waqas
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/aspose-Tasks-for-net_1002.png" alt="">}}


We are pleased to announce the release of [Aspose.Tasks for .NET][1] 8.2.0. This month’s release enhances the feature of formula calculation in project documents by implementing function and other calculations. It also includes an enhancement feature of rendering display details column to output. For a complete list of new features, enhancements and bug fixes, please visit our [product download][2] page.

## Support for Formula Calculations

Our last month’s release introduced the feature of Reading and Writing formulas from extended attributes of a project. This was our first effort to provide support for formulae calculation using the API. This month’s release further enhances the feature of formula calculations by providing support for:

**Using Tasks and Resource Fields in Formulae:** This month’s release now includes support for using a Task and Resource’s fields in formula calculations. For example, a formula can be set to the display the different of task’s finish and deadline dates.

**Using Arithmetic Expression in Formulae:** This month’s release provides support for usage of arithmetic expressions, for example ((1+3\*(2+-5) + 8/2)^3) in formulae. This allows to set any mathematical expression as formula in the extended attribute definition and get as well as save its calculated value in document.

**Using Task Number Fields in Formulae:** Task Outline level, priority and percent complete refer to task number fields. With this month’s release, the API now supports the usage of these properties as formula for a task.

**Using Boolean Values in Formulae:** Formula value can not only be set to tasks and resource fields, arithmetic expression, and task number fields, but also to Boolean values from the project. This sets the formula to various project/tasks’s Boolean parameters that are then calculated at run-time.

For further information about working with formulas, please visit our documentation sections for:

*   Working with Formulas
*   Working with Task, Resource and Project Fields Calculation in Expressions

## Support for Evaluation of Functions

This month’s release also introduces a new feature of evaluating various functions defined as formula expression in Extended Attributes. These include:

**Calculation of Mathematical Functions:** Supports math functions such as _Abs, Atn, Cos, Exp, Fix, Int, Log, Rnd, Sgn, Sin, Sqr_ and _Tan_.

**Calculation of General Functions:** General functions such as _Choose, IIF, IsNumeric, IsNull_ and _Switch_ are also supported with this month’s release.

**Calculation of Text Functions:** Provides support for Text functions such as _Asc, Chr, Format, Instr, LCase, Left, Len, LTrim, Mid, Right, RTrim, Space, StrComp, StrConv, String, Trim_ and _UCase_ functions.

**Calculation of Date/Time Functions:** This month’s release also includes support for a number of Date/Time functions such as _CDate, Date, DateAdd, DateDiff, DatePart, DateSerial, DateValue, Day, Hour_ and a number of others.

For a complete list of supported evaluation functions, please visit our documentation article Support for Evaluation of Functions in Formulas.

## Support for Rendering Details Usage Fields in Chart Area

This month’s release also introduces a new feature of rendering [Details column in the MPP][3] to the output using the project view’s _DisplayDetailsHeaderColumn_ property. This includes the list of following supported fields:

*   Work
*   Actual Work
*   Actual Overwork time
*   Baseline Work
*   Baseline 1-10 Work

## Other Improvements

This month’s release also includes a number of bug fixes that further improves the overall API functionality. These include:

*   Issues with _Timephasedata_ from MPP file
*   Exceptions raised while reading and saving certain MPP files
*   Issues with Task’s GUIDs in MPP 2013 formats
*   Wrong start and finish dates while creating manual tasks

As always, we welcome your queries and inquiries about Aspose.Tasks API. Please feel free to write to us over [Aspose.Tasks forum][4] to get assistance about your questions.




[1]: https://products.aspose.com/tasks/net
[2]: https://products.aspose.com/tasks/net
[3]: https://blog.aspose.com/
[4]: http://forum.aspose.com




