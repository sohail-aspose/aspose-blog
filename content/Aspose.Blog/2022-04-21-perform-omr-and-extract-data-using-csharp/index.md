---
title: 'Perform OMR and Extract Data using C#'
seoTitle: "Perform OMR and Extract Data using C# | Extract OMR Data from Images"
description: "Programmatically perform OMR and extract data using C# with Aspose.OMR for .NET API. Extract OMR data from scanned images programmatically and save as CSV."
date: Thu, 21 Apr 2022 16:56:28 +0000
draft: false
url: /2022/04/21/perform-omr-and-extract-data-using-csharp/
author: Muzammil Khan
summary: 'You can easily perform OMR operations on scanned images of survey forms or test sheets programmatically, and read user inputs programmatically in .NET applications. In this article, you will learn **how to perform OMR and extract data using C#**.'
tags: ['Get OMR Data C#', 'OMR', 'OMR in C#', 'OMR on Images', 'OMR on Scanned Images', 'OMR using C#', 'Perform OMR Operation C#']
categories: ['Aspose.OMR Product Family']
---



{{< figure align=center src="images/perform-omr-and-extract-data-using-csharp.jpg" alt="Perform OMR and Extract Data using C#">}}


Optical mark recognition (OMR) allows the reading and capturing of data marked on a special type of document form. This document form could be a test or a survey, consisting of bubble or square inputs filled by users. We can easily perform OMR operations on the scanned images of such survey forms or test sheets and read the user inputs programmatically in .NET applications. In this article, we will learn **how to perform OMR and extract data using C#**.

The following topics shall be covered in this article:

*   [C# OMR API to Perform OMR and Extract Data][1]
*   [Perform OMR and Extract Data from Image][2]
*   [Perform OMR and Extract Data from Multiple Images][3]
*   [Get OMR Results with Threshold][4]
*   [OMR Operation with Recalculation][5]

## C# OMR API to Perform OMR and Extract Data {#CSharp-OMR-API-to-Perform-OMR-and-Extract-Data}

For performing OMR operations and exporting data from images, we will be using the [Aspose.OMR for .NET API][6]. It allows designing, creating, and recognizing answer sheets, tests, MCQ papers, quizzes, feedback forms, surveys, and ballots. Please either [download][7] the DLL of the API or install it using [NuGet][8].

```
PM> Install-Package Aspose.OMR
```

## Perform OMR and Extract Data from Image {#Perform-OMR-and-Extract-Data-from-Image}

In order to perform OMR operation on an image, we need the prepared OMR template (.omr) and the image (user-filled forms/sheets) to perform OMR on. We can perform an OMR operation on an image and extract data by following the steps given below:

1.  Firstly, create an instance of the **_[OmrEngine][9]_** class.
2.  Next, call the **_[GetTemplateProcessor()][10]_** method and initialize **_[TemplateProcessor][11]_** class object. It takes the OMR template file path as an argument.
3.  Then, get the **_[RecognitionResult][12]_** object by calling the **_[RecognizeImage()][13]_** method with the image path as an argument.
4.  After that, get recognition results as CSV strings using the **_[GetCsv()][14]_** method.
5.  Finally, save the CSV result as a CSV file on the local disk.

The following code sample shows **how to perform OMR on an image and extract data in CSV format using C#**.

{{< gist aspose-com-gists 2c6d45fd5c4fa67c9bd9d7e4268152a2 "PerformOMR_CSharp_OMROnImage.cs" >}}



{{< figure align=center src="images/Perform-OMR-and-Extract-Data-from-Images-1024x682.jpg" alt="Perform OMR and Extract Data from Images" caption="Perform OMR and Extract Data from images.">}}


The OMR template used in the above code example can be downloaded from [here][15].

## Perform OMR and Extract Data from Multiple Images {#Perform-OMR-and-Extract-Data-from-Multiple-Images}

We can perform OMR operations on multiple images and extract data in a separate CSV file for each image by following the steps mentioned earlier. However, we need to repeat steps # 3, 4, and 5 for all the images one by one.

The following code sample shows **how to perform OMR on multiple images and extract data in CSV format using C#**.

{{< gist aspose-com-gists 2c6d45fd5c4fa67c9bd9d7e4268152a2 "PerformOMR_CSharp_OMROnMultipleImages.cs" >}}

The API also provides functionality to detect and recognize any barcodes available on the image during OMR operation. It is the default feature of the OMR operation. We can perform OMR operations and recognize barcodes by following the steps mentioned earlier.

## Get OMR Results with Threshold {#Get-OMR-Results-with-Threshold}

We can apply the threshold while performing OMR operations on images. The value of the threshold could be from 0 to 100 depending on the requirements. The higher the value of the threshold, the API becomes more strict regarding highlight the answers. Please follow the steps mentioned earlier to perform OMR with the threshold. However, we just need to call the overloaded _**[RecognizeImage(string, int32)][16]**_ method in step # 3. It takes the image file path and the threshold value as arguments.

The following code sample shows **how to perform OMR with threshold value using C#**.

{{< gist aspose-com-gists 2c6d45fd5c4fa67c9bd9d7e4268152a2 "PerformOMR_CSharp_OMRwithThreshold.cs" >}}

## OMR Operation with Recalculation {#OMR-Operation-with-Recalculation}

In certain cases, we may need to recalculate the OMR results with different threshold values. For this purpose, we can configure the API to automatically recalculate using [**TemplateProcessor.recalculate()**][17] method. It allows processing an image multiple times by changing the threshold setting to get the desired result. We can perform OMR operation with recalculation by following the steps given below:

1.  Firstly, create an instance of the **_[OmrEngine][18]_** class.
2.  Next, call the **_[GetTemplateProcessor()][19]_** method and initialize **_[TemplateProcessor][20]_** class object. It takes the OMR template file path as an argument.
3.  Then, initialize the Stopwatch object and start the timer.
4.  Next, get the **_[RecognitionResult][21]_** object by calling the **_[RecognizeImage()][22]_** method with the image path as an argument.
5.  Then, stop the timer and export recognition results as a CSV string using the **_[GetCsv()][23]_** method.
6.  Next, save the CSV result as a CSV file on the local disk.
7.  Then, restart the timer using the Restart() method.
8.  Next, call the **_[Recalculate()][24]_** method. It takes the RecognitionResult object and the threshold value as arguments.
9.  After that, stop the timer and export recognition results as a CSV string using the **_GetCsv()_** method.
10.  Finally, save the CSV result as a CSV file on the local disk.

The following code sample shows **how to perform OMR with the recalculation method using C#**.

{{< gist aspose-com-gists 2c6d45fd5c4fa67c9bd9d7e4268152a2 "PerformOMR_CSharp_OMRwithRecalculation.cs" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][25] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   perform OMR operation on images and extract data in CSV format using C#;
*   apply threshold setting while performing OMR on images;
*   recalculate OMR results in an automotive process programmatically.

Besides, you can learn more about Aspose.OMR for .NET API using the [documentation][26]. In case of any ambiguity, please feel free to contact us on the [forum][27].

## See Also

*   [Create Survey Form from JSON Markup using C#][28]
*   [Create OMR Template from Text Markup using Aspose.OMR for .NET][29]




[1]: #CSharp-OMR-API-to-Perform-OMR-and-Extract-Data
[2]: #Perform-OMR-and-Extract-Data-from-Image
[3]: #Perform-OMR-and-Extract-Data-from-Multiple-Images
[4]: #Get-OMR-Results-with-Threshold
[5]: #OMR-Operation-with-Recalculation
[6]: https://products.aspose.com/omr/net/
[7]: https://downloads.aspose.com/omr/net
[8]: https://www.nuget.org/packages/aspose.omr
[9]: https://apireference.aspose.com/omr/net/aspose.omr.api/omrengine
[10]: https://apireference.aspose.com/omr/net/aspose.omr.api/omrengine/methods/gettemplateprocessor
[11]: https://apireference.aspose.com/omr/net/aspose.omr.api/templateprocessor
[12]: https://apireference.aspose.com/omr/net/aspose.omr.model/recognitionresult
[13]: https://apireference.aspose.com/omr/net/aspose.omr.api.templateprocessor/recognizeimage/methods/1
[14]: https://apireference.aspose.com/omr/net/aspose.omr.model/recognitionresult/methods/getcsv
[15]: https://gist.github.com/aspose-com-gists/2c6d45fd5c4fa67c9bd9d7e4268152a2#file-performomr_csharp_sheet-omr
[16]: https://apireference.aspose.com/omr/net/aspose.omr.api.templateprocessor/recognizeimage/methods/1
[17]: https://apireference.aspose.com/java/omr/com.aspose.omr/TemplateProcessor#recalculate-com.aspose.omr.RecognitionResult-int-
[18]: https://apireference.aspose.com/omr/net/aspose.omr.api/omrengine
[19]: https://apireference.aspose.com/omr/net/aspose.omr.api/omrengine/methods/gettemplateprocessor
[20]: https://apireference.aspose.com/omr/net/aspose.omr.api/templateprocessor
[21]: https://apireference.aspose.com/omr/net/aspose.omr.model/recognitionresult
[22]: https://apireference.aspose.com/omr/net/aspose.omr.api.templateprocessor/recognizeimage/methods/1
[23]: https://apireference.aspose.com/omr/net/aspose.omr.model/recognitionresult/methods/getcsv
[24]: https://apireference.aspose.com/omr/net/aspose.omr.api/templateprocessor/methods/recalculate
[25]: https://purchase.aspose.com/temporary-license
[26]: https://docs.aspose.com/omr/net/
[27]: https://forum.aspose.com/c/omr/38
[28]: https://blog.aspose.com/2022/02/26/create-survey-form-from-json-markup-using-csharp/
[29]: https://blog.aspose.com/2019/10/07/create-omr-template-from-text-markup-using-aspose.omr-for-.net/




