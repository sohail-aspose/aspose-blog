---
title: 'Recognize Image from MemoryStream using OMR in C#'
seoTitle: "Recognize Image from MemoryStream using OMR in C#"
description: "You can recognize image from MemoryStream using OMR in C#. Scan folders containing images of survey, questionnaire with batch processing."
date: Thu, 10 Jun 2021 08:08:00 +0000
draft: false
url: /2021/06/10/recognize-images-from-memorystream-using-omr-in-csharp/
author: Farhan Raza
summary: 'You can recognize specific marks on images by performing optical mark recognition operations. For example, you can recognize bubbles filled for a questionnaire, survey, or an exam in the form of Multiple Choice Questions. Please refer to the following sections for further details.'
tags: ['OMR csharp', 'OMR image', 'OMR on MemoryStream', 'Optical Character Recognition csharp', 'recognize image']
categories: ['Aspose.OMR Product Family']
---



{{< figure align=center src="images/OMR-image-1.png" alt="">}}


You can recognize specific marks on images by performing optical mark recognition operations. For example, you can recognize bubbles filled for a questionnaire, survey, or an exam in the form of Multiple Choice Questions. Please refer to the following sections for further details:

*   [Optical Mark Recognition – C# API Installation][1]
*   [Recognize Image from MemoryStream using OMR in C#][2]
*   [Batch Processing the Images for Recognition with OMR using C#][3]

## Optical Mark Recognition – C# API Installation {#section1}

You can configure [Aspose.OMR for .NET][4] API in your C# applications by downloading the DLL from the [Downloads][5] sections, or via [NuGet][6] gallery with the following installation command:

```
PM> Install-Package Aspose.OMR
```

## Recognize Image from MemoryStream using OMR in C# {#section2}

Sometimes the images are stored in database or some remote resource and you can load those files in a MemoryStream. Likewise, there can be many scenarios where saving an image on the disk and then loading it for processing can be an overhead. So you can conveniently load the image into a Stream and perform OMR operations on it. Below are the steps to recognize an image from MemoryStream:

1.  Get the template to recognize.
2.  Initialize [OmrEngine][7] class object.
3.  Recognize image in the [MemoryStream][8] with the [RecognizeImage][9] method.
4.  Save output file with [RecognitionResult][10] class instance.

The following code shows how to recognize the image from a MemoryStream with OMR in C#:

{{< gist aspose-com-gists a9d1baca3598602f46e7d857cc19f730 "omr-stream.cs" >}}

## Batch Processing the Images for Recognition with OMR using C# {#section3}

You can process a batch of images in a folder and recognize the marks with optical mark recognition. Please follow the following steps for recognizing a batch of images:

1.  Get the OMR template to recognize.
2.  Get [RecognitionResult][11] of all the images using [RecognizeFolder][12] method.
3.  Save output as a CSV file.

The code below explains how to process a batch of images for optical mark recognition programmatically using C#:

{{< gist aspose-com-gists a9d1baca3598602f46e7d857cc19f730 "omr-recognize-batch.cs" >}}

## Get Free API License

You can evaluate the API without any limitations by requesting a [Free Temporary License][13].

## Conclusion

In this article, you have learned how to recognize an image from a MemoryStream using OMR in C#. It also discusses recognizing all the images in a folder and saving the output result as CSV, comma-separated values, files. Moreover, you can take a look at other features of the API by visiting the [Documentation][14]. You can always get in touch with us at [Free Support Forum][15] for any of your concerns.

## See Also

[Create OMR Sheet Checker or Scanner Application in C#][16]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: https://products.aspose.com/omr/net/
[5]: https://downloads.aspose.com/omr/net
[6]: https://www.nuget.org/packages/Aspose.OMR
[7]: https://apireference.aspose.com/omr/net/aspose.omr.api/omrengine
[8]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream?view=net-5.0
[9]: https://apireference.aspose.com/omr/net/aspose.omr.api/templateprocessor/methods/recognizeimage/index
[10]: https://apireference.aspose.com/omr/net/aspose.omr.model/recognitionresult
[11]: https://apireference.aspose.com/omr/net/aspose.omr.model/recognitionresult
[12]: https://apireference.aspose.com/omr/net/aspose.omr.api/templateprocessor/methods/recognizefolder
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/omr/net/developer-guide/
[15]: https://forum.aspose.com/c/omr
[16]: https://blog.aspose.com/2020/08/25/create-omr-question-answer-sheet-csharp/





