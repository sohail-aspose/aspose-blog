---
title: 'How to Represent OOXML Versions in the Aspose.Words API?'
date: Sat, 27 Mar 2010 00:36:00 +0000
draft: false
url: /2010/03/27/how-to-represent-ooxml-versions-in-the-aspose-words-api/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

As of today we have three OOXML versions/flavours:

*   **OOXML ECMA-376 1st Edition, 2006 (this is Word 2007) -** as of today, Aspose.Words supports only this.

*   **ISO/IEC 29500:2008 Transitional (Word 2010)** \- we have code ready for the upcoming release that will support this.

*   **ISO/IEC 29500:2008 Strict - **Aspose.Words will support this some time in the future.

The question I have to all of the customers of Aspose.Words is:  

**What is the best way to represent the different OOXML versions in the Aspose.Words API?**  

The general requirements I have:

1.  It should be easy to use and look natural and consistent.

1.  It should follow the accepted .NET framework coding guidelines.

The two scenarios we are currently considering are:

*   Add the **OoxmlCompliance** enum and add the **SaveOptions.OoxmlCompliance** property.  
    \-or-

*   Add new values to the **SaveFormat** enum.

I will quickly discuss both of the scenarios below and I am looking for your feedback and new ideas as well.  

**Scenario 1: Add the OoxmlCompliance enum and a new option to SaveOptions**  

Saving a document in the new ISO 29500 format will look like this:  

**// You need to set the option. The default will be ECMA-376 to preserve existing behaviour.**

doc.SaveOptions.**OoxmlCompliance** = OoxmlCompliance.Iso29500\_2008\_Transitional;  
doc.Save(@"C:\\MyFile.docx");

/// <summary>  
/// Allows to specify which OOXML specification will be used for the output DOCX file.  
/// </summary>  
public enum OoxmlCompliance  
{  
    /// <summary>  
    /// ECMA-376 1st Edition, 2006.  
    /// </summary>  
    Ecma376\_2006,  
  
    /// <summary>  
    /// ISO/IEC 29500:2008 Transitional compliance level.  
    /// </summary>  
    /// <remarks>  
    /// ISO/IEC 29500:2008 specification is sometimes referred to as as ECMA-376 2nd Edition.  
    /// </remarks>  
    Iso29500\_2008\_Transitional  
}  
  

What I don't like:

1.  It requires an extra line of code to select the OOXML version/flavour.

1.  The names of the enum values are quite ugly and don't follow .NET guidelines, but I want the names to be informative. Tried other variants and did not like them.

**Scenario 2: Add more values to the SaveFormat enum.**  

Saving a document in OOXML could look like this:  

// This is for the new format.

doc.Save(@"C:\\MyFile.docx", **SaveFormat.Docx\_Iso29500\_2008\_Transitional**);

  
 

// This is for the existing ECMA-376 format to keep the behavior unchanged.

doc.Save(@"C:\\MyFile.docx", **SaveFormat.Docx**);

// This is to maintain consistency (have all versions named explicitly)

doc.Save(@"C:\\MyFile.docx", **SaveFormat.Docx\_Ecma376\_2006**);  
  
  

What I don't like:  

We have **SaveFormat.Docx**, **SaveFormat.Docm**, we probably should have **SaveFormat.Dotx** and **SaveFormat.Dotm** and if we want to add ISO29500 Transitional and Strict and also explicit name for ECMA-376 we could end up with 4 x 4 = 16 enum values like **SaveFormat.Docm\_Iso29500\_2008\_Transitional, SaveFormat.Docx\_Iso29500\_2008\_Transitional** etc. Too noisy.  
  

Any ideas?








