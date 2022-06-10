---
title: 'Java QR Code Generator by Aspose.BarCode for Java'
date: Wed, 04 Mar 2015 05:24:21 +0000
draft: false
url: /2015/03/04/qr-code-generator-by-aspose.barcode-for-java/
author: Farooq Sheikh
summary: ''
tags: ['Aspose.BarCode', 'Generate QR Code in Java', 'Generate QR Code in Java Spring MVC', 'QR Code Generator in Java', 'qr code generator']
categories: ['Aspose.BarCode Product Family']
---

QR Code Generator by Aspose.BarCode for Java is a web application to generate various types of QR Codes using [Aspose.BarCode for Java][1].

[Aspose.BarCode for Java][2] is a robust and reliable barcode generation and recognition component, written in Java. It allows developers to quickly and easily add barcode generation and recognition functionality to their Java applications. It is available for the Java SE, Java EE and Java ME platforms.

This application highlights commonly used features of [Aspose.BarCode for Java][3] and demonstrates how to utilize them to generate various types of QR Codes including Text, Url, Email, Phone number, Contact (VCard), Event, Geolocation, Wifi and SMS.



{{< figure align=center src="images/aspose-showcase-qrcodegen.png" alt="Java QR Code Generator">}}


## QR Code Generator - Highlights {#highlights}

*   Spring MVC 4.0 RESTFul API based web application for QR Code generation using [Aspose.BarCode for Java][4] library
*   Mobile friendly [responsive and flat UI][5] using Bootstrap 3+ , RequireJS, Backbone.js on top of restful APIs
*   Generate various types of (scan-able) QR Codes using [Aspose.BarCode for Java][6]
    *   URL
    *   Text
    *   Vcard
    *   SMS
    *   Phone
    *   Event
    *   Wifi
    *   Geolocation
    *   Encrypted Text
*   Supports various QR Code customizations including
    *   Resizing
    *   Selection of Level of Reed-Solomon error correction. From low to high: LevelL, LevelM, LevelQ, LevelH
    *   Foreground and Background color selection
*   Save the generated QR Code in different image formats (Bmp, Gif, Jpeg, Png, Tiff)
*   Generate encrypted QR Code from Plain Text using password-based encryption (PBE)- PBEWITHMD5AND128BITAES-CBC-OPENSSL with OpenSSL compatibility

### Steps To Generate QR Code {#steps-to-generate-qr-code}

1.  Select the QR Code Type
2.  Input Type Context
3.  Customize QR Code Settings
4.  Generate/Preview QR Code
5.  Save QR Code



{{< figure align=center src="images/aspose-showcase-qrcodegen-generation-steps.png" alt="Generate QR Code in Java">}}


## Export/Save Generated QR Code {#export-save-generated-qr-code}

You can export the generated QR Code into any of the following formats.

*   PNG
*   JPEG
*   GIF
*   TIFF
*   BMP

## Embed Anywhere {#embed-anywhere}

The application also supports embedding generated QR Codes into any website of your choice using a direct URL. Here are the steps.

### **Steps To Generate Embed QR Code** {#steps-to-generate-qr-code}

1.  Select the QR Code Type
2.  Input Type Context
3.  Customize QR Code Settings
4.  Generate/Preview QR Code
5.  Copy QR Code Save URL
6.  Change URL query string ‘download’ to false.
7.  That’s it. URL is now ready to embed as an image.

```
<img width="100%" src="http://localhost:8080/qrcodegen/api/qrcode/generate?data=http://aspose.com&ecc=L&foreColor=%23000000&bgColor=%23FFFFFF&download=false&format=png">

```

## API Documentation {#api-documentation}

The application also exports its Restful APIs documentation using [swagger specification][7]. You can also view the application APIs swagger based documentation by accessing the following URL after running the project.

_http://localhost:8080/qrcodegen/public/docs/_



{{< figure align=center src="images/aspose-showcase-qrcodegen-swagger-api-docs.png" alt="Create QR in Java">}}


## Clone Repository {#to-get-the-code}```
$ git clone https://github.com/AsposeShowcase/QR\_Code\_Generator\_by\_Aspose.BarCode\_for\_Java.git

```

If this is your first time using Github, review [http://help.github.com][8] to learn the basics.

## Run QR Code Generator {#to-run-the-application-}

**From the command line with Maven:**

```
$ cd QR\_Code\_Generator\_by\_Aspose.BarCode\_for\_Java
$ mvn jetty:run

```

**From IDE such as NetBeans IDE, Eclipse, IDEA or others:**

*   [Download][9] or [clone][10] the project Github repository
*   Import [QR\_Code\_Generator\_by\_Aspose.BarCode\_for\_Java][11] as a Maven Project
*   Server to run, such as [Glassfish][12]/[Tomcat][13]

_Note: Set the application context path to ‘qrcodegen’ (if required)._

##### Access the deployed application at: _http://localhost:8080/qrcodegen/_ {#access-the-deployed-application-at-http-localhost-8080-qrcodegen-}

Aspose License

The project works without a license, with limitations. To remove limitations, you can acquire a free [temporary license][14] or [buy a full license][15].

## How to Apply License {#to-apply-aspose-lincese}

Simply change _license.file_ property value to the path to your Aspose license file in the project configuration `src/main/resources/config.properties`.

```
license.file=C:\\\\aspose\\\\Aspose.Total.Java.lic

```

## Technologies {#technologies}

The project uses a number of open-source projects to work properly:

*   [Spring Framework][16]
*   [swagger-springmvc][17]
*   [Swagger UI][18]
*   [Twitter Bootstrap][19]
*   [RequireJS][20]
*   [Backbone.js][21]
*   [jQuery][22]

## Download the Source Code

Complete source code of **QR Code Generator by Aspose.BarCode for Java** is available on your favorite site.

*   [QR Code Generator by Aspose.BarCode for Java on **Github**][23]
*   [QR Code Generator by Aspose.BarCode for Java on **Codeplex**][24]
*   [QR Code Generator by Aspose.BarCode for Java on **Google Code**][25]




[1]: https://products.aspose.com/barcode/java
[2]: https://products.aspose.com/barcode/java
[3]: https://products.aspose.com/barcode/java
[4]: https://products.aspose.com/barcode/java
[5]: http://asposeshowcase.github.io/QR_Code_Generator_by_Aspose.BarCode_for_Java/images/docs/aspose-showcase-qrcodegen-ios_iPhone-6_8.0_portrait.jpg
[6]: https://products.aspose.com/barcode/java
[7]: https://github.com/OAI/OpenAPI-Specification
[8]: http://help.github.com
[9]: https://github.com/AsposeShowcase/QR_Code_Generator_by_Aspose.BarCode_for_Java/archive/master.zip
[10]: //github.com/AsposeShowcase/QR_Code_Generator_by_Aspose.BarCode_for_Java
[11]: https://github.com/AsposeShowcase/QR_Code_Generator_by_Aspose.BarCode_for_Java/
[12]: https://javaee.github.io/glassfish/
[13]: http://tomcat.apache.org/
[14]: https://purchase.aspose.com/temporary-license
[15]: https://purchase.aspose.com/
[16]: https://spring.io/projects/spring-framework
[17]: https://github.com/springfox/springfox
[18]: https://github.com/swagger-api/swagger-ui
[19]: https://getbootstrap.com/2.3.2/
[20]: http://requirejs.org/
[21]: http://backbonejs.org/
[22]: http://jquery.com
[23]: https://github.com/AsposeShowcase/QR_Code_Generator_by_Aspose.BarCode_for_Java/
[24]: https://en.wikipedia.org/wiki/CodePlex
[25]: https://code.google.com/archive/p/qr-code-generator-by-aspose-barcode-for-java




