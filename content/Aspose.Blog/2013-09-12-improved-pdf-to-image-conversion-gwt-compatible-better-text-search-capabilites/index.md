---
title: 'Improved PDF to Image Conversion using Java'
date: Thu, 12 Sep 2013 06:43:44 +0000
draft: false
url: /2013/09/12/improved-pdf-to-image-conversion-gwt-compatible-better-text-search-capabilites/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for Java logo">}}


Since we introduced the autoported version of Aspose.PDF for Java, we have been working to make this new product as stable and robust as its sibling on .NET. So keeping the tradition of better products alive, we are pleased to announce the release of another major version of [Aspose.PDF for Java 4.2.0][1]. This new release provides a better and more stable PDF to image (TIFF, JPEG, PNG) conversion feature as well as the capability to search for text strings split over two lines. This requirement can be accomplished using [Regular Expressions][2].

```
 String myDir ="c:/pdftest/";
// Open document
com.aspose.pdf.Document pdfDocument = new com.aspose.pdf.Document(myDir+"two_line_text3.pdf");
// Create TextAbsorber object to find all instances of the input search phrase
com.aspose.pdf.TextFragmentAbsorber textFragmentAbsorber = new com.aspose.pdf.TextFragmentAbsorber("one text in( | \r\n)two",new com.aspose.pdf.TextSearchOptions(true));
// Accept the absorber for first page of document
pdfDocument.getPages().accept(textFragmentAbsorber);
// Get the extracted text fragments into collection
com.aspose.pdf.TextFragmentCollection textFragmentCollection = textFragmentAbsorber.getTextFragments();

int fragmentsCount = 0;
// Loop through the Text fragments
for(com.aspose.pdf.TextFragment textFragment : (Iterable)textFragmentCollection)
{
    // The whole textFragment found in the document
    System.out.println("\r\n Fragment #"+ ++fragmentsCount);
    System.out.println("Whole textFragment :- " + textFragment.getText());
    // Iterate through text segments in the separated textFragment
    for(com.aspose.pdf.TextSegment textSegment : (Iterable)textFragment.getSegments())
    {
        System.out.println("Next text segment:- " + textSegment.getText());
        System.out.println("Position :- " + textSegment.getPosition());
        System.out.println("XIndent :- " + textSegment.getPosition().getXIndent());
        System.out.println("YIndent :- " + textSegment.getPosition().getYIndent());
        System.out.println("Font - Name :- " + textSegment.getTextState().getFont().getFontName());
        System.out.println("Font - IsAccessible :- " + textSegment.getTextState().getFont().isAccessible());
        System.out.println("Font - IsEmbedded - " + textSegment.getTextState().getFont().isEmbedded());
        System.out.println("Font - IsSubset :- " + textSegment.getTextState().getFont().isSubset());
        System.out.println("Font Size :- " + textSegment.getTextState().getFontSize());
        System.out.println("Foreground Color :- " + textSegment.getTextState().getForegroundColor());
    }
} 
```

This version is also compatible with Google Web Toolkit. Please visit the following link for further details on what's new and fixed in [Aspose.PDF for Java 4.2.0][3].




[1]: https://products.aspose.com/pdf/java
[2]: http://msdn.microsoft.com/en-us/library/cc295435.aspx
[3]: https://downloads.aspose.com/pdf/java




