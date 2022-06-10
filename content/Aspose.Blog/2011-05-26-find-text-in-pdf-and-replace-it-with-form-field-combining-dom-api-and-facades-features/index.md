---
title: 'Find Text in PDF and Replace it with Form Field: Combining DOM API and Facades Features'
date: Thu, 26 May 2011 07:12:40 +0000
draft: false
url: /2011/05/26/find-text-in-pdf-and-replace-it-with-form-field-combining-dom-api-and-facades-features/
author: Shahzad Latif
summary: ''
tags: ['Shahzad Latif', 'Add Form Field', 'Find Text', 'Find and remove text in PDF', 'Find and replace text in PDF', 'Replace Text']
---

In this blog post, I'm going to explain two things; first one is to show you an interesting feature of the merged Aspose.Pdf -- find and replace text with form field. This feature was previously not supported in Aspose.Pdf.Kit. The second one is to elaborate how you can combine the features from DOM API and Aspose.Pdf.Facades.

However, before I move forward, I would like you to have a look into my previous posts on the merged Aspose.Pdf, if you haven't read those already:

*   [New Aspose.Pdf for .NET – Merged Aspose.Pdf.Kit and Aspose.Pdf: A Sneak Peek!][1]
*   [Introduction to Merged Aspose.Pdf API][2]
*   [Performing Multiple Operations using Merged Aspose.Pdf: Comparing Two Approaches][3]

After reading the above posts, you'll have a better understanding of the example shown in this post.

Now, coming back to the example for this post, I'm going to find a particular text from the PDF file and then replace it with a form field. There are following four steps to achieve this goal:

1.  Find text and its location
2.  Remove text from the PDF
3.  Add form field at the location of the text
4.  Set form field attributes

All of these tasks can be completed using DOM API alone. However, I just want to show you that you can also combine different features from DOM API and Aspose.Pdf.Facades as well. That's why, I have divided it into two parts. The first two steps will be performed using DOM API, while the last two steps will be completed using Aspose.Pdf.Facades.



{{< figure align=center src="images/Find-and-Remove-Text.gif" alt="Find and Remove Text from PDF File">}}


This snapshot shows you the input PDF file. It contains the text which we want to replace with a form field; we'll replace the text 'Your File Format Experts!' with a text field.

In the following code snippet, you can see that DOM API is used to open the input PDF file and then find the particular text from that PDF. It is also used to find the location of the text and then remove the text from the PDF.

> //open document  
> Document pdfDocument = new Document("input.pdf");
> 
> //find text  
> TextFragmentAbsorber textFragmentAbsorber = new TextFragmentAbsorber("Your File Format Experts!");  
> pdfDocument.Pages\[1\].Accept(textFragmentAbsorber);
> 
> //determine text position  
> Rectangle textRect = textFragmentAbsorber.TextFragments\[1\].Rectangle;
> 
> //remove text  
> textFragmentAbsorber.TextFragments\[1\].Text = string.Empty;
> 
> //save document without text  
> pdfDocument.Save("TextRemoved.pdf");



{{< figure align=center src="images/Add-Field.png" alt="Add Field in the PDF file">}}


The second part of the example is using Aspose.Pdf.Facades to add a new form field in the PDF, at the same location where the text was found. It is also used to set the form field attributes like BackgroundColor and BorderColor.

You can also see the final output in the snapshot on the left. The text 'Your File Format Experts!' is replaced with a text field with red border color and gray background color. The field is added at the same location where the text was found.

The following code snippet shows you how to add the form field and set its attributes using Aspose.Pdf.Facades.

> //add form field on text position  
> FormEditor formEditor = new FormEditor("TextRemoved.pdf", "FieldAdded.pdf");
> 
> //use the location obtained from the text  
> formEditor.AddField(FieldType.Text, "NewFieldName", 1,  
> (float)textRect.LLX,  
> (float)textRect.LLY,  
> (float)textRect.URX,  
> (float)textRect.URY);
> 
> //set field attributes  
> FormFieldFacade fieldFacade = new FormFieldFacade();  
> formEditor.Facade = fieldFacade;  
> fieldFacade.BackgroundColor = System.Drawing.Color.Gray;  
> fieldFacade.BorderColor = System.Drawing.Color.Red;  
> formEditor.DecorateField("NewFieldName");
> 
> //save document with form field  
> formEditor.Save();

If you learn better by watching then I have prepared a video as well. In this video, I perform all the above steps using Visual Studio 2005. Please enjoy this video!

<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">https://youtu.be/wWReTmGQiK0</div></figure>

I hope you enjoyed this tutorial and learned something new about the merged version of Aspose.Pdf. If you have any questions or suggestions then we would love to hear from you! You may share your comments under this post.




[1]: https://blog.aspose.com/2011/05/04/new-aspose.pdf-for-.net-merged-aspose.pdf.kit-and-aspose.pdf-a-sneak-peek/
[2]: https://blog.aspose.com/2011/05/14/introduction-to-merged-aspose.pdf-api/
[3]: https://blog.aspose.com/2011/05/18/performing-multiple-operations-using-merged-aspose.pdf-comparing-two-approaches/



