---
title: 'Set DPI/PPI for Images in PDF and Remove Metadata from PDF in Java'
date: Fri, 03 Oct 2014 12:13:49 +0000
draft: false
url: /2014/10/03/set-dpippi-for-images-remove-metadata-pdf-to-html-support-for-bufferedimage-object-with-aspose.pdf-for-java-9.5.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Add Digital Signature to PDF in Java', 'Check DPI of images in PDF', 'Remove metadata from PDF in Java', 'Set DPI of Images in PDF', 'convert html to pdf in java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for Java logo">}}


The Aspose.PDF product family is one of the most demanded APIs provided by Aspose because this single suite provides great support for PDF creation and manipulation on the .NET, Java, JasperReports, SharePoint, Reporting Services, Cloud and Android platform. Sometimes the requirement is to create a solution for PDF files that can be deployed on various operating systems (such as Windows, Linux, MAC OS, and Solaris). In such situations, Java is the ultimate choice and to cater for these requirements, we have an API specific for these needs.

Aspose.PDF for Java is one of our best-selling APIs and makes it possible to create and manipulate PDF files in Java applications. This product is autoported from its sibling Aspose.PDF for .NET and provides great stability and ease of use. This post highlights some of the exciting features offered in the latest release of [Aspose.PDF for Java, 9.5.0.][1]

## Set DPI/PPI of Images in PDF in Java

Aspose.PDF for Java has been providing support for adding, updating, deleting and extracting images from PDF files. Recently, we received a requirement for setting the DPI/PPI (Pixels Per Inch) factor for images when adding them to a PDF file, or when replacing existing images in a PDF file.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-images-SettingDPIOrPPIOfImagesInPDF-.java" >}}

For further details regarding this feature, please read [Setting DPI/PPI of Images in PDF][2].

## Convert PDF to HTML in Java - Specify Image folder

PDF to HTML conversion is one of the most most popular Aspose.Pdf features because it makes it possible to create PDF files that can be viewed on various platforms without a PDF document viewer application. The output HTML is in accordance with WWW standards and can easily be viewed in all web browsers. Using this feature, PDF files can be viewed on handheld devices because you do not need to install any PDF viewing application: a simple web browser is enough to view the file. By default, when converting PDF files to HTML, any images in the PDF are saved in a folder created in the same directory as the output HTML. However, recently we received a request for making it possible to specify a different folder for saving images when generating HTML files. To accomplish this, the saveOptions.SpecialFolderForAllImages property has been introduced. It can be used to specify a target folder for storing output images.

The following code snippet shows a few simple steps that accomplish the requirement of converting a [PDF file to HTML and saving images in a separate folder.][3]

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-docconversion-PDFToHTMLSpecifyImagesFolder-.java" >}}

## Remove Metadata from PDF File

Aspose.Pdf for Java offers the feature to add, update, and remove metadata from PDF documents. Before attempting to remove metadata from a PDF, check if the source PDF contains metadata. The following code snippet shows the steps to [remove metadata from a PDF document.][4]

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-RemoveMetadataFromPDF-.java" >}}

## Support HP-GL to PDF Conversion

PCL file to PDF conversion has been supported in Aspose.Pdf for Java for a while. However, in this release, we also provide support for HP-GL to PDF conversion. For further details, please read [Convert PCL File to PDF][5].

## Add Digital Signatures to PDF Documents

When signing a PDF document using a signature, you basically confirm that its contents should remain "as is". Consequently, any changes made afterwards invalidate the signature and thus you know if the document was altered. Certifying a document first allows you to specify the changes that a user can make to the document without invalidating the certification. For further information, please read [Add Digital Signature to PDF File][6].

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-securityandsignatures-AddDigitalSignatureToPDFFile-.java" >}}

## Image from BufferedImage to PDF Document

Starting from the release of Aspose.Pdf for Java 9.5.0, we have introduced support for adding an image from a BufferedImage instance to a PDF document. To support this requirement, a new method has been implemented: XImageCollection.add(BufferedImage image);

```
BufferedImage originalImage = ImageIO.read(new File("c:\\image\\anyImage.jpg"));
Document pdfDocument1 = new Document();
Page page2 = pdfDocument1.getPages().add();
page2.getResources().getImages().add(originalImage);
```

Now you can use any InputStream and not just FileInputStream objects to add an image. So when using a java.io.ByteArrayInputStream object, you do not need to store any files on the system:

```
BufferedImage originalImage = ImageIO.read(new File("c:\\image\\anyImage.jpg"));
ByteArrayOutputStream baos = new ByteArrayOutputStream();
ImageIO.write( originalImage, "jpg", baos );
baos.flush();
Page page2 = pdfDocument1.getPages().get_Item(i+1);
page2.getResources().getImages().add(new ByteArrayInputStream(baos.toByteArray()));
```

## FDF File Conversion to/from PDF

It is possible to store the values of these form fields in a separate file and that file is an FDF (Forms Data Format) file that contains the values of the form fields in key/pair fashion. FDF files are still being used for this purpose. But now, Adobe also provides an XML encoded form of FDF that is called XFDF. An XFDF file stores the values of form fields in a hierarchical manner using XML tags. For more information, read Whats the Difference Between XML, FDF and XFDF?

Using Aspose.Pdf for Java, developers cannot only export the values of their PDF form fields to an FDF or XFDF file but also to an XML file. The most important thing to know is that all these files use different syntax to save the values of PDF form fields. The following code snippets shows the steps to export FDF file from PDF and also how to import FDF file into PDF.

```
String myDir = "D:\\Temp\\";
// Changed document
com.aspose.pdf.Document doc = new com.aspose.pdf.Document(myDir + "PdfWithAcroForm.pdf");
try
{
    ((TextBoxField)doc.getForm().get_Item("textField")).setValue("new text value");
    ((ListBoxField)doc.getForm().get_Item("listboxField")).setSelected(3);
    ((RadioButtonField)doc.getForm().get_Item("radiobuttonField")).setSelected(2);
    ((CheckboxField)doc.getForm().get_Item("checkboxField")).setChecked(false);

    doc.save(myDir + "Form_Updated.pdf");
}
finally
{
    if (doc != null)
        doc.dispose();
}

// Export to FDF
com.aspose.pdf.facades.Form oldform = new com.aspose.pdf.facades.Form(myDir + "Form_Updated.pdf");
FileOutputStream fsold = new FileOutputStream(myDir + "export.fdf");
try
{
    oldform.exportFdf(fsold);
}
finally
{
    fsold.close();
    if (oldform != null)
        oldform.dispose();
}

// Import from fdf into the source file
com.aspose.pdf.facades.Form form = new com.aspose.pdf.facades.Form(myDir + "PdfWithAcroForm.pdf", myDir + "Form_importFdf.pdf");
try
{
    InputStream fs = new FileInputStream(myDir + "export.fdf");
    try
    {
        form.importFdf(fs);
    }
    finally
    {
        fs.close();
    }
    form.save();
}
finally
{
    if (form != null)
        form.dispose();
}
```

As well as the new features mentioned above, this version includes fixes related to converting SVG, PCL, HTML and XPS files to PDF, and converting PDF files to image format, better text and image extraction, general performance improvements when generating PDF files and much more. Go ahead, download and start exploring the new release of [Aspose.PDF for Java 9.5.0.][7]




[1]: https://downloads.aspose.com/pdf/java
[2]: http://docs.aspose.com/display/pdfjava/Setting+DPI+or+PPI+of+images+in+PDF
[3]: https://docs.aspose.com/display/pdfjava/Convert+PDF+to+HTML+format#ConvertPDFtoHTMLformat-PDFtoHTML-SpecifyImagesFolder
[4]: https://docs.aspose.com/display/pdfjava/PDF+File+Metadata#PDFFileMetadata-RemoveMetadatafromPDF
[5]: https://docs.aspose.com/display/pdfjava/Convert+a+File+to+PDF+Format#ConvertaFiletoPDFFormat-ConvertPCLfiletoPDFformat
[6]: https://docs.aspose.com/
[7]: https://downloads.aspose.com/pdf/java




