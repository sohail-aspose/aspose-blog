---
title: 'Create OMR Template from Text Markup using Aspose.OMR for .NET'
date: Mon, 07 Oct 2019 12:35:49 +0000
draft: false
url: /2019/10/07/create-omr-template-from-text-markup-using-aspose.omr-for-.net/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'OMR Template Editor', 'OMR in C#', 'OMR template']
categories: ['Aspose.OMR Product Family']
---



{{< figure align=center src="images/Aspose_OMR-for-net-256x256.png" alt=" OMR template from Text Markup">}}


An OMR Template is used to be compatible with the optical mark recognition software or API that you are using before it is printed. Designing a custom OMR Template allows your OMR Sheets to look better or they can be created in a way that they will look the same. Aspose.OMR for .NET is an API that can be used in .NET Applications and with its latest release, it allows you to create OMR template from Text Markup. Yes, generating surveys and test sheets from simple text markup is now achievable using the API. Thanks to Aspose and Congratulations to the Users that they can now get their personal test sheets. In the following section, you will be having insights into how to create OMR Template from Text Markup using [Aspose.OMR for .NET 19.7][1]. Without waiting so much, let’s dive then.

## Create OMR Template

Aspose.OMR for .NET provides the option to create OMR template (.omr) files and images by using simple text markup. [OmrEngine.GenerateTemplate][2] method that takes the path of the markup text file as a parameter, returns a [GenerationResult][3] object which contains the template image and the template (JSON that describes elements location on the image).  

You can further check following simple text markup which can be used to create OMR template using the API:

```
?text=Name\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ Date\_\_\_\_\_\_\_\_\_\_\_\_

?grid=ID
sections\_count=8
#What is Aspose.OMR main function?
() OCR () Capture human-marked data
() There is no main function () Enhance images
#Can Aspose.OMR process photos as well?
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
?answer\_sheet=MainQuestions
elements\_count=10
columns\_count=5

?text=Sign\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
```

Following code snippet can be used to process the above sample text markup to generate the OMR template file and the image of the sheet.

{{< gist aspose-com-gists 9351fac3e25a64343d5920a7770ded08 "Examples-CSharp-PerformOMR-GenerateOMRTemplate-1.cs" >}}  

When you are done with the processing of text markup, you will receive the following image generated at your end:



{{< figure align=center src="images/OMR-Template-Generation-724x1024.png" alt="OMR maekup in C#">}}


Please note that you cannot test this functionality while using the trial version of the API. You must use a valid license in order to create OMR Template. You can also [apply 30-days free temporary license][4] to test and evaluate the API without any trial version limitations.

## Improvements and API Changes

In addition to the above-introduced feature, some improvements have also been made regarding image processing. Some API changes are also included in the release since there has been a new functionality introduced.

We strongly recommend you check [release notes page][5] of the API for further details about the release and you are always encouraged to ask about API in our [public forums][6]. We will be back soon with more updates regarding revisions of the API and don’t forget to [subscribe][7] so that you will not miss any post.




[1]: https://www.nuget.org/packages/Aspose.OMR/19.7.0 "Aspose.OMR for .NET 19.7"
[2]: https://apireference.aspose.com/net/omr/aspose.omr.api/omrengine/methods/generatetemplate "OmrEngine.GenerateTemplate"
[3]: https://apireference.aspose.com/net/omr/aspose.omr.generation/generationresult "GenerationResult"
[4]: https://purchase.aspose.com/temporary-license "30-days temporary license for Aspose.OMR"
[5]: https://docs.aspose.com/display/omrnet/Aspose.OMR+for+.NET+19.7+Release+Notes "Aspose.OMR for .NET 19.7 Release Notes"
[6]: https://forum.aspose.com/c/omr "Aspose.OMR Support Forum"
[7]: https://blog.aspose.com/category/omr/ "Subscribe Aspose.OMR Blog"




