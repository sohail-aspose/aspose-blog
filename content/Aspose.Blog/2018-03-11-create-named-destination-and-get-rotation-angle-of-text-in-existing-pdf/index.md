---
title: 'Create Named Destination and Get Rotation Angle of Text in PDF using C#'
date: Sun, 11 Mar 2018 22:12:12 +0000
draft: false
url: /2018/03/11/create-named-destination-and-get-rotation-angle-of-text-in-existing-pdf/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'Create Named Destination in PDF', 'Get Rotation Angle of Text in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="">}}


As per the regular monthly release process, we are pleased to announce [Aspose.PDF for .NET 18.2][1]. The new version of Aspose.PDF for .NET has been released for .NET platform and is available now to be used in .NET applications. Since we have been providing an efficient and full of attractive features API to deal with PDF documents, we have introduced new exciting features in Aspose.PDF for .NET 18.2. In case you are going to use the new version of Aspose.PDF for .NET, we suggest you go through the detailed [release notes page][2] of the API. Each new feature and enhancement has been enlisted in release notes along with the fixes, which have been made against the bugs reported in the previous version(s) of the API.

## Create Named Destination in PDF using C#

One of the exciting features introduced in Aspose.PDF for .NET 18.2 is to create names destinations in existing PDF documents. If you want to change a destination without effecting any internal/external link inside a PDF document, you have to use the named destination. Creating named destinations manually can be a very tedious task – however, you can also create named destinations programmatically using Aspose.PDF for .NET 18.2. We have implemented the [Document.NamedDestinations][3] property which allows manipulating named destinations. [NamedDestinationCollection][4] has the following properties:

*   IAppointment this\[string name\]= Access to named destination; (getter and setter are implemented)
*   int Count = Number if named destinations;
*   string\[\] names = List of destination names;
*   Add(string name, IAppointment appointment = Create new named destination;
*   Remove(string name) = Remove named destination by its name.

Following example shows the usage of NamedDestinations:

```
Document pdf = new Document();
// Create document with 100 pages
for (int i = 1; i <= 100; i++)
{
 Page page = pdf.Pages.Add();
 page.AddStamp(new Aspose.Pdf.TextStamp("Page " + i));
   // Named destinations for every page
 pdf.NamedDestinations.Add("Page" + i, new XYZExplicitDestination(i, 0, 600, 0.5));
}
for (int i = 1; i <= 100; i++)
{
   // Create outlines (two outlines for every page)
 OutlineItemCollection item1 = new OutlineItemCollection(pdf.Outlines);
 item1.Destination = new NamedDestination(pdf, "Page" + i);
 item1.Title = "Page  " + i + "(1)";
 pdf.Outlines.Add(item1);

 OutlineItemCollection item2 = new OutlineItemCollection(pdf.Outlines);
 item2.Destination = new NamedDestination(pdf, "Page" + i);
 item2.Title = "Page  " + i + "(2)";
 pdf.Outlines.Add(item2);
}
 // Let's update on of the named destinations
pdf.NamedDestinations\["Page50"\] = new XYZExplicitDestination(50, 0, 100, 2);
pdf.Save("result.pdf");
```

## Get Rotation Angle of Text in PDF

In Aspose.PDF for .NET 17.5 version, we had introduced the feature of rotating the added text inside PDF document. However, we have been receiving feature requests from our customers, about determining the rotation angle of the text found using [TextFragmentAbsorber][5] class. The functionality to get rotation angle of the text has been implemented in Aspose.PDF for .NET 18.2 and can be achieved by using the following code snippet:

```
Document pdfDocument = new Document(myDir + "input.pdf");
TextFragmentAbsorber textFragmentAbsorber = new TextFragmentAbsorber("Ｒ");
// Accept the absorber for first page of document
pdfDocument.Pages\[4\].Accept(textFragmentAbsorber);

TextFragmentCollection textFragmentCollection = textFragmentAbsorber.TextFragments;
foreach (TextFragment tf in textFragmentCollection)
{
 Console.Out.WriteLine("Fragment: " + tf.Text + " " + tf.Rectangle);

 TextFragmentState state = tf.TextState;
 Console.Out.WriteLine("Rotation: " + state.Rotation);

 foreach (TextSegment ts in tf.Segments)
 {
  Console.Out.WriteLine("Segment: " + ts.Text + " " + ts.Rectangle);

  foreach (CharInfo cI in ts.Characters)
  {
   Console.Out.WriteLine(cI.Position);
  }
 }
}
```

## Miscellaneous Fixes

Besides the above-mentioned enhancements and features, we also have provided fixes against bugs reported in the previous version(s) of the Aspose.PDF for .NET. In order to check the complete list of issues that have been fixed in this release of Aspose.PDF for .NET, please check the [Release Notes][6] section of Aspose.PDF for .NET 18.2.

As it is always recommended to use the latest release of our API’s, so we suggest you please download the latest release [Aspose.PDF for .NET 18.2][7] and check following resources which will help you working with API:

*   [Home page for Aspose.PDF for .NET][8]
*   [Download Aspose.PDF for .NET 18.2][9]
*   [Aspose.PDF product family forum][10]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for .NET online documentation][11]– help documentation and API reference documents.
*   [Enable Blog Subscription][12]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][13] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Pdf/18.2.0
[2]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+18.2+Release+Notes
[3]: https://apireference.aspose.com/net/pdf/aspose.pdf/document/properties/nameddestinations
[4]: https://apireference.aspose.com/net/pdf/aspose.pdf/nameddestinationcollection
[5]: https://apireference.aspose.com/net/pdf/aspose.pdf.text/textfragmentabsorber/
[6]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+18.2+Release+Notes
[7]: https://www.nuget.org/packages/Aspose.Pdf/18.2.0
[8]: https://products.aspose.com/pdf/net
[9]: https://www.nuget.org/packages/Aspose.Pdf/18.2.0
[10]: https://forums.aspose.com/c/pdf
[11]: https://docs.aspose.com/display/pdfnet/Home
[12]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[13]: https://github.com/aspose-pdf/Aspose.PDF-for-.NET




