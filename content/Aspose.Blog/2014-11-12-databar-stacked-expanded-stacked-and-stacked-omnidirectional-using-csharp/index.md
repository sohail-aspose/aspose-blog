---
title: 'Work with DataBar Stacked, DataBar Expanded Stacked and DataBar Stacked Omnidirectional Symbologies using C#'
date: Wed, 12 Nov 2014 18:02:35 +0000
draft: false
url: /2014/11/12/databar-stacked-expanded-stacked-and-stacked-omnidirectional-using-csharp/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Total Product Family', 'Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.BarCode for .NET][1] 6.6.0. This new release supports the DataBar Stacked, DataBar Expanded and DataBar Stacked Omnidirectional symbologies. Developers can now add generation and recognition operations to their .NET, Compact framework and Silverlights applications. DataBar is really a family of barcode symbologies.

## Support for DataBar Stacked

We've added support for DataBar stacked generation and recognition. DataBar stacked is a variation of the RSS-14 symbology that is stacked in two rows and is used when the normal symbol would be too wide for the application. The sample code below specifies the use of Aspose.BarCode API.

### DataBar Stacked Generation```
// Initialize BarCodeBuilder class object
using (BarCodeBuilder builder = new BarCodeBuilder())
{
    // Set code text
    builder.CodeText = "(01)00012345678905";
    // Set symbology type
    builder.SymbologyType = Symbology.DatabarStacked;
    // Save barcode image
    builder.Save("databarstacked.png");
}
```

Result:



{{< figure align=center src="images/databarstacked1.png" alt="">}}


### DataBar Stacked Recognition```
// Define BarCodeReader class object
BarCodeReader reader;
// Initialize reader object
reader = new BarCodeReader("databarstacked.png", BarCodeReadType.DatabarStacked);
// Scan barcode image
if (reader.Read())
{
    // Get code text
    Console.WriteLine(reader.GetCodeText());
}
// Dispose reader object
reader.Close();
```

Result: (01)0001234567890

## Support for DataBar Expanded Stacked

We've added support for DataBar expanded stacked generation and recognition. A DataBar expanded stacked barcode can grow vertically, it can encode a large amount of data in small space. Below is an Aspose.BarCode API code sample that shows how to use it.

### DataBar Expanded Stacked Generation```
// Initialize BarCodeBuilder class object
using (BarCodeBuilder builder = new BarCodeBuilder())
{
    // Set code text
    builder.CodeText = "(01)90012345678908(3932)04055GBP";
    // Set symbology type
    builder.SymbologyType = Symbology.DatabarExpandedStacked;
    // Save barcode image
    builder.Save("databarexpandedstacked.png");
}
```

Result:



{{< figure align=center src="images/databarexpandedstacked.png" alt="Databar Expanded Stacked code">}}


### DataBar Expanded Stacked Recognition```
// Define BarCodeReader class object
BarCodeReader reader;
// Initialize reader object
reader = new BarCodeReader("databarexpandedstacked.png", BarCodeReadType.DatabarExpandedStacked);
// Scan barcode image
if (reader.Read())
{
    // Get code text
    Console.WriteLine(reader.GetCodeText());
}
// Dispose barcode image
reader.Close();
```

Result: (01)90012345678908(3932)04055GBP

## Support of DataBar Omnidirectional Stacked

We've added support for DataBar omnidirectional stacked generation and recognition. It is  perfectly suitable for POS (point of sale) applications. Below, you'll find a Aspose.BarCode API code sample that shows how to use it.

### DataBar OmniDirectional Stacked Generation```
// Initialize BarCodeBuilder class object
using (BarCodeBuilder builder = new BarCodeBuilder())
{
    // Set barcode text
    builder.CodeText = "(01)00034567890125";
    // Set symbology type
    builder.SymbologyType = Symbology.DatabarStackedOmniDirectional;
    // Save barcode image
    builder.Save("databarstackedomnidirectional.png");
}
```

Result:



{{< figure align=center src="images/databarstackedomnidirectional.png" alt="Databar Stacked Omnidirectional code">}}


### DataBar Omnidirectional Stacked Recognition```
// Define BarCodeReader class object
BarCodeReader reader;
// Initialize reader object
reader = new BarCodeReader("databarstackedomnidirectional.png", BarCodeReadType.DatabarStackedOmniDirectional);
// Scan barcode image
if (reader.Read())
{
    // Get barcode text
    Console.WriteLine(reader.GetCodeText());
}
// Dispose reader object
reader.Close();
```

Result: (01)0003456789012

To view a complete list of API features and try the API, please visit the following page and [download the latest version of Aspose.BarCode for .NET][2]. If you need any help, please feel free to ask in the [Aspose.BarCode forum][3]. For more details, please visit the Aspose.BarCode for .NET documentation.




[1]: https://products.aspose.com/barcode/net
[2]: https://downloads.aspose.com/barcode/net
[3]: http://forum.aspose.com




