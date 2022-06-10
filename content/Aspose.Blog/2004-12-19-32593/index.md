---
title: 'Aspose.Report - The brief introduction to RDL element class and interface model'
date: Sun, 19 Dec 2004 23:50:00 +0000
draft: false
url: /2004/12/19/32593/
author: GeorgeKahn
summary: ''
tags: ['George Kahn']
---

I am currently working on RDL element class and interface model, here is the brief introduction.

*   BaseElement - Base abstract RDL element class
    

The BaseElement class is an abstract class for all of RDL elements; it provides three major functionality – Composite structure support, Serialize support, logging and debugging support.

1.  Composite structure support – considering the RDL is based on XML document, so every element is capable to hold the reference of its child elements. It also provides an interface to ensure other visitor classes to navigate entire or parts of RDL elements inside a report
    
2.  Serialize support – it is useful to be able to serialize the RDL elements to a XML based file so that we create a custom RDL file for a report
    
3.  Logging and debugging support - every RDL element includes a location object that is used to record a position by which we can locate any RDL element inside the RDL file, a location object includes line number and column number so that the report engine could print the user friendly error message when a RDL file exists problem.
    

*   The RDL element interface based on Inversion Of Control (IOC) pattern and prototype pattern.
    

> Considering the extensibility nature of RDL elements, we adopt the Inversion Of Control pattern  to apply the extensibility to all of RDL elements..
> 
> 1.  A RDL element might be a report item such as a report header, or a macro variable type such as directory or connection string. We group those different RDL elements according to their common functionality by different RDL element interfaces such as ReportItem or VariableType, every interface includes a set of common virtual methods and properties so that the report engine only needs to deal with a few RDL element interfaces without knowing various specific RDL element classes. For instance, if we need to draw a box on report, we could write a new descendant BaseElement class ReportBox implemented the ReportItem interface that includes Positon propertiy and Draw method, then compile this class into a centralized or separated DotNet assembly and copy it to a specified folder. When report engine read this box definition from a RDL file, it would go to this folder to scan all of RDL assemblies, locate the ReportBox class and initialize it through reflection. 
>     
> 2.  As we know that scanning of Dotnet assemblies and reflection are sort of expensive, so we adopt the Prototype pattern in order to minimize the number of scanning and reflection. Report engine only scan the RDL assemblies and initialize the instance of a specific RDL element class once while report engine encounter its definition at the first time, then we add this instance into a in-memory collection, so that report engine could create other same element class instances by looking up this collection and making copies of existed RDL element instance, modifying them as appropriate properties.
>







