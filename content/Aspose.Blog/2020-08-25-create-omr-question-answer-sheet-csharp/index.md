---
title: 'Create OMR Sheet Checker or Scanner Software in C#'
seoTitle: "Create OMR Question and Bubble Sheet Checker or Scanner Software C#"
description: "You can create OMR sheet checker, scanner software for bubble question and answer sheet and perform OCR on templates using C# or VB.NET. OMR Creator Maker."
date: Tue, 25 Aug 2020 21:56:24 +0000
draft: false
url: /2020/08/25/create-omr-question-answer-sheet-csharp/
author: Farhan Raza
summary: ''
tags: ['Bubble Sheet Scanner', 'bubble answer sheet generator', 'multiple choice answer sheets', 'omr c#', 'omr sheet checker', 'omr sheet scanner software']
categories: ['Aspose.OMR Product Family']
---

Optical Mark Recognition, abbreviated as OMR, is frequently used to assess questionnaires, surveys, and other information collection standards. In this article, you can learn how to create and check the OMR question and bubble answer sheets using C# language in a .NET application. We will explore the following approaches briefly:

[OMR Template Creator and Checker API – Installation][1]  
[Create OMR Question Sheet Template, Image, and PDF File using C#][2]  
[Perform OMR on Multiple Choice Bubble Answer Sheet Images using C#][3]

## OMR Template Creator and Checker API – Installation {#section1}

For creating OMR templates and performing OMR operations in C# or VB.NET applications, firstly we need to install Aspose.OMR for .NET API. You can easily download it from [New Releases][4] or with following [NuGet][5] Command:

_Install-Package Aspose.OMR -Version 20.6.0_

Therefore, we are now ready to proceed for creating multiple choice question sheet resources with the API using C#:

## Create OMR Question Sheet Template, Image, and PDF File using C# {#section2}

Let us explore creating OMR question sheet resources. Here we will store sample questions in a TXT file which will later be utilized by OMR engine for creating the OMR question paper template, image and PDF file. Moreover, following is the text markup that we will be using as input for the OMR engine:

```
?text=Name__________________________________ Date____________

?grid=ID
	sections_count=8
#What is Aspose.OMR main function?
	() OCR () Capture human-marked data
	() There is no main function () Enhance images
#Can Aspose.OMR process not only scans, but also photos?
	() Yes, indeed! () No
#Aspose.OMR is available on any platform, because it is:
	() Cross-platform code () Cloud service
#Aspose.OMR works with any kind of OMR forms: tests, exams, questionnaires, surveys, etc.
	() Yes, indeed! () No
#Excellent recognition results can be achieved only for filled bubbles at least for:
	() 40% () 60% () 75% () 98%
#Do you have to mark up every question on the page?
	(Yes) Yes, that will help a lot! (No) No
#Rate your preference from 0 to 9 with "0" being preference towards performance
and "9" being preference towards flexibility.
	(0) (1) (2) (3) (4) (5) (6) (7) (8) (9)
#I found aspose omr to be a useful tool. (5 - strongly agree, 1 - strongly disagree)
	(5) (4) (3) (2) (1)

?text= Answer sheet section
?answer_sheet=MainQuestions
	elements_count=10
	columns_count=5

?text=Sign________________________________
```

Now we will be following these steps with C# code to create OMR Multiple Choice Question Sheet:

1.  Initialize [OMR engine][6]
2.  Call [GenerateTemplate][7] method with text markup
3.  Save OMR output question sheet

Following code snippet is based on these steps which show how to create OMR question sheet template, image, and PDF file using C#:

{{< gist aspose-com-gists f08b8b0277fe563d616a807aefce753d "CreateOMR.cs" >}}

So we have created OMR question paper as shown in the following screenshot. You may distribute papers by printing the generated PDF file or image as per your requirements.



{{< figure align=center src="images/Grid-724x1024.png" alt="OMR template">}}


## Perform OMR on Multiple Choice Bubble Answer Sheet Images using C# {#section3}

Finally, you would collect the responses on generated bubble answer sheets and then capture images, or scan them for performing OMR using C#. In this example, let us consider the following sample image. Aspose.OMR for .NET API will create a comma-separated (CSV) file as the output of performing OMR.



{{< figure align=center src="images/Sheet1-768x1024.jpg" alt="create omr">}}


Let us follow these steps for performing OMR using C#:

1.  Specify the template file path
2.  Specify the scanned image file path
3.  Initialize [TemplateProcessor][8]
4.  Recognize images with [RecognizeImage][9] method
5.  Write CSV output in TXT file

The code snippet below shows how to perform OMR on multiple-choice bubble answer sheet images in C#:

{{< gist aspose-com-gists f08b8b0277fe563d616a807aefce753d "PerformOMR.cs" >}}

The following screenshot shows how efficiently and accurately the output CSV file is generated with Aspose.OMR for .NET API. This CSV information can now be further processed as per your system design.



{{< figure align=center src="images/OCR-answer-sheet-1.png" alt="perform omr">}}


## Conclusion

In a nutshell, we have learned how to create question sheets and later perform OMR operations to mark bubble answer sheet images using C#. This OMR sheets creation and then performing OMR operations on images is very helpful in different research methods. Moreover, in case of any concerns or queries, you can reach out to us via [Free Support Forums][10].

## See Also

[Print PDF Documents Programmatically using C#][11]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: https://downloads.aspose.com/omr/net
[5]: https://www.nuget.org/packages/Aspose.OMR
[6]: https://apireference.aspose.com/omr/net/aspose.omr.api/omrengine
[7]: https://apireference.aspose.com/omr/net/aspose.omr.api/omrengine/methods/generatetemplate
[8]: https://apireference.aspose.com/omr/net/aspose.omr.api/templateprocessor
[9]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr/methods/recognizeimage/index
[10]: https://forum.aspose.com/c/omr
[11]: https://blog.aspose.com/2020/07/09/print-pdf-csharp/





