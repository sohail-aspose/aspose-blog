---
title: 'Aspose.Words for .NET 20.3 is released!'
seoTitle: "Aspose.Words for .NET Standard for Xamarin.iOS Mac and Android"
description: "Xamarin developers can use Aspose.Words for .NET Standard in Xamarin.iOS 10.14 or newer, Xamarin.Mac 3.8 or newer and with Xamarin.Android 8.0 or newer."
date: Tue, 10 Mar 2020 12:37:17 +0000
draft: false
url: /2020/03/10/aspose.words-for-.net-20.3-released/
author: Andrey Noskov
summary: ''
tags: ['Aspose.Words for .NET', 'PDF to Word C#', 'Word to pdf conversion C#', 'insert Chart', 'insert online video', 'new release of Aspose.Words', 'release notes', 'word to pdf .net core', 'word to pdf c#', 'word to pdf in .NET', 'word to pdf programmatically']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words_.png" alt="">}}


This month we managed to deliver 72 improvements and fixes including 18 Enterprise and Priority support issues. Totally, 110 issues have been processed in the latest release of Aspose.Words for .NET.

## Updates for Xamarin Platform

Starting with Aspose.Words 20.3, the support of Xamarin is changed. In earlier versions, we provided separate DLLs for Xamarin.Android, Xamarin.Mac and Xamarin.iOS. Now Xamarin developers can use Aspose.Words for .NET Standard in all the above-mentioned platforms. According to the [.NET Standard documentation][1], Aspose.Words for .NET Standard 2.0 can be used with Xamarin.iOS 10.14 or newer, Xamarin.Mac 3.8 or newer and with Xamarin.Android 8.0 or newer.

## Salient Features and Improvements

In the latest release, several new features have been introduced. The most notable are:

*   _FindReplaceOptions_ class is extended with new properties.
*   Added a new public property _SaveOptions.UpdateLastPrintedProperty_.
*   Supported dynamic stretching of an image within textbox bounds preserving the ratio of the image for the LINQ Reporting Engine.

We have almost completed the first version of 3D Effects rendering through the OpenGL feature, however, it was decided to delay the release for thorough testing and experimenting with the new functionality.

Furthermore, we had a major overhaul of the footnote balancing algorithm as it did not work properly in a combination with paragraph rules. The test output has significantly improved for many documents and like always, a number of fixes related to CJK spacing for Japanese texts, handling of hidden paragraphs whose properties affect layout still, clipping logic to account for a rare condition, and etc. are introduced.

We have also released the latest version of Aspose.Words for Java along with Aspose.Words for .NET. We are happy to introduce huge performance and memory improvements in Aspose.Words for Java 20.3 by performing NodeCollectionEnumerator algorithm optimization, removing Ref<T> objects creation from nested cycles, blank document loading optimization, and using arraycopy for small arrays.




[1]: https://docs.microsoft.com/en-us/dotnet/standard/net-standard





