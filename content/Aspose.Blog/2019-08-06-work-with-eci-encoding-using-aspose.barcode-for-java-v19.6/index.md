---
title: 'Use ECI Encoding for Barcodes in Java with Aspose.BarCode for Java v19.6'
date: Tue, 06 Aug 2019 00:26:27 +0000
draft: false
url: /2019/08/06/work-with-eci-encoding-using-aspose.barcode-for-java-v19.6/
author: Ahsaniqbal
summary: ''
tags: ['ECI encoding for barcodes using Java']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-Java_100.png" alt="">}}


[Aspose.BarCode for Java 19.6][1] is released which contains new properties and improvements which will ease your work to read and write barcodes with ECI encoding information and also make possible to read low-resolution TIFF images. These API changes and other details can be obtained in the [release note][2] page of the API documentation. Let me share the details of these new features and their use in the programming.

## ECI Encoding for Barcodes

Implementing barcode reading is quite a complex task. Barcode readers need a lot of configurations and information while reading a barcode e.g. the used references for encoding the data in the symbol. This information is embedded in the barcode by adding Extended Channel Interpretation (ECI) setting in the barcode. This mechanism allows usually unsupported national character sets such as Arabic, Greek, or Japanese to be used in barcode symbols. When a symbol is scanned, this information is not intended to be the part of the barcode data, that is why it is kept transparent while scanning a symbol. It is just a switch or tick-box that is checked by the reader followed by a symbology-dependent ECI selection. In Basic Channel Mode, the ECI control information is not transmitted from the reader to the host system. In Extended Channel Mode, both the ECI control information and the data are transmitted to the host system.

Aspose.Barcode has implemented this feature by providing a property QrParameters.setQrECIEncoding() and getQrECIEncoding() in the barcode generator class. For example, if you want to set the encoding mode to ECI and encoding scheme to UTF 8 you should use the following statements while creating a barcode.

{{< gist aspose-com-gists 9dea2dd38be50330a824dd05da062a97 "Examples-src-main-java-com-aspose-barcode-examples-TwoD_barcodes-basic_features-CreatingAQRBarcode-EncodeQRCodEInECIMode.java" >}}

The following are the ECI encodings that are provided while using this feature.

1.  **ISO\_8859\_1** - ISO/IEC 8859-1 Latin alphabet No. 1 encoding. ECI Id:"\\000003".
2.  **ISO\_8859\_2** - ISO/IEC 8859-2 Latin alphabet No. 2 encoding. ECI Id:"\\000004".
3.  **ISO\_8859\_3** - ISO/IEC 8859-3 Latin alphabet No. 3 encoding. ECI Id:"\\000005".
4.  **ISO\_8859\_4** - ISO/IEC 8859-4 Latin alphabet No. 4 encoding. ECI Id:"\\000006".
5.  **ISO\_8859\_5** - ISO/IEC 8859-5 Latin/Cyrillic alphabet encoding. ECI Id:"\\000007".
6.  **ISO\_8859\_6** - ISO/IEC 8859-6 Latin/Arabic alphabet encoding. ECI Id:"\\000008".
7.  **ISO\_8859\_7** - ISO/IEC 8859-7 Latin/Greek alphabet encoding. ECI Id:"\\000009".
8.  **ISO\_8859\_8** - ISO/IEC 8859-8 Latin/Hebrew alphabet encoding. ECI Id:"\\000010".
9.  **ISO\_8859\_9** - ISO/IEC 8859-9 Latin alphabet No. 5 encoding. ECI Id:"\\000011".
10.  **ISO\_8859\_10** - ISO/IEC 8859-10 Latin alphabet No. 6 encoding. ECI Id:"\\000012".
11.  **ISO\_8859\_11** - ISO/IEC 8859-11 Latin/Thai alphabet encoding. ECI Id:"\\000013".
12.  **ISO\_8859\_13** - ISO/IEC 8859-13 Latin alphabet No. 7 (Baltic Rim) encoding. ECI Id:"\\000015".
13.  **ISO\_8859\_14** - ISO/IEC 8859-14 Latin alphabet No. 8 (Celtic) encoding. ECI Id:"\\000016".
14.  **ISO\_8859\_15** - ISO/IEC 8859-15 Latin alphabet No. 9 encoding. ECI Id:"\\000017".
15.  **ISO\_8859\_16** - ISO/IEC 8859-16 Latin alphabet No. 10 encoding. ECI Id:"\\000018".
16.  **Shift\_JIS** - Shift JIS (JIS X 0208 Annex 1 + JIS X 0201) encoding. ECI Id:"\\000020".
17.  **Win1250** - Windows 1250 Latin 2 (Central Europe) encoding. ECI Id:"\\000021".
18.  **Win1251** - Windows 1251 Cyrillic encoding. ECI Id:"\\000022".
19.  **Win1252** - Windows 1252 Latin 1 encoding. ECI Id:"\\000023".
20.  **Win1256** - Windows 1256 Arabic encoding. ECI Id:"\\000024".
21.  **UTF16BE** - ISO/IEC 10646 UCS-2 (High order byte first) encoding. ECI Id:"\\000025".
22.  **UTF8** - ISO/IEC 10646 UTF-8 encoding. ECI Id:"\\000026".
23.  **US\_ASCII** - ISO/IEC 646:1991 International Reference Version of ISO 7-bit coded character set encoding. ECI Id:"\\000027".
24.  **Big5** - Big 5 (Taiwan) Chinese Character Set encoding. ECI Id:"\\000028".
25.  **GB18030** - GB (PRC) Chinese Character Set encoding. ECI Id:"\\000029".
26.  **EUC\_KR** - Korean Character Set encoding. ECI Id:"\\000030".

For more information visit the following article:

*   [QR code encoding in the ECI mode][3]

## Barcode Recognition on Low-Resolution TIFF

Some times there are images that are quite low in resolution and cannot be detected like one of the reasons can be fully wiped bars in the barcode. This issue can make them too difficult rather impossible to be read by any barcode reading software. We have put a special effort for this and added a new property to overcome this issue. New public property AllowOneDWipedBarsRestoration has been added to the QualitySettings. It allows the engine for 1D barcodes to recognize barcodes with single wiped/glued bars in pattern. Property is enabled by default in HighQuality, MaxBarCodes modes.

Currently the property is used for Code128, GS1Code128, SCC14, EAN14, SSCC18, AustralianPosteParcel, SwissPostParcel barcode types. You can use this feature by calling the following line of code before reading information from a BarCodeReader object to signal it to read low-resolution TIFF images.

{{< gist aspose-com-gists 9dea2dd38be50330a824dd05da062a97 "Examples-src-main-java-com-aspose-barcode-examples-barcode_recognition-advanced_features-SingleWipedBarsInPattern-SingleWipedBarsInPattern.java" >}}




[1]: https://downloads.aspose.com/barcode/java/new-releases/aspose.barcode-for-java-19.6/
[2]: https://docs.aspose.com/display/barcodejava/Aspose.BarCode+for+Java+19.6+Release+Notes
[3]: https://docs.aspose.com/display/barcodejava/Creating+a+QR+Barcode#CreatingaQRBarcode-QRCodeEncodingintheECIMode




