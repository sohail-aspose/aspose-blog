---
title: 'Aspose.Imaging for .NET 1.9.0 Introduces a Simplified Image Creation Approach'
date: Mon, 22 Jul 2013 11:23:08 +0000
draft: false
url: /2013/07/22/aspose.imaging-for-.net-1.9.0-introduces-a-simplified-image-creation-approach/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---

[](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose.imaging-logo2.jpg)We are pleased to announce the release of Aspose.Imaging for .NET 1.9.0.

This month’s release includes some new features along with bug fixes. We have added some new overload methods to Graphics.DrawImage with parallelogram mode and ImageAttribute object parameters.  In this version we have introduce a simplified and optimized approach for creating images. Now you can pass any raster image to TiffFrame(). Please check the following code snippet for details:

```
 string pathTiff = @"TiffImage.TIF";
string pathJpg = @"JpegImage.jpg";
using (TiffImage output = (TiffImage)Image.Load(pathTiff))
{
    output.InsertFrame(1, new TiffFrame(pathJpg));
    output.Save("C:\\output.tif");
}
```

We have dropped support for .NET 1.1 Framework.

To see a complete list of features, fixes and to download Aspose.Imaging for .NET 1.9.0, [please visit the download page][1].




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.imaging-for-.net/entry483586.aspx




