---
title: 'Create Survey Form from JSON Markup using C#'
date: Sat, 26 Feb 2022 12:31:24 +0000
draft: false
url: /2022/02/26/create-survey-form-from-json-markup-using-csharp/
author: ''Muzammil Khan''
summary: 'You can easily generate surveys, quizzes, and ready-to-print OMR answer sheets from JSON markup programmatically. In this article, you will learn **how to create a survey form from JSON markup using C#**.'
tags: ['C# OMR API', 'Create Survey in C#', 'JSON to Survey C#', 'OMR Survey C#', 'Survey from JSON using C#']
categories: ['Aspose.Total Product Family', 'Aspose.OMR Product Family']
---



{{< figure align=center src="images/create-survey-form-from-json-markup-using-csharp.jpg" alt="Create Survey Form from JSON Markup using C#">}}


Surveys play a vital role in market research for companies or organizations to grow their businesses. They use survey forms to collect customer feedback, user reviews, or opinions. Survey forms usually include multi-choice questions to mark user inputs. We can easily generate surveys, quizzes, and ready-to-print OMR answer sheets from JSON markup programmatically. JSON allows storing and transporting data that can be parsed and processed programmatically. In this article, we will learn **how to create a survey form from JSON markup using C#**.

The following topics shall be covered in this article:

*   [C# OMR API to Create Survey Form from JSON][1]
*   [Create OMR Survey Form from JSON Markup][2]
*   [Generate Survey in PDF from JSON Markup][3]

## C# OMR API to Create Survey Form from JSON {#CSharp-OMR-API-to-Create-Survey-Form-from-JSON}

For creating survey forms from JSON markup, we will be using the [Aspose.OMR for .NET API][4]. It allows designing, creating, and recognizing answer sheets, tests, MCQ papers, quizzes, feedback forms, surveys, and ballots. Please either [download][5] the DLL of the API or install it using [NuGet][6].

```
PM> Install-Package Aspose.OMR
```

## Create OMR Survey Form from JSON Markup using C# {#Create-OMR-Survey-Form-from-JSON-Markup}

We can create a survey form from JSON markup by following the steps given below:

*   Firstly, create an instance of the [_**OmrEngine**_][7] class.
*   Next, call the **_[GenerateJSONTemplate][8]_** method with JSON markup file path as an argument.
*   After that, get results as an object of the **_[GenerationResult][9]_** class.
*   Finally, call the **_[Save][10]_** method to save template images and OMR template. It takes the path of the local disk folder and name of the template as arguments.

The following code example demonstrates **how to create an OMR survey form template from JSON markup using C#**.

{{< gist aspose-com-gists 77ffea3f2a23f7a5e93f78dfdf90114f "CreateSurveyFormFromJSON_CSharp_GenerateOMRTemplate.cs" >}}



{{< figure align=center src="images/Create-OMR-Survey-Form-from-JSON-Markup-724x1024.png" alt="" caption="Create OMR Survey Form from JSON Markup using C#">}}


We have used the following JSON template markup in the code example mentioned above.

{{< gist aspose-com-gists 77ffea3f2a23f7a5e93f78dfdf90114f "CreateSurveyFormFromJSON_CSharp_JSONTemplate.json" >}}

## Generate Survey in PDF from JSON Markup using C# {#Generate-Survey-in-PDF-from-JSON-Markup}

We can also save the generated survey form in a PDF document by following the steps mentioned above. However, we just need to call the **_[SaveAsPdf(string folder, string name)][11]_** method instead of the **_Save_** method in the last step.

{{< gist aspose-com-gists 77ffea3f2a23f7a5e93f78dfdf90114f "CreateSurveyFormFromJSON_CSharp_GenerateAndSaveAsPDF.cs" >}}



{{< figure align=center src="images/Create-Survey-in-PDF-from-JSON-Markup.jpg" alt="Create Survey in PDF from JSON Markup using C#" caption="Create Survey in PDF from JSON Markup using C#.">}}


## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][12] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned **how to create an OMR survey template from JSON markup** and generate survey images. We have also seen **how to save the generated survey in a PDF document** programmatically. Besides, you can learn more about Aspose.OMR for .NET API using the [documentation][13]. In case of any ambiguity, please feel free to contact us on the [forum][14].

## See Also

*   [Create OMR Template from Text Markup using Aspose.OMR for .NET][15]




[1]: #CSharp-OMR-API-to-Create-Survey-Form-from-JSON
[2]: #Create-OMR-Survey-Form-from-JSON-Markup
[3]: #Generate-Survey-in-PDF-from-JSON-Markup
[4]: https://products.aspose.com/omr/net/
[5]: https://downloads.aspose.com/omr/net
[6]: https://www.nuget.org/packages/aspose.omr
[7]: https://apireference.aspose.com/omr/net/aspose.omr.api/omrengine
[8]: https://apireference.aspose.com/omr/net/aspose.omr.api/omrengine/methods/generatejsontemplate
[9]: https://apireference.aspose.com/omr/net/aspose.omr.generation/generationresult
[10]: https://apireference.aspose.com/omr/net/aspose.omr.generation/generationresult/methods/save
[11]: https://apireference.aspose.com/omr/net/aspose.omr.generation/generationresult/methods/saveaspdf
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/omr/net/
[14]: https://forum.aspose.com/c/omr/38
[15]: https://blog.aspose.com/2019/10/07/create-omr-template-from-text-markup-using-aspose.omr-for-.net/




