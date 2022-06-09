---
title: 'Create, Fill, or Edit Fillable PDF Forms Programmatically with C#'
seoTitle: ""
description: ""
date: Mon, 25 May 2020 22:23:00 +0000
draft: false
url: /2020/05/25/create-fill-edit-fillable-pdf-form-csharp/
author: Farhan Raza
summary: ''
tags: ['Extended Rights', 'Fill PDF Form', 'JavaScript', 'JavaScript in PDF', 'Preserve Extended Rights', 'fillable form', 'fillable pdf form', 'form fields']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/PDF_Form-1-239x300.png" alt="Fill PDF Form">}}


PDF forms are frequently used to collect data and information. For example, Questionnaires are usually designed to collect responses for survey purposes. We interact with different fillable PDF forms in today's digital world. Considering the huge scope and importance of PDF forms, [Aspose.PDF for .NET][1] API supports many features to work with PDF forms. Let us explore the following use cases using C# language in this article:

*   [Create Fillable PDF Forms using C#][2]
*   [Fill a Form Field in Existing PDF file using C#][3]
*   [Modify a Form Field in PDF Document using C#][4]
*   [Delete a Form Field in Existing PDF File using C#][5]
*   [Preserve Extended Rights of PDF Forms using C#][6]
*   [Use JavaScript in PDF Form using C#][7]

## Create Fillable PDF Forms using C# {#section1}

You can create a fillable PDF form from scratch using Aspose.PDF for .NET API. Here we will consider the basic example of adding two **TextBoxField** instances and **RadioButton**. However, one of the TextBoxField is single line while the other one is multi-line. Below are the steps to create a form in PDF document:

1.  Create an instance of [Document][8] class
2.  Add a blank page in PDF document
3.  Add [TextBox][9] Field in the form
4.  Set different properties of the fields including Font, Border etc.
5.  Add [Radio Button][10] in the form
6.  Save PDF document

Following code snippet shows how to create form in PDF using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Create_Fillable_Form_PDF.cs" >}}

The screenshot below shows output PDF document containing form fields as specified in above code snippet:



{{< figure align=center src="images/Fillable_Form_PDF-1024x615.png" alt="PDF form">}}


## Fill, Modify, or Delete Form Fields in Existing PDF using C#

As we have explored creating a form in PDF document using C#, Aspose.PDF for.NET API supports working with existing PDF forms as well. Let us discuss the following features of the API.

### i) Fill a Form Field in Existing PDF file using C# {#section2}

For filling the PDF forms, we will continue with the PDF document that was created in the example above. Below are the steps to fill fields in an existing PDF document:

1.  Load source PDF document
2.  Get [Textbox][11] Fields and fill values
3.  Get [Radio button field][12] and select an option from the group
4.  Save filled PDF form

Following code snippet follows these steps and explains how to fill fields in a PDF document using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Fill_Form_Field.cs" >}}

Below screenshot shows filled form fields of PDF form using C#:



{{< figure align=center src="images/Fill_Form_Field-1.png" alt="Fillable PDF">}}


### ii) Modify a Form Field in PDF Document using C# {#section3}

Sometimes you may need to change value in any field of a PDF form. Changing a value in a form field is a basic use case that can be achieved with below steps:

1.  Load the PDF form
2.  Get a specific field using its name
3.  Modify field value
4.  Save the updated PDF document

Following code snippet shows how to change a value in a form field of PDF document:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Modify_Form_Field.cs" >}}

It is noteworthy here that you can not only change the value of the form but other properties can be updated as well. For instance, the field has been marked as Read Only in the code snippet above.

### iii) Delete a Form Field in Existing PDF File using C# {#section4}

We have already learned about adding and filling PDF form fields. Now let us explore removing a form field. You need to follow the steps below:

1.  Load the PDF document
2.  Call Delete method with the name of the form field
3.  Save PDF Document

Following code snippet shows how to delete form field from PDF file using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Delete_Form_Field.cs" >}}

## Preserve Extended Rights of PDF Forms using C# {#section5}

A PDF form might have extended rights, also referred to as extended features, which you would want to preserve during form manipulation. You should save it incrementally while following the steps below:

*   Load the PDF document in Stream
*   Work with form
*   Save the file without any parameter

The following C# code snippet explains how to preserve extended rights of PDF form:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Extended_Features.cs" >}}

## Use JavaScript in PDF Form using C# {#section6}

You can use JavaScript in PDF form fields with Aspose.PDF for .NET API. Let us follow the below steps to achieve this requirement:

1.  Initiate an instance of Document class
2.  Add a [TextBoxField][13] on the first page at specific page coordinates
3.  Set up JavaScript
4.  Specify document action
5.  Save PDF document

Following code snippet shows how to add JavaScript in PDF form using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "JS_Form.cs" >}}

The JavaScript gets the current date and time of the system when PDF document is opened and that value is populated into a text box.

## Conclusion

In this article, we have learned different aspects of working with form in PDF documents. Creating, filling or editing PDF forms is simple with Aspose.PDF for .NET API. The API offers many such exciting features to work with different files. Let us know your feedback or comments via [Free Support Forum][14].

## See Also

[Fill, Create, or Edit Fillable PDF Forms Programmatically using Java][15]




[1]: https://products.aspose.com/pdf/net
[2]: #section1
[3]: #section2
[4]: #section3
[5]: #section4
[6]: #section5
[7]: #section6
[8]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf.forms/textboxfield
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf.forms/textboxfield
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.forms/textboxfield
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2020/07/20/create-fill-edit-fillable-pdf-form-field-java/





