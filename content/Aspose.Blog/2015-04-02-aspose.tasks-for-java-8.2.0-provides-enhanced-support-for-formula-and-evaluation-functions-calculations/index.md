---
title: 'Aspose.Tasks for Java 8.2.0 provides Enhanced Support for Formula and Evaluation Functions Calculations'
date: Thu, 02 Apr 2015 09:01:47 +0000
draft: false
url: /2015/04/02/aspose.tasks-for-java-8.2.0-provides-enhanced-support-for-formula-and-evaluation-functions-calculations/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2015/04/aspose-Tasks-for-Java_1001.png)

After the release of Aspose.Tasks for .NET 8.2.0, we are pleased to share the release of Aspose.Tasks for Java 8.2.0. Ported from its equivalent .NET version, this month’s release includes the same enhancements and improvements. For a complete list of enhancements and other improvements, please visit the Aspose.Tasks for Java [release page][2]. If you have any query/inquiry about Aspose.Tasks, please feel free to write to us over [Aspose.Tasks forum][3].

# Enhancements

This month’s release has a number of enhancements related to formula calculations in document. These include:

# Using Project Data Fields in Formula Calculations

Aspose.Tasks for Java 8.1.0 introduced the feature of reading and writing formulas to project document. Working with formulas was supported by adding formula expressions to Extended Attributes of the project. This month’s release further enhances the support for working with formulas by implementing the usage of Project data, arithmetic and Boolean expressions as formula values as described below.More Info

**Tasks, Resource and Project Fields Usage in Formulae:**With this month’s release, Project data fields such as Tasks’ and Resource’s properties can be used in formula calculation now. This allows, for example, to use a task’s finish and deadline dates in formula fields. In addition, task’s number fields such as outline level, priority and percent can also be as formula for a task.

**Arithmetic Expressions Usage in Formula:** In addition to project data, this month’s release now provides support for setting formula values in a document to arithmetic expressions such as ((1+3\*(2+-5) + 8/2)^3). Calculation of such arithmetic formulas is done using the standard operator precedence.

**Boolean Values Usage in Formulae:**The new enhancements in theAPI also provide support for using project’s/task’s Boolean parameters as formula values.

# Support for Evaluation Functions

In addition to using project’s data as formula expressions, the API now supports using:

*   **Mathematical functions** such as Abs, Atn, Cos, Exp, Fix, Int, Log, Rnd, Sgn, Sin, Sqr and Tan as formula expresions
*   **General Functions** such as Choose, IIF, IsNumeric, IsNull and Switch as formula expressions
*   **Text functions** as formula expression, for example _Asc, Chr, Format, Instr, LCase, Left, Len, LTrim, Mid, Right, RTrim, Space, StrComp, StrConv, String, Trim_ and_UCase_
*   **Date/Time Functions** as formula expressions such as _CDate, Date, DateAdd, DateDiff, DatePart, DateSerial, DateValue, Day, Hour_ and a number of others

You can visit our documentation article, Support for Evaluation Functions, for examples about these.

# Bug Fixes

This month’s release also fixes a number of bugs that were reported by our valued customers. This further improves the overall functionality of the API. These include functionality bug fixes related to time and duration of tasks, wrong timephased data, and a few exceptions.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/04/aspose-Tasks-for-Java_1001.png "aspose-Tasks-for-Java_1001"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.tasks-for-java/default.aspx
[3]: http://www.aspose.com/community/forums/aspose.tasks-product-family/96/showforum.aspx




