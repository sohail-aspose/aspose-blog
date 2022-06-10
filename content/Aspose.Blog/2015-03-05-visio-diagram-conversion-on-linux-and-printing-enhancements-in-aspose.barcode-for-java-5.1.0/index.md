---
title: 'Visio Diagram Conversion on Linux and Printing Enhancements in Aspose.Diagram for Java 5.1.0'
date: Thu, 05 Mar 2015 17:05:30 +0000
draft: false
url: /2015/03/05/visio-diagram-conversion-on-linux-and-printing-enhancements-in-aspose.barcode-for-java-5.1.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/aspose_diagram-for-java.png)We’re pleased to announce the release of Aspose.Diagram for Java 5.1.0. In this minor release, we have enhanced Visio diagram printing support through the printer which is connected to the local computer or available on the network. Users were not able to print Visio diagrams by using its Java version. It is now fixed. Another fix is about the conversion, the client was trying to export a VDX to PDF and PNG file formats on the Red Hat Linux Server, but the process hanged. It has also been fixed. This release also includes the most recent bug fixes along with the above enhancements.

We have fixed a number of issues in this release. The most noteworthy problems are listed below.

*   Fixed: Diagram.print("Printer Name") method does not work
    
*   Fixed: NullReferenceException occurred when getting page object by its name
    
*   Fixed: VDX to PDF export hangs on Red Hat Linux Server
    
*   Fixed: VDX to PNG export hangs on Red Hat Linux Server
    

## Deprecate the Support of JDK 1.4 and 1.5

Previously, we were providing three jar files. One for the JDK 1.4, second for JDK 1.5 and third for JDK 1.6 and higher versions. In this new release, we have dropped the support of JDK 1.4 and JDK 1.5. Since, we have provided a single jar for JDK 1.6 or higher versions. It is because both JDKs are discontinued by Sun/Oracle. Even commercial (non-open) support of JDK 1.5 is dropped about a year ago. **If you are presently using JDK 1.4.x or 1.5.x, you must upgrade your JDK prior to migrating to this new release.**

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][2].
    
*   [Download Aspose.Diagram for Java][3].
    
*   Aspose.Diagram for Java wiki docs - Help documentation and API reference documents.
    
*   [Aspose.Diagram product family forum][4] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
    
*   [Enable email subscription][5] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
    
*   [Aspose.Diagram for Java Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
    

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/aspose_diagram-for-java-e1401178596961.png "Aspose.Diagram for Java logo"
[2]: http://www.aspose.com/java/diagram-component.aspx
[3]: http://www.aspose.com/community/files/72/java-components/diagram-java/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[5]: https://blog.aspose.com/
[6]: https://github.com/asposediagram/Aspose_Diagram_Java




