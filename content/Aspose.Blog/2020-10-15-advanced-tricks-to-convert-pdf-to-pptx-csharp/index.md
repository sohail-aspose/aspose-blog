---
title: 'C# PDF to PPTX Conversion - Handle Notes and Decoration Graphics'
seoTitle: ""
description: ""
date: Thu, 15 Oct 2020 13:51:05 +0000
draft: false
url: /2020/10/15/advanced-tricks-to-convert-pdf-to-pptx-csharp/
author: Andriyandruhovski
summary: 'In one of the previous posts, we talked about how to convert PDF to PowerPoint presentation conversion. In most cases, the basic set of options works well, but today we will discuss two advanced trick'
tags: ['Handle Notes or Comments in pdf to pptx', 'Separate Decoration Graphics in pdf to pptx', 'convert pdf to pptx csharp']
categories: ['Aspose.PDF Product Family']
---

In [one of the previous posts][1], we talked about how to convert PDF files to PowerPoint PPT/PPTX presentations using C# within our .NET applications. In most cases, the basic set of conversion options works well. However, today, we will discuss some advanced tricks for PDF to PPTX conversion:

*   [Handle Notes or Comments][2]
*   [Separate Decoration Graphics from Content Images][3]

## Handle Notes or Comments in PDF to PPTX C# Conversion {#Handle-Notes-or-Comments}

When I tell people about something and use a presentation, I also like to make notes on slides, draw arrows, make accents with geometric shapes, etc.

### How to Draw on PDF?

It is easy, I open my PDF file in Adobe Reader DC or in Microsoft Edge and use a pencil tool. By default, Adobe Reader uses a red pencil.



{{< figure align=center src="images/conversion-pdf-pptx-adv-01-1024x616.png" alt="handle notes in pdf to pptx " caption="Making notes in Adobe Reader">}}


Whereas, Microsoft Edge uses a blue one.



{{< figure align=center src="images/conversion-pdf-pptx-adv-02-1024x546.png" alt="pdf to pptx comments and notes">}}


If such PDF files are converted into a PPTX presentation, then all notes are transferred to the PPTX file.

### How Can we Fix It?

In terms of the PDF standard, we are dealing with pages' content and additional elements named annotation. Let’s write a small piece of C# code to investigate which kinds of annotations are present in such documents.



After execution, we will get the result something like this:

```
1 Andrew Ink #E52237
1 Andrew Popup #000000
1 Andrew Square #E52237
1 Andrew Popup #000000
```

This means that there are three types of annotations on the PDF's page:

*   **Ink** – it’s our pencil drawing,
*   **Square** – our rectangle drawing,
*   **Popup** – a pop-up annotation displays text in a pop-up window for entry and editing. It shall not appear alone but is associated with a markup annotation, its parent annotation, and shall be used for editing the parent’s text. In our case, Popup annotation linked with Ink and Square. It shall have no appearance stream, so it will not affect to PDF to PPTX conversion.

### Remove Annotations in PDF to PPTX Conversion

So, in order to remove extra drawings in PDF, we should remove **Ink** and **Square** annotations. The following are the steps to perform this operation.

*   Access the annotations using the [Page.Annotations][4] property.
*   Filter the annotations by type.
*   Loop through the annotations and remove them one by one using [Page.Annotations.Delete(Annotation)][5] method.

The C# code snippet below shows one of the possible ways to remove annotation in PDF to PPTX conversion:



As mentioned above, the presenter can use different tools and colors for comments, and we can (if needed) tune the last sample. For example, we can remove only red (color code **#E52237**) annotations or certain presenter’s annotations.

Let's try another way to improve graphic content in PDF to PPTX conversion.

## C# PDF to PPTX - Separate Decoration Graphics from Content Images {#Separate-Decoration-Graphics-from-Content-Images}

While converting PDF into PPTX, usually all images in the PDF file are grouped into a single background image in the output. It’s not always convenient and Aspose.PDF for .NET has a special mode that can change the converter's behavior while converting PDF to PPTX.

To enable this mode, you can set the [SeparateImages][6] property to **true**. The following code snippet shows how to use this option in PDF to PPTX conversion in C#:



Thus, the slide from the previous example will be split into 3 images.



{{< figure align=center src="images/conversion-pdf-pptx-adv-03-1024x577.png" alt="decoration images in pdf to pptx">}}


It should be noted that it is not always possible to accurately separate the background images from the content images. Therefore, the converter can sometimes make mistakes and add extra elements to the content.

## Conclusion

In this article, you learned how to handle comments and decoration graphics in PDF to PPTX C# conversion. You can evaluate the working quality of our PDF to PPTX converter using a fully functional free web application - [Aspose.PDF PPTX Converter][7].

## See Also

*   [Convert PDF to PPTX using C#][8]




[1]: https://blog.aspose.com/2020/03/18/convert-pdf-to-powerpoint-ppt-pptx-in-csharp-net/
[2]: #Handle-Notes-or-Comments
[3]: #Separate-Decoration-Graphics-from-Content-Images
[4]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/annotations
[5]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations.annotationcollection/delete/methods/1
[6]: https://apireference.aspose.com/pdf/net/aspose.pdf/pptxsaveoptions/properties/separateimages
[7]: https://products.aspose.app/pdf/conversion/pdf-to-pptx
[8]: https://blog.aspose.com/2020/03/18/convert-pdf-to-powerpoint-ppt-pptx-in-csharp-net/





