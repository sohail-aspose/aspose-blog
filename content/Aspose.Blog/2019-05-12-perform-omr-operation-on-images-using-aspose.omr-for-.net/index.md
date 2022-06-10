---
title: 'Perform OMR operation on Images using Aspose.OMR for .NET'
date: Sun, 12 May 2019 18:20:11 +0000
draft: false
url: /2019/05/12/perform-omr-operation-on-images-using-aspose.omr-for-.net/
author: Asad Ali
summary: ''
tags: ['Asad Ali']
categories: ['Aspose.OMR Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2019/05/Aspose_OMR-for-net-256x256.png)  
Wait is over guys! [Aspose.OMR or .NET][1] has been released and now is available over NuGet Gallery to be used in .NET Application. As shared in pre-release announcement of the API, Aspose.OMR has been provided as simple and lightweight solution that makes performing OMR operation on images a breeze. In this blog post, we will try to go through maximum features API is offering to its users. Without waiting so much, let’s dive into information which will be helpful to use API first time and perform OMR operations over images.  

## Perform OMR using Aspose.OMR

API provides simple to use features for performing OMR operation. For a simple OMR operation, you only need two things; the prepared template (special markers will be drawn over user’s form) and the images to perform OMR operation on. Aspose.OMR provides [TemplateProcessor.RecognizeImage()][2] method that takes an image path and returns a string output. The following code snippet demonstrates the usage of OmrEngine and [TemplateProcessor][3] to perform OMR on two images.  
  
{{< gist aspose-com-gists 9351fac3e25a64343d5920a7770ded08 "Examples-CSharp-PerformOMR-PerformOMROnImages-1.cs" >}}

Well, we are not finished yet. The things would get more exciting because this API also provides a threshold setting to fine-tune the result of OMR according to your needs. You can set the value of threshold from 0 to 100 depending upon your needs. A detailed example and demonstration can be seen over following link in API documentation:

*   [Perform OMR operation with threshold setting][4]

## Using API with Graphic Control

The most worth-mentioning feature API has been offered with is Graphic Control that can be added into your application and lets you manually correct the threshold and markup to see changes in real-time. A complete guide to use Graphic Control in your application has been given in API documentation and can be visited on following link:

*   [Using Aspose.OMR with Graphic Control][5]

## API Limitations

First version of the API also offers some following limitations which should be kept in view while working with it:

*   Recognition process works only with prepared templates (special markers will be drawn over the user’s form)
*   Performing OCR operation is also not supported for now
*   OMR operation will show results only in text format

We really hope that above guide will help you setting up the API for first time usage. In case we missed something here, you are always welcome to post your inquiries in our [support forum][6]. Do not forget to go through [release notes][7] page of the API. We further intend to introduce more enhancements and attractive features in future releases of the API. [Stay with us][8] in order to get latest updates about releases of the API.




[1]: http://nuget.org/packages/Aspose.OMR/19.4.0 "Aspose.OMR for .NET 19.4"
[2]: https://apireference.aspose.com/net/omr/aspose.omr.api/templateprocessor/methods/recognizeimage "TemplateProcessor.RecognizeImage"
[3]: https://apireference.aspose.com/net/omr/aspose.omr.api/templateprocessor "TemplateProcessor"
[4]: https://docs.aspose.com/display/omrnet/Perform+OMR+on+Images#PerformOMRonImages-PerformOMRoperationwithathresholdsetting "Perform OMR operation with threshold setting"
[5]: https://docs.aspose.com/display/omrnet/Working+with+Graphical+Control "Using Aspose.OMR with Graphic Control"
[6]: https://forum.aspose.com/c/omr "Aspose.OMR Support Forum"
[7]: https://docs.aspose.com/display/omrnet/Aspose.OMR+for+.NET+19.4+Release+Notes "Aspose.OMR for .NET 19.4 release notes"
[8]: https://blog.aspose.com/category/aspose-products/aspose-omr-product-family/ "Subscribe Aspose.OMR Blog"




