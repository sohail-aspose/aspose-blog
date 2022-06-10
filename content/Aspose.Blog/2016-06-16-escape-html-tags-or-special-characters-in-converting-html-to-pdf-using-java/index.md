---
title: 'Escape HTML Tags and Special Characters in HTML to PDF using Java'
date: Thu, 16 Jun 2016 14:12:48 +0000
draft: false
url: /2016/06/16/escape-html-tags-or-special-characters-in-converting-html-to-pdf-using-java/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Convert HTML to PDF using Java', 'Escape special characters in HTML to PDF', 'Escape specified HTML tags in HTML to PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for .NET logo">}}


A new release of [Aspose.PDF for Java][1] has been published with new and exciting features that makes PDF files creation, as well as manipulation much convenient. We have always strived to provide simple and robust features in our API which help our customers to achieve complex requirements with simple code snippets. Our APIs have uncompromising capabilities for document manipulation/generation and these startling features put incredible power that leaps past most APIs in the market. It makes even complex work as easy as two lines of code and users can perform interfile format conversion with simple code snippets. The key to our API’s experience is its simple and workable approach, which helps in creating incredible applications with fewer lines of code. Likewise, we have provided some greatly demanded features in this release as well as fixes for issues reported in earlier release versions.

## HTML to PDF - Escape HTML Tags and Special Characters

One of the customers recently shared a requirement to have a built-in feature that can be used to escape the HTML tags and unescape special characters when writing those in PDF. Also ignoring any kind of text formatting (e.g. escape < /li > with "\\r\\n" etc.)

```
// input HTML 
String HTML = "< b >BIG TEXT< /b>< ol>SOME VALUE< /ol>< li >item1< /li >< li >item2 & 3 < /li >< /ol >";
// CSS for input HTML contents
String CSS = " ✱ {font-weight : normal !important ; margin :0 !important ; padding:0 !important ; list-style-type:none !important}";
// instantiate Document instance
Document doc = new Document();
// add page to pages collection of Document object
Page page = doc.getPages().add();
// add HTMLFragment to paragraphs collection of PDF page
page.getParagraphs().add(new com.aspose.pdf.HtmlFragment(CSS + HTML));
// save resultant PDF file
doc.save("output.pdf");
```

## Get Warnings for Font Substitution

One of the customers recently had a requirement to show a warning when fonts are substituted. This is a useful feature in tests, as it allows to fail the tests faster if the font is missing, rather than having to track down why the result looks incorrect. In order to cater to this requirement, please try using the following code snippet where Document class gets notifications about font substitutions.

```
// Load existing PDf file 
Document pdfDoc = new Document(inFile);

final Map<string,string> names =  new HashMap<string,string>() ;
        
pdfDoc.FontSubstitution.add(new Document.FontSubstitutionHandler()
{
    public void invoke(Font font, Font newFont)
    {
        //add substituted FontNames into map.  
        names.put(font.getFontName(), newFont.getFontName());
        //or print the message into console
        System.out.println("Warning: Font "+ font.getFontName() + " was substituted with another font -> " + newFont.getFontName());
    }
});
// instantiate HTMLSave option to save output in HTML
HtmlSaveOptions htmlSaveOps = new HtmlSaveOptions();
// save resultant file
pdfDoc.save("output.html", htmlSaveOps);</string,string></string,string>
```

## EmfDevice Implementation

We have implemented the EmfDevice class to convert PDF files to EMF format and in order to accomplish this requirement, please try using the following code snippet.

```
// instantiate EmfDevice object
EmfDevice device = new EmfDevice(new Resolution(96));
// load existing PDF file
Document doc = new Document("Input.pdf");
// save first page of PDF file as Emf image
device.process(doc.getPages().get_Item(1), "output.emf");
```

## Default Font when Specific Font from Document is Missing

When transforming PDF files to DOC or HTML format, the fonts used inside PDF files are used in resultant files, so that formatting of the document is preserved. However recently some customers reported that they are facing Font not found issue when converting PDF files to DOC or HTML format on the non-Windows environment. As a workaround, the user has to install the respective font on his system but sometimes the user is not certain about the font to be used. Therefore a request to have a feature of using default font if specific fonts used inside the document are missing (_not installed over system_). So instead of throwing an exception, they are interested in having a feature to use one of the default fonts i.e. Arial when performing conversion and as may consider showing a message in Console that default font was used because ABC font was found missing. However, notice that we do not guarantee that the substituted font will correctly show all the characters. Therefore you should find yourself the font that will be compatible with the absent original font. Also, we implemented the ability to get a notification when the font is substituted.

```
Document pdf = new Document(myDir+"Redis.pdf");

//configure font substitution
CustomSubst1 subst1 = new CustomSubst1();
FontRepository.getSubstitutions().add(subst1);
        
//Configure notifier to console
pdf.FontSubstitution.add(new Document.FontSubstitutionHandler()
{
    public void invoke(Font font, Font newFont)
    {
        //print substituted FontNames into console
        System.out.println("Warning: Font "+ font.getFontName() + " was substituted with another font -> " + newFont.getFontName());
    }
});
        
HtmlSaveOptions htmlSaveOps = new HtmlSaveOptions();
pdf.save(myDir+"Redis_1150_substitutedWithMSGothic_release.html", htmlSaveOps);

/**
* The class to implement font substitution
*/
private static class CustomSubst1 extends CustomFontSubstitutionBase
{
    public boolean trySubstitute(OriginalFontSpecification originalFontSpecification, /*out*/ com.aspose.pdf.Font[] substitutionFont)
    {
        //1. substitute Arial font with TimesNewRoman font
//            if ("Arial".equals(originalFontSpecification.getOriginalFontName()))
//            {
//                substitutionFont[0] = FontRepository.findFont("TimesNewRoman");
//                return true;
//            }            
//            else
//                return super.trySubstitute(originalFontSpecification, /*out*/ substitutionFont);
        //2. or substitute all the fonts with the MSGothic font            
        substitutionFont[0] = FontRepository.findFont("MSGothic");
        return true;            
    }
}
```

## Miscellaneous Fixes

As well as the enhancements and features discussed above, there have been specific improvements regarding PDF to HTML, PDF to PDF/A, HTML to PDF, Epub to PDF, Conversion of Non-Searchable PDF to Searchable PDF file, Text extraction from PDF and image placement inside PDF are also improved. Please download and try the latest release of [Aspose.PDF for Java 11.5.0][2].




[1]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+11.5.0+Release+Notes
[2]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+11.5.0+Release+Notes




