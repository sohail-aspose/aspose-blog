---
title: 'SVG to PDF, Optimize PDF Size, Set More than One Font Path in Aspose.Pdf for Java 4.6.0'
date: Tue, 11 Mar 2014 03:27:33 +0000
draft: false
url: /2014/03/11/svg-to-pdf-optimize-pdf-size-setting-more-than-one-font-path-in-aspose.pdf-for-java-4.6.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Convert SVG to PDF in Java', 'Java library to optimize PDF', 'Optimize PDF document', 'SVG to PDF Converter in Java', 'optimize PDF document in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="SVG to PDF Converter">}}


We are very much excited to announce the release of [Aspose.PDF for Java 4.6.0][1]. This new release provides some great new features including **SVG to PDF** conversion and also includes fixes to problems reported in earlier releases. Furthermore, since the first release of the autoported version of Aspose.Pdf for Java, the development team has been working hard to synchronize the classes and enumerations of the two siblings (Aspose.Pdf for .NET and Aspose.Pdf for Java). In this release, we have made great progress in this area by moving and adding many of the classes from Aspose.Pdf for .NET to the Aspose.Pdf for Java architecture. The complete details of these changes can be found in section [Public API Changes in Aspose.Pdf for Java 4.6.0][2].

# Convert SVG to PDF in Java

In this new release, we have introduced a feature that lets you convert Scalable Vector Graphics (SVG) to PDF format. In order to accomplish this requirement, we have introduced a class named SvgLoadOptions. For further details, please read [SVG to PDF conversion][3].

```
 String file = "Document.svg";
//// Instantiate LoadOption object using SVG load option
com.aspose.pdf.LoadOptions options = new com.aspose.pdf.SvgLoadOptions();
// Create Document object
Document document = new Document(file, options);
// Save the resultant PDF document
document.save("Result.pdf");
```

# Optimize PDF File Size in Java

PDF files usually contain text, images, form fields, fonts, annotations and so on, and sometime duplication of resources in a document increases the file size. To reduce the file size, remove unused and duplicate objects. Aspose.Pdf for Java offers the capability to accomplish this requirement. For further details, read [Optimize PDF file size][4].

```
 // Load source PDF file
com.aspose.pdf.Document doc = new Document("source.pdf");
// Optimize the file size by removing unused objects
com.aspose.pdf.Document.OptimizationOptions opt = new Document.OptimizationOptions();
opt.setRemoveUnusedObjects(true);
opt.setRemoveUnusedStreams(true);
opt.setLinkDuplcateStreams(true);
doc.optimizeResources(opt);
// Save the updated file
doc.save("optimized.pdf");
```

# Setting More than One Font Paths for PDF

A PDF file is mostly comprised of text and text can have more than one font. Therefore, during PDF generation, we can set more than one font path. In order to accomplish this requirement, please try using the following code snippet.

```
 // Adding a new font path
String path = "c:\\fonts\\";
com.aspose.pdf.Document.addLocalFontPath(path);

// Getting the list for standard font directories in different OS
java.util.List list = com.aspose.pdf.Document.getLocalFontPaths();

// Setting the user list for standard font directories
list.add("c:\\fonts2\\");
list.add("c:\\fonts3\\");
com.aspose.pdf.Document.setLocalFontPaths(list);

// Restoring list for standard font directories by default.
com.aspose.pdf.Document.restoreLocalFontPath();
```

# Unified Documentation Archive

In earlier versions of Aspose.Pdf for Java, we had two separate documentation archives: one for the aspose.pdf package and one for the com.aspose.pdf package. From this release, we are providing a single documentation archive for all packages. The .jar is provided under javadoc folder of Aspose.Pdf for Java package.

Go ahead and download and start exploring the new features of [Aspose.Pdf for Java 4.6.0.][5]




[1]: http://www.aspose.com/community/files/72/java-components/aspose.pdf-for-java/entry529105.aspx
[2]: http://docs.aspose.com/display/pdfjava/Public+API+Changes+in+Aspose.Pdf+for+Java+4.6.0
[3]: https://docs.aspose.com/display/pdfjava/Convert+a+File+to+PDF+Format#ConvertaFiletoPDFFormat-ConvertSVGfiletoPDFformat
[4]: https://docs.aspose.com/
[5]: https://downloads.aspose.com/pdf/java




