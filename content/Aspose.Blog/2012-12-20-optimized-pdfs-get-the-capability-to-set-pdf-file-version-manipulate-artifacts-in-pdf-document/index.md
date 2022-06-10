---
title: 'Optimized PDF''s, capability to set PDF file version, manipulate artifacts in PDF document'
date: Thu, 20 Dec 2012 17:07:21 +0000
draft: false
url: /2012/12/20/optimized-pdfs-get-the-capability-to-set-pdf-file-version-manipulate-artifacts-in-pdf-document/
author: Codewarior
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

![Aspose.Pdf icon][1]

We are glad to announce the release of [Aspose.Pdf for .NET 7.6.0][2]. This release version gives the capability to optimize the resultant PDF document by eliminating duplicate fonts, resources which are not used in document are removed and duplicate resources are joined as a single object. All this can be achieved using a single method OptimizeResources(..) in Document class. Furthermore, this release versions offers the feature to set the resultant file version i.e. v1.4, v1.5,, v1.6 etc. Even you can specify the file version when concatenating PDF documents.

```
Aspose.Pdf.Facades.PdfFileEditor pfe = new Aspose.Pdf.Facades.PdfFileEditor();
pfe.ConvertTo = PdfFormat.v_1_5;
pfe.Concatenate(new string[] { "Round-Corner-Table.pdf", "PdfWithText.pdf" }, "source-Merged-output.pdf");
```

In order to deal with Artifacts in PDF file, we have implemented a new class **Articat** and its descendants (FooterArtifact, HeaderArtifact, WatermarkArtifact, BackgroundArtifact). These classes allow to read artifacts on page, add, delete, artifacts, update artifact.

*   ArtifactCollection.Add(Artifact artifact) - allows to add artifact to the artifacts on page;
*   ArtifactCollection.Delete(int index) - deletes artifact by its index from the collection.

Please take a look over the following code snippet to add Artifacts to PDF file

```
 Document doc = new Document(TestSettings.GetInputFile("empty.pdf"));
Artifact artifact = new Artifact(Artifact.ArtifactType.Pagination, Artifact.ArtifactSubtype.Header);
FormattedText ft = new FormattedText("ABCD", System.Drawing.Color.Red, System.Drawing.Color.Blue);
ft.AddNewLineText("EFGH");
artifact.SetText(ft);

artifact.Position = new Point(100, 100);
artifact.Rotation = 45;
doc.Pages[1].Artifacts.Add(artifact);
```

The following code snippet shows how to remove Artifacts from PDF

```
 Document doc = new Document(TestSettings.GetInputFile("33603.pdf"));
System.Console.WriteLine(doc.Pages[1].Artifacts.Count);
int count = doc.Pages[1].Artifacts.Count;
doc.Pages[1].Artifacts.Delete(2);
doc.Save(TestSettings.GetOutputFile("34425-4.pdf")); 
```

Furthermore, we have greatly improved the performance and scale-ability of product in terms of performance and output document size

, specially while converting PDF file to Image formats. the PDF to XPS conversion features has been improved and likewise, the XPS to PDF conversion is also stabilized. Lots of other issues which were reported in earlier release versions are fixed in this latest release.

Please visit the following link for further details on what's new & fixed in [Aspose.Pdf for .NET 7.6.0][3].




[1]: http://www.aspose.com/Images/aspose.pdf-logo2.jpg
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry432898.aspx
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry432898.aspx




