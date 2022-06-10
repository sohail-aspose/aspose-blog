---
title: 'Create EMF metafile image with Aspose.Imaging for .NET 3.9.0'
date: Tue, 23 Aug 2016 19:12:20 +0000
draft: false
url: /2016/08/23/create-emfwmf-metafile-with-aspose.imaging-for-.net-3.9.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2013/09/aspose-Imaging-for-net_100.png "aspose-Imaging-for-net_100") We are pleased to announce the release of Aspose.Imaging for .NET 3.9.0. The major development in this release is support for creating EMF metafile image. This release supports PSD file created/updated using SAI and GIMP2 tools. Support to export text as shapes while converting EMF metafile to SVG format has also been incorporated in this release.

## Create EMF Metafile Image

Aspose.Imaging for .Net now supports creating EMF metafile image. Aspose.Imaging for .Net provides the EmfRecorderGraphics2D class to create EMF metafile. Below provided sample code demonstrates how to create EMF metafile.

```
 private void Gen_EMF_Image()
{
    // EmfRecorderGraphics2D class provides you the frame or canvas to draw shapes on it.
    // Create an instance of EmfRecorderGraphics2D class. The constructor takes in 3 parameters:
    // 1. Instance of Imaging Rectangle class
    // 2. Instance of Imaging Size class
    // 3. Instance of Imaging Size class
    Aspose.Imaging.FileFormats.Emf.Graphics.EmfRecorderGraphics2D graphics = new Aspose.Imaging.FileFormats.Emf.Graphics.EmfRecorderGraphics2D(
        new Aspose.Imaging.Rectangle(0, 0, 1000, 1000),
        new Aspose.Imaging.Size(1000, 1000),
        new Aspose.Imaging.Size(100, 100));
    {
                
        // Create an instance of Imaging Pen class and mention its color.
        Aspose.Imaging.Pen pen = new Aspose.Imaging.Pen(Aspose.Imaging.Color.Bisque);
        // Draw a line by calling DrawLine method and passing x,y coordinates of 1st point and same for 2nd point along with color infor as Pen.
        graphics.DrawLine(pen, 1, 1, 50, 50);

        // Reset the Pen color.
        pen = new Aspose.Imaging.Pen(Aspose.Imaging.Color.BlueViolet, 3);
                
        // specify the end style of the line.
        pen.EndCap = LineCap.Round;

        // Draw a line by calling DrawLine method and passing x,y coordinates of 1st point and same for 2nd point along with color infor as Pen and end style of line.
        graphics.DrawLine(pen, 15, 5, 50, 60);

        // specify the end style of the line.
        pen.EndCap = LineCap.Square;

        // Draw a line by calling DrawLine method.
        graphics.DrawLine(pen, 5, 10, 50, 10);

        // specify the end style of the line.
        pen.EndCap = LineCap.Flat;

        // Draw a line by calling DrawLine method and passing parameters.
        graphics.DrawLine(pen, new Aspose.Imaging.Point(5, 20), new Aspose.Imaging.Point(50, 20));

        // Create an instance of HatchBrush class to define rectanglurar brush with with different settings.
        Aspose.Imaging.Brushes.HatchBrush hatchBrush = 
            new Aspose.Imaging.Brushes.HatchBrush() 
            { BackgroundColor = Aspose.Imaging.Color.AliceBlue, ForegroundColor = Aspose.Imaging.Color.Red, HatchStyle = HatchStyle.Cross };

        // Draw a line by calling DrawLine method and passing parameters.
        pen = new Aspose.Imaging.Pen(hatchBrush, 7);
        graphics.DrawRectangle(pen, 50, 50, 20, 30);

        // Draw a line by calling DrawLine method and passing parameters with different mode.
        graphics.BackgroundMode = Aspose.Imaging.FileFormats.Emf.Emf.Consts.EmfBackgroundMode.OPAQUE;
        graphics.DrawLine(pen, 80, 50, 80, 80);

        // Draw a polygon by calling DrawPolygon method and passing parameters with line join setting/style.
        pen = new Aspose.Imaging.Pen(new Aspose.Imaging.Brushes.SolidBrush(Aspose.Imaging.Color.Aqua), 3);
        pen.LineJoin = LineJoin.MiterClipped;
        graphics.DrawPolygon(pen, new Aspose.Imaging.Point[] 
        { 
            new Aspose.Imaging.Point(10, 20), 
            new Aspose.Imaging.Point(12, 45), 
            new Aspose.Imaging.Point(22, 48), 
            new Aspose.Imaging.Point(48, 36), 
            new Aspose.Imaging.Point(30, 55), 
        });

        // Draw a rectangle by calling DrawRectangle method.
        pen.LineJoin = LineJoin.Bevel;
        graphics.DrawRectangle(pen, 50, 10, 10, 5);

        pen.LineJoin = LineJoin.Round;
        graphics.DrawRectangle(pen, 65, 10, 10, 5);

        pen.LineJoin = LineJoin.Miter;
        graphics.DrawRectangle(pen, 80, 10, 10, 5);

        // Call EndRecording method to produce the final shape. EndRecording method will return the final shape as EmfImage.
        // So create an instance of EmfImage class and initialize it with EmfImage returned by EndRecording method.
        using (Aspose.Imaging.FileFormats.Emf.EmfImage image = graphics.EndRecording())
        {
            Test(image, "Pens.emf");
        }
    }
}

// Test method will convert the metafile image to PDF formate.
private static void Test(Aspose.Imaging.FileFormats.Emf.EmfImage image, string fileName)
{
    // Create an instance of PdfOptions class.
    PdfOptions options = new PdfOptions();

    // Create an instance of EmfRasterizationOptions class and define different settings.
    EmfRasterizationOptions rasterizationOptions = new EmfRasterizationOptions();
    rasterizationOptions.PageSize = image.Size;
    options.VectorRasterizationOptions = rasterizationOptions;

    string outPath = fileName + ".pdf";
            
    // Call the save method to convert the EMF metafile image to PDF.
    image.Save(outPath, options);
} 
```

## Export Text As Shape While Converting EMF To SVG

Using Aspose.Imaging for .Net, developers can get text as shapes while converting EMF to SVG format. Aspose.Imaging for .Net provides the TextAsShapes property to get text as shape while converting EMF metafile. Below is the code demonstration.

```
 string path = @"CaplifeDisclaimer_eng.emf";
string destPath = @"CaplifeDisclaimer_eng_Path.svg";
string destTextPath = @"CaplifeDisclaimer_eng_Text.svg";

using (Aspose.Imaging.Image image = Aspose.Imaging.Image.Load(path))
{
    EmfRasterizationOptions emfRasterizationOptions = new EmfRasterizationOptions();
    emfRasterizationOptions.BackgroundColor = Aspose.Imaging.Color.White;
    emfRasterizationOptions.PageWidth = image.Width;
    emfRasterizationOptions.PageHeight = image.Height;

    image.Save(destPath, 
        new SvgOptions() 
        { 
            VectorRasterizationOptions = emfRasterizationOptions, 
            TextAsShapes = true 
        });
    image.Save(destTextPath, 
        new SvgOptions() 
        { 
            VectorRasterizationOptions = emfRasterizationOptions, 
            TextAsShapes = false 
        });
} 
```

## Enhancements

Following enhancements have been introduced in this release.

*   Support to load PSD file created/updated using SAI software/editing tool has been incorporated.
    
*   Support to load PSD file created/updated using GIMP2 software/editing tool has been incorporated.
    
*   Process of converting Djvu to PDF has been improved.
    
*   Process of converting Djvu image pages to PNG has been improved.
    
*   Process of updating text in PSD text layers has been improved.
    
*   ICC profiles for Jpeg2000 images have been implemented.
    
*   Process of rotate operation on raster image has been improved.
    
*   Process of converting TIFF to JPEG has been improved.
    
*   Process of extracting frames from a TIFF file has been improved.
    

Please refer to the release notes of [Aspose.Imaging for .NET 3.9.0][1] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the Public API Change section to know what has been changed in the public API since your current version.

## Aspose.Imaging for .Net Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for .Net API][2].
*   [Download Aspose.Imaging for .NET][3].
*   [Aspose.Imaging for .NET online documentation][4] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][5] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][6] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][8] for a chat.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.imaging-for-.net/default.aspx
[2]: https://www.aspose.com/products/imaging/net
[3]: https://downloads.aspose.com/imaging/net
[4]: https://docs.aspose.com/display/imagingnet/Home
[5]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx
[6]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[7]: https://github.com/aspose-imaging/Aspose.Imaging-for-.NET
[8]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx




