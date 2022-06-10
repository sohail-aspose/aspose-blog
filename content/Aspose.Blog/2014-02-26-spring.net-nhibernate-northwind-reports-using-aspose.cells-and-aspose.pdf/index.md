---
title: 'Spring.NET NHibernate Northwind Reports using Aspose.Cells and Aspose.PDF'
date: Wed, 26 Feb 2014 13:26:14 +0000
draft: false
url: /2014/02/26/spring.net-nhibernate-northwind-reports-using-aspose.cells-and-aspose.pdf/
author: Zaheer Tariq
summary: ''
tags: []
categories: ['Aspose.PDF Product Family', 'Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose.words-aspose.pdf_.NET_.png" alt="Aspose.Words and Aspose.Pdf logo">}}


The Spring.NET NHibernate Northwind sample demonstrates the use of Spring's NHibernate integration to simplify the use of NHibernate. A web tier is also included showing how to use the Open-Session In View approach to session management in the web tier.

We have extended the Northwind application to support the following features:

*   Product Catalog report generation using Aspose.Cells and Aspose.Pdf for .NET.
*   Customer Labels report generation using Aspose.Cells and Aspose.Pdf for .NET.
*   Products by Category report using Aspose.Cells and Aspose.Pdf for .NET.
*   Spring.NET NHibernate is used to retrieve the data from the Products, Customers and Categories table of Northwind database, to generate the reports.

The sample demonstrates some great features of Aspose.Cells and Aspose.Pdf such as:

*   Generate XLSX and PDF document with dynamic data from a database.
*   Font, text and table styling with borders and colors.
*   Inserting and positioning images in Microsoft Excel or Acrobat PDF document.
*   Creating and formatting a table with dynamic data in Microsoft Excel or Acrobat PDF document.
*   Group records in the output document and show a total row at the end of a table.
*   Save the same document as XLSX or PDF format.

## Sample Reports Generated using Aspose.Cells



{{< figure align=center src="images/3-Products-by-Category-report-using-Aspose.Cells-for-.NET_-277x300.png" alt="Products by Category report using Aspose.Cells for .NET" caption="Products by Category report using Aspose.Cells for .NET">}}




{{< figure align=center src="images/2-Product-Catalog-report-using-Aspose.Cells-for-.NET_-300x268.png" alt="Product Catalog report using Aspose.Cells for .NET" caption="Product Catalog report using Aspose.Cells for .NET">}}


## Sample Reports Generated using Aspose.Pdf



{{< figure align=center src="images/5-Customer-Labels-report-using-Aspose.Pdf-for-.NET_-300x177.png" alt="Customer Labels report using Aspose.Pdf for .NET" caption="Customer Labels report using Aspose.Pdf for .NET">}}


### Source Code

You can download the complete working source code from:

*   [https://asposespringnet.codeplex.com/][1]

## What is Spring.NET?

Spring.NET is an open source application framework that makes building enterprise .NET applications easier.

Spring.NET provides comprehensive infrastructure support for developing enterprise .NET applications. It allows you to remove incidental complexity when using the base class libraries for best practices, such as test driven development, or easy practices.

The design of Spring.NET is based on the Java version of the Spring Framework, which has shown real-world benefits and is used in thousands of enterprise applications worldwide. Spring .NET is not a quick port from the Java version, but rather a ‘spiritual port’ based on following proven architectural and design patterns in that are not tied to a particular platform.

The breath of functionality in Spring.NET spans application tiers which allows you to treat it as a ‘one stop shop’ but that is not required. Spring .NET is not an all-or-nothing solution. You can use the functionality in its modules independently.

## What is Spring.NET NHibernate Northwind?

The Spring.NET NHibernate Northwind application uses the Northwind database and uses NHibernate to browse and edit customers. It is a simple application that directly uses the DAO layer in many use-cases, as it is doing nothing more than table maintenance, but there is also a simple service layer that handles a fulfillment process. The application uses Spring's declarative transaction management features, standard NHibernate API, and Open Session In View module.

The data access layer consists of two projects: Spring.Northwind.Dao and Spring.Northwind.Dao.NHibernate. The former contains only the Data Access Object (DAO) interfaces. The latter contains the NHibernate implementation of those interfaces. The project Spring.Northwind.Service contains a simple service that calls into multiple DAO objects to satisfy a fulfillment process. The web project, meanwhile, is an ASP.NET web application and the Spring.Northwind.IntegrationTests project contains integration tests for the DAO and Service layers.

The web application uses dependency injection on the .aspx pages to access the middle tier services , for example the FullfillmentService, or in the case of simple table maintenance, the DAO objects directly.

Please check the link below for more details:  
[http://www.springframework.net/doc-latest/reference/html/nh-quickstart.html][2]

## Video

Please check the video below to see it in action.

<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">https://youtu.be/Zubj8V6uUFM</div></figure>




[1]: https://docs.aspose.com/
[2]: http://www.springframework.net/doc-latest/reference/html/nh-quickstart.html




