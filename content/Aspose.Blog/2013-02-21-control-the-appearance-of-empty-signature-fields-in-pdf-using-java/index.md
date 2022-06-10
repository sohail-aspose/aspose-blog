---
title: 'Control the Appearance of Empty Signature Fields in PDF using Java'
date: Thu, 21 Feb 2013 16:23:07 +0000
draft: false
url: /2013/02/21/control-the-appearance-of-empty-signature-fields-in-pdf-using-java/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Acrobat', 'PDF to Image conversion', 'PdfSignature', 'Sign PDF file', 'Signature appearance', 'Text extraction', 'annotation export', 'java', 'product release', 'text replace']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Control the Appearance of Empty Signature Fields in PDF">}}


We are pleased to announce the release of [Aspose.PDF for Java][1] 4.5.0. In this release version, we have greatly improved the text extraction feature and we have also introduced a method to control the appearance of empty signature fields. In order to fulfill this requirement, new methods are implemented in the FormEditor class. Now you can make form fields hidden by specifying the Form.FLAG\_HIDDEN flag as a parameter of the addField(...) method.

```
FormEditor editor = new FormEditor(INPUT_FILE, tmp_filename);  
editor.addField(FieldType.Signature, "Kunde", 1, 100, 100, 201, 201, Form.FLAG_HIDDEN);  
editor.addField(FieldType.Signature, "gesetzl Vertreter", 100, 100, 201, 201, Form.FLAG_HIDDEN);  
editor.addField(FieldType.Signature, "Berater", 2, new Rectangle(300, 100, 500 - 300, 250 - 100), 
       Form.FLAG_HIDDEN); 
editor.save();
```

You may also use the setFieldFlag method for the same reason. It is fixed for editing new fields before save, but this is not recommended due to performance reasons.

```
FormEditor editor = new FormEditor(INPUT_FILE, tmp_filename);  
editor.setFieldFlag("Berater", Form.FLAG_HIDDEN); 
editor.save();
```

Please visit the following link for further details on what's new & fixed in [Aspose.PDF for Java][2] 4.5.0.




[1]: https://downloads.aspose.com/pdf/java
[2]: https://downloads.aspose.com/pdf/java




