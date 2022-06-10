---
title: 'Improved Memory Management in Java PDF Manipulation API'
date: Fri, 27 Sep 2013 19:29:03 +0000
draft: false
url: /2013/09/27/improved-memory-management-single-approach-of-license-initialization/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for Java logo">}}


We are pleased to announce the release of the [Aspose.PDF for Java 4.2.1][1] hotfix. This release provides better memory management when processing large-size documents and performing operations that consume lots of memory. Furthermore, with this version, you only need to initialize the license using the com.aspose.pdf.License object and there is no need to explicitly set the license for legacy versions of Aspose.Pdf for Java (the aspose.pdf package).

Recently, a customer contacted us who needed to search for two strings and remove the text appearing between them. We are pleased to share that this feature has been implemented. Please try using the following code snippet.

```
String path = "c:\\pdftest\\";
// Open document
com.aspose.pdf.Document pdfDocument = new com.aspose.pdf.Document(path+"testHeading (2).pdf");
// Create TextAbsorber object to find all instances of the input search phrase
//
String from="this is heading of level 1";
String till="this is bullet style 1";
com.aspose.pdf.TextFragmentAbsorber textFragmentAbsorber = 
new com.aspose.pdf.TextFragmentAbsorber(from+".*"+till,new com.aspose.pdf.TextSearchOptions(true));
// Accept the absorber for first page of document
pdfDocument.getPages().accept(textFragmentAbsorber);
// Get the extracted text fragments into collection
com.aspose.pdf.TextFragmentCollection textFragmentCollection = 
textFragmentAbsorber.getTextFragments();

// Loop through the Text fragments
for(com.aspose.pdf.TextFragment textFragment : (Iterable)textFragmentCollection)
{
	// It is enough to remove all segments between the first and last segment.
	int size = textFragment.getSegments().size();
	size++;
	// After each deleting size is decremented by 1
	while(textFragment.getSegments().size()>2)
	{
            // Removes the second fragment and recalculates the remaining fragments		
            textFragment.getSegments().delete(2);
	}
}

pdfDocument.save(path+"testHeading_out.pdf");
```

Please visit the following link for further details on what's fixed in [Aspose.PDF for Java 4.2.1][2].




[1]: https://downloads.aspose.com/pdf/java
[2]: https://downloads.aspose.com/pdf/java




