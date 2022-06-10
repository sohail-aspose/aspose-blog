---
title: 'Improved Text Extraction Mechanism for PDF using Aspose.Pdf.Kit for .NET 4.2.0'
date: Wed, 10 Mar 2010 20:46:00 +0000
draft: false
url: /2010/03/10/improved-text-extraction-mechanism-for-pdf-using-csharp/
author: Shahzad Latif
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

In [Aspose.Pdf.Kit for .NET][1] versions before 4.2.0, ExtractText method placed an additional byte sequence into the memory stream to indicate that the bytes are Unicode encoded. As StreamReader class has auto-detect behavior, so ReadToEnd method produced correct string. However that behavior was not very convenient.

Aspose.Pdf.Kit for .NET 4.2.0 uses a new approach for text extraction. The additional byte sequence has been removed and the StreamReader can't automatically detect the text encoding, rather the user will have to provide the encoding type explicitly.

Parameterless ExtractText method extracts the text using 16-bit Unicode encoding, whereas the StreamReader object creates a UTF-8 encoded stream. Now, there are two ways that you can get proper text: either extract text using UTF-8 encoding and create a StreamReader object with the default encoding type or use parameterless ExtractText method and then specify Unicode encoding while creating a StreamReader object.

You can find the examples for both of these methods below:

**Method 1:**   

```
 PdfExtractor pdfExtractor = new PdfExtractor();
                pdfExtractor.BindPdf(“input.pdf”);

                //specify UTF-8 encoding
                pdfExtractor.ExtractText(Encoding.UTF8);

                MemoryStream tempMemoryStream = new MemoryStream();
               pdfExtractor.GetText(tempMemoryStream);

                string text = “”;
                //create StreamReader object with default encoding
                using (StreamReader sr = new StreamReader(tempMemoryStream))
                {
                      sr.BaseStream.Seek(0, SeekOrigin.Begin);
                        text = sr.ReadToEnd();
                  }
```

**Method 2:**

```
PdfExtractor pdfExtractor = new PdfExtractor();
                pdfExtractor.BindPdf(“input.pdf”);

                //use parameterless ExtractText method
                pdfExtractor.ExtractText();

                MemoryStream tempMemoryStream = new MemoryStream();
                pdfExtractor.GetText(tempMemoryStream);

                string text = “”;
                //specify Unicode encoding type in StreamReader constructor
                using (StreamReader sr = new StreamReader(tempMemoryStream, Encoding.Unicode))
                {

                      sr.BaseStream.Seek(0, SeekOrigin.Begin);
                      text = sr.ReadToEnd();
                  }
```




[1]: https://products.aspose.com/pdf/net




