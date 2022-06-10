---
title: 'Stable PDF to Image Conversion in Java with Aspose.PDF for Java 4.4'
date: Wed, 10 Oct 2012 08:19:34 +0000
draft: false
url: /2012/10/10/set-signature-appearance-better-pdf-printing-and-stable-pdf-to-image-conversion/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Acrobat', 'PDF to Image conversion', 'PdfSignature', 'Sign PDF file', 'Signature appearance', 'annotation export', 'java', 'product release', 'text replace']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-java.jpg" alt="">}}


We are pleased to announce the release of [Aspose.PDF for Java 4.4.0][1]. In this release, we've improved PDF to image conversion and PDF printing. There are also a couple of new features.

We've introduced a new method for setting the image for a signature appearance from an input stream has been implemented in the PdfFileSignature class.

```
PdfFileSignature pdfSign = new PdfFileSignature(firstFilename, secondFilename); 
pdfSign.setSignatureAppearanceStream(new FileInputStream("filename")); 
pdfSign.sign("Signature", "Reason", "Contact", "Location", signature); 
pdfSign.save();
```

We have also implemented a new method to control the appearance of signature properties.

```
PdfFileSignature pdfSign = new PdfFileSignature(firstFilename, secondFilename); 
pdfSign.setSignatureAppearanceStream(new FileInputStream(SIGN_IMG_FILENAME)); 
pdfSign.sign("Signature", "Reason", "Contact", "Location", sugnature); 
pdfSign.setShowProperties(false); 
pdfSign.save();
```

Please visit the following link for further details on what's new & fixed in [Aspose.PDF for Java 4.4.0][2].




[1]: https://downloads.aspose.com/pdf/java
[2]: https://downloads.aspose.com/pdf/java




