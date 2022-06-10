---
title: 'Aspose.Report - The module list for report tools'
date: Tue, 07 Dec 2004 18:56:00 +0000
draft: false
url: /2004/12/07/32592/
author: GeorgeKahn
summary: ''
tags: ['George Kahn']
---

The following is the module list for upcoming report tools, the first release will include report build engine, visual report designer and data gather interface.

*   Report build engine.

The Report build engine could create and format a report based on a RDL (report definition language) script, RDL is an industry standard and a kind of extensible script, the different development tools vendor could add their own predefined syntax into it. Here is the brief introduction about which feature our RDL script will support.

1.  The definition of general report layout - such as the height of report header, the count of report column, etc.
2.  The definition of report data source - such as a SQL for retrieving data from database or a Tab delimited text file, the Report build engine will retrieve the data based on SQL by invoking the data gather interface.
3.  The definition of some simple procedural flow logic - such as loop and branch (if/else) by which the user could customize some complex reports that can be varied according to some specific situation at the reports building stage.
4.  The definition of some macro variables - It has two purposes, one is that it can work with the definition of procedural flow logic to handle the complex reports; another is that its value could be replaced with some text contents at the reports building stage.
5.  The definition of security validation - It is used to verify if the contents inside the reports can be retrieved and viewed by specified users or groups, the contents could be entire report body, or some report columns, or some report cells only. The Report build engine will validate the security by invoking the report security interface when it encounters the definition of security validation.
6.  The definition of report output type - it is used to specify which reports output format the report build engine will generate, such as Excel, Word or PDF.

*   Visual report designer

The visual report designer is a GUI tools that allow the report analysts or developers to design and define the report template by drag and drop visually. It includes the report design GUI and preview GUI, the report template will be save as RDL script for Report build engine using.

*    Data gather interface

The data gather interface is based on ADO.NET, it can retrieve the data from various database according the connection string and SQL script, and store the data into local disk for the Report build engine use.

*   Report security interface

The report security interface includes a set of APIs that are used to verify if specific users or groups have rights to retrieve and view the data. The report security interface provides the support of development extension, so the client could integrate it with their existing authorization system.

*   Visual query builder

The visual query builder is provided for building the queries visually. It allows users to create and edit queries without knowledge of SQL, prepare and execute queries, and view the results of the execution. It will be integrated with visual report designer.

*   Domain object interface

The domain object interface is provided for simplifying and speeding up the reports designing process, and minimizing the development effort.

The domain object interface includes some APIs to import and reference the domain objects marshaled by the predefined web service; the property of these domain objects will be referenced as the definition of macro variables inside the RDL script.

The domain object interface also includes a visual GUI integrated with visual report designer.

The users will benefit from this feature by separating the work between the report analysts and backend developers, it means that backend developers can boil down complex server-side database behaviors into simple and easy-to-use business elements that report analysts can easily incorporate into their reports with the visual report design tools. For instance, a cross-tab report need some rows of products in the table as the report header, and the products name and count is varied by different situation, the developers could write a web service to retrieve these product list by passing some parameter, then report analysts could use the visual GUI to reference this web service and specify the parameter as macro variables. The report build engine will invoke this web service to get the product list at the reports building stage. This products web service can be reused by other reports.







