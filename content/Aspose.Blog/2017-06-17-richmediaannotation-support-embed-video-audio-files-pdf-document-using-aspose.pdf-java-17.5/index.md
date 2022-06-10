---
title: 'Embed Video or Audio Files in PDF Document using Aspose.PDF for Java 17.5'
date: Sat, 17 Jun 2017 21:14:40 +0000
draft: false
url: /2017/06/17/richmediaannotation-support-embed-video-audio-files-pdf-document-using-aspose.pdf-java-17.5/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Add Media Files to PDF in Java', 'Embed audio or video files in PDF', 'Embed media file in PDF in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="">}}


A new release of Aspose.PDF for Java 17.5 supporting the feature to add RichMediaAnnotation inside PDF document is introduced. The RichMediaAnnotation allows the feature to embed media files within the PDF document and sets video/audio player, implemented as a flash application. Furthermore, we also have tested the compatibility of API with Grails, Dockers platform and Oracle Agile Product Lifecycle Management applications and it has proved to work without any issues. It also includes fixes related to previously reported issues, which make this release version stable and robust enough for PDF files creation, manipulation, and transformation to other support formats.

## Adding RichMediaAnnotation

If we have a requirement to add an external video link in PDF document, we can use MovieAnnotaiton object. However, when there is a requirement to embed media inside the PDF document, we need to use RichMediaAnnotation. This annotation allows to embed media file within the PDF document and sets video/audio player, implemented as a flash application. Due to license restrictions, we can not include third-party flash scripts in our product, so you need to provide your script for playing videos or audios. You should provide a flash application code. For example, you can use videoplayer.swf and audioplayer.swf which are distributed with Adobe Acrobat and may be found in Multimedia Skins/Players sub-folder in Acrobat folder. Another option is using StrobeMediaPLayback.swf player or any other video player implemented in flash.  
For further details, please visit [Working with RichMediaAnnotation][1]

```
// instantiate Document instance
Document doc = new Document();
 
// add page to pages collection of Document object
Page page = doc.getPages().add();
  
// create RichMediaAnnotation object
RichMediaAnnotation rma = new RichMediaAnnotation(page, new Rectangle(100,500, 300, 600));
  
//here we should specify stream containing code of the video player
InputStream is = new FileInputStream(myDir+"Videoplayer.swf");
rma.setCustomPlayer(is);
  
// Give name to video data. This data will be embedded into document 
// with this name and referenced from flash variables by this name. 
// videoName should not contain path to the file; this is rather "key" 
// to access data inside of the PDF document
String videoName = "VideoTutorial.mp4";
  
//also we use skin for video player
String skinName = "SkinOverAllNoFullNoCaption.swf";
  
//compose flash variables line for player. please note that different players may 
// have different format of the flash variables line. Refer to documentation for your player.
rma.setCustomFlashVariables(String.format("source=%s&skin=%s", "VideoTutorial.mp4", skinName));
  
//add skin code. 
InputStream is2 = new FileInputStream(myDir+"SkinOverAllNoFullNoCaption.swf");
rma.addCustomData(skinName,is2);
  
//set poster for video
InputStream is3 = new FileInputStream(myDir+"barcode.jpg");
rma.setPoster(is3);
  
 
InputStream fs = new FileInputStream(myDir + videoName);
//set video content
rma.setContent(videoName, fs);
  
//set type of the content (video)
rma.setType(RichMediaAnnotation.ContentType.Video);
  
//active player by click
rma.setActivateOn(RichMediaAnnotation.ActivationEvent.Click);
  
//update annotation data. This method should be called after all assignments/setup. 
// This method initializes data structure of the annotation and embeds required data. 
rma.update();
  
//add annotation on the page.
page.getAnnotations().add(rma);
  
doc.save(myDir + "Output"+version+"2.pdf");
 
try
{
    if (is!=null)
        is.close();
    if (is2!=null)
        is2.close();
    if (is3!=null)
        is3.close();
    if (fs!=null)
        fs.close();
} catch (Exception e)
{
    // TODO: handle exception
} 
```

## Miscellaneous fixes

Apart from the above mentioned improvements, the PDF to HTML conversion is one of the significant improvement which helps to create output files with great fidelity. We also have made improvements in PDF to PDF/A conversion feature, Image to PDF conversion, Annotation creation, and manipulation, Text extraction, Text replacement. As it is always recommended to use the latest release of our API's, so we suggest you to please download the latest release of Aspose.Pdf for Java 17.5 and check Release Notes section regarding the list of issues fixed in [Aspose.PDF for Java 17.5][2]

*   [Home page for Aspose.PDF for Java][3]
*   [Download Aspose.Pdf for Java][4]
*   [Aspose.PDF product family forum][5]– Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   [Aspose.PDF for Java online documentation][6]– help documentation and API reference documents.
*   [Enable Blog Subscription][7]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.Pdf for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://docs.aspose.com/
[2]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+17.5+Release+Notes
[3]: https://products.aspose.com/pdf/java
[4]: https://downloads.aspose.com/pdf/java
[5]: http://forum.aspose.com
[6]: https://docs.aspose.com/display/pdfjava/Home
[7]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[8]: https://github.com/aspose-pdf/Aspose.Pdf-for-Java




