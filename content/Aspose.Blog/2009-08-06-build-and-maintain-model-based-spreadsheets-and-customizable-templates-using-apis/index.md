---
title: 'ModelSheet Authoring and Customizable Templates using Aspose.Cells to build and maintain complex Spreadsheet Models'
date: Thu, 06 Aug 2009 11:30:39 +0000
draft: false
url: /2009/08/06/build-and-maintain-model-based-spreadsheets-and-customizable-templates-using-apis/
author: Modelsheet Team
summary: ''
tags: ['Aspose.Cells', 'Success Stories']
categories: ['Aspose.Cells Product Family']
---

## Product Background / Overview



{{< figure align=center src="images/Model-Sheet-Software-Logo.png" alt="">}}


Our goal is to enhance the power of desktop modelling by augmenting, not replacing, existing tools such as spreadsheets. With this target, we have developed ModelSheet Authoring, an environment for building and maintaining model-based spreadsheets, and Customizable Templates.

## ModelSheet Authoring

As models become larger and more complex, they become harder to author and maintain by conventional methods. ModelSheet Authoring addresses this issue on several fronts. It separates model logic from sheet layout, while using web workbooks (similar to Excel workbooks) to visualize the model during the authoring process, so modellers can focus on business logic. It captures model logic with named variables that have dimensions, time series and data types. Formulas are expressed with named variables; they apply to regions of cells, so there are far fewer formulas. Cell addresses don't exist anywhere. You can build and evolve your model in ModelSheet Authoring, and then export it to Excel where formulas are expressed with cell addresses. You can also re-import any values you change in exported Excel workbooks to update and refine your original model.

## ModelSheet Customizable Templates

A customized template is a flexible model that you can adapt to your situation by filling in a simple form, without editing a spreadsheet or its formulas. For example, you can specify time range and time grain; number and names of items in a dimension (such as your products and product families); and include or exclude major features. The resulting spreadsheet matches your needs better than any standard template.

## Requirements Scenario

Our requirements for an Excel spreadsheet library included: support for a wide range of Excel capabilities including formulas, formatting, sheet layout and named regions; the ability to handle (very) large spreadsheets efficiently; access to advanced features like graphics and pivot tables; full .NET support; flexible licensing terms for SaaS and desktop deployment; and responsive technical support. After evaluating the leading candidates, [Aspose.Cells][1] came out on top.

## Solution Implementation

The main output of our product is a complex, fully-functional Excel spreadsheet. Our solution is coded using C#, running as either an IIS ASP.NET web site or a Windows Forms application. We use both 32-bit and 64-bit operating systems (some of our processes require more than 4GB of managed memory.) The .NET version 2.0 Aspose.Cells DLL integrates perfectly into all of these scenarios. We use [Aspose.Cells for .NET][2] to create spreadsheets from scratch, filling in individual formulas, data and formats. We also merge existing worksheets into our output workbook, many of which contain charts and pivot tables, integrating them via named ranges. We use [Aspose.Cells][3] to do all of the reading and merging.

## Building a Model with ModelSheet Authoring

Using ModelSheet Authoring, the user builds models by working only with what’s important – the pieces of information such as revenue and cost, and how they are related to each other. The user need not be concerned with how they are laid out on a spreadsheet. This enables the user to build large, reliable and expressive models quite simply. ModelSheet Authoring can then, using [Aspose.Cells][4], generate Excel spreadsheets from these models and re-import any changes made to them as shown in steps 2 and 3.



{{< figure align=center src="images/ModelSheet_Case-study_for_Aspose-Cells_.NET_-1024x322.png" alt="">}}


## A Snapshot of a Part of a model in ModelSheet Authoring

This view shows the formulas for the sales forecast. Software sales for Products A and B are given in the first time period and then grow by planned growth rates. Sales of support services are determined by planned retention rates of existing service customers, plus a planned percentage of new software license sales four quarters ago.

In this view, the pink cells contain the data and formulas (listed below the table) that define all values in the table.



{{< figure align=center src="images/ModelSheet_Case-study_for_Aspose-Cells_.NET-1.png" alt="" caption="Part of a model">}}


## A Snapshot of Parts of an Exported Excel Workbook

ModelSheet Authoring models are exported to Excel using [Aspose.Cells][5] resulting in workbooks that are complex and detailed, making them ideal for making key inferences and decisions that can help users take action to maximize outcomes.



{{< figure align=center src="images/ModelSheet_Case-study_for_Aspose-Cells_.NET-2.png" alt="" caption="Exported Excel workbook">}}


## Benefits

In our situation, using Excel automation to read and write workbooks wasn’t possible: it was far too slow and didn’t work in a server-based environment. And, with our small team, custom-coding reading and writing of Excel didn’t make sense. [Aspose.Cells][6] provides an off-the-shelf, cost-effective, well-supported solution that frees us to spend time on our core technology. Also, since we’re using spreadsheet technology in a novel way, we fully expected we’d need additional support and features. We’ve found Aspose’s quick response to be a real benefit and a critical factor in our success.

## Future Implementations

We will likely enable ModelSheet to produce workbooks for Excel 2007 in the near future and for Excel 2010 in a year or so. We also expect to be generating charts and pivot tables from scratch.

## Conclusion

[Aspose.Cells][7] has become an integral part of ModelSheet technology and products. It has worked well and enabled us to focus on our core competencies. The excellent technical support, especially the willingness to quickly add new features in response to our needs, has been critical to our success.

## For More Information

If you wish to learn more about how ModelSheet uses [Aspose.Cells][8], or more about their products please visit them at [www.modelsheetsoft.com][9] or contact them at [info@modelsheetsoft.com][10].




[1]: https://products.aspose.com/cells
[2]: https://products.aspose.com/cells/net
[3]: https://products.aspose.com/cells
[4]: https://products.aspose.com/cells
[5]: https://products.aspose.com/cells
[6]: https://products.aspose.com/cells/family
[7]: https://products.aspose.com/cells
[8]: https://products.aspose.com/cells
[9]: http://www.modelsheetsoft.com
[10]: mailto:info@modelsheetsoft.com




