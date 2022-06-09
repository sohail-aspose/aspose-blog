---
title: 'Encrypt and Decrypt Excel Files using Java'
seoTitle: "Encrypt Decrypt Excel Files in Java | Password-Protect Excel Files"
description: "Java Spreadsheet API to encrypt and decrypt Excel files in Java. Encrypt Excel files using SHA and AES encryptions. Password protect Excel files in Java."
date: Tue, 02 Feb 2021 23:19:00 +0000
draft: false
url: /2021/02/02/encrypt-and-decrypt-excel-files-using-java/
author: Usman Aziz
summary: 'MS Excel provides you with a wide range of features to keep and analyze the data seamlessly. You can perform computations, generate charts as well as define your custom logic using VBA modules. Knowing the importance of the data in spreadsheets, MS Excel allows you to protect the workbooks using encryption. Furthermore, you can password protect the Excel files to avoid unauthorized access. In accordance with that, this article covers **how to encrypt/decrypt and password-protect Excel files using Java**.'
tags: ['Decrypt Excel Files using Java', 'Encrypt Excel Files using Java', 'Java API to Encrypt and Decrypt Excel Files', 'Verify Password of Encrypted Excel File']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Protect-Excel-Files-C.jpg" alt="encrypt decrypt excel files in java">}}


MS Excel provides you with a wide range of features to keep and analyze the data seamlessly. You can perform computations, generate charts as well as define your custom logic using VBA modules. Knowing the importance of the data in spreadsheets, MS Excel allows you to protect the workbooks using encryption. Furthermore, you can password protect the Excel files to avoid unauthorized access. In accordance with that, this article covers **how to encrypt/decrypt and password-protect Excel files using Java**.

*   [Java API to Encrypt and Decrypt Excel Files][1]
*   [Encrypt Excel Files using Java][2]
*   [Decrypt Excel Files using Java][3]
*   [Verify Password of Encrypted Excel File][4]
*   [Get Free API License][5]

## Java API to Encrypt and Decrypt Excel Files {#Java-API-to-Encrypt-and-Decrypt-Excel-Files}

[Aspose.Cells for Java][6] is a powerful spreadsheet manipulation API that lets you create and manipulate Excel files seamlessly. Furthermore, it allows you to encrypt and decrypt the workbooks within a few lines of code. In addition, you can protect an Excel file with a password. Aspose.Cells for Java can either be downloaded as [JAR][7] or installed using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-cells</artifactId>
    <version>20.12</version>
</dependency>
```

## Encrypt Excel Files using Java {#Encrypt-Excel-Files-using-Java}

Aspose.Cells for Java provides the following encryption types for Excel 2003 files.

*   [XOR][8]
*   [COMPATIBLE][9] (Office 97/2000 compatible)
*   [ENHANCED CRYPTOGRAPHIC PROVIDER V1][10]
*   [STRONG CRYPTOGRAPHIC PROVIDER][11]

However, 2007/2010 workbooks are encrypted using SHA and AES encryption techniques in the same way MS Excel does. The following are the steps to encrypt an Excel file using Aspose.Cells for Java.

*   Load the Excel file using [Workbook][12] class.
*   Set password using [Workbook.getSettings().setPassword(string)][13] method.
*   Encrypt Excel file using [Workbook.setEncryptionOptions(EncryptionType, int)][14] method.
*   Save the encrypted workbook using [Workbook.save(string)][15] method.

For demonstration, the following code sample shows how to encrypt an Excel file using Java.

{{< gist aspose-com-gists 5bccba043cd3a3f2f27b92453a3e37d5 "encrypt-excel-file.java" >}}

## Decrypt Excel Files using Java {#Decrypt-Excel-Files-using-Java}

In order to decrypt an encrypted Excel file, you only need to provide its password and the rest will be handled by Aspose.Cells for Java. The following are the steps to decrypt an Excel file using Java.

*   Create an instance of [LoadOptions][16] class.
*   Specify the password using [LoadOptions.setPassword(string)][17] method.
*   Create an instance of the [Workbook][18] class and pass the file's path and [LoadOptions][19] object to its constructor.
*   Set password to _null_ using [Workbook.getSettings().setPassword(string)][20] method.
*   Once done, save the decrypted workbook using [Workbook.save(string)][21] method.

The following code sample shows how to decrypt a password-protected Excel file using Java.

{{< gist aspose-com-gists 5bccba043cd3a3f2f27b92453a3e37d5 "decrypt-excel-file.java" >}}

## Verify Password of an Encrypted Excel File {#Verify-Password-of-Encrypted-Excel-File}

In addition to encryption/decryption, Aspose.Cells for Java also allows you to verify the password of a protected Excel file. The following are the steps to perform password verification.

*   Load the encrypted Excel file using [FileInputStream][22] class.
*   Use [FileFormatUtil.verifyPassword(FileInputStream, string)][23] method to verify the password.
*   As a result, if the return value is true then the password is valid else it is invalid.

The following code sample shows how to verify the password of an encrypted Excel file using Java.

{{< gist aspose-com-gists 5bccba043cd3a3f2f27b92453a3e37d5 "verify-password.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

In case you want to try the API without evaluation limitations, you can [get a free temporary license][24].

## Conclusion

In this article, you have learned how to encrypt or decrypt Excel files using Java. Furthermore, you have seen how to verify the password of an encrypted Excel file. In case you want to explore more about the Java spreadsheet manipulation API, visit the [documentation][25].

## See Also

*   [](https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/)[Create MS Excel Files using Java without MS Office][26]




[1]: #Java-API-to-Encrypt-and-Decrypt-Excel-Files
[2]: #Encrypt-Excel-Files-using-Java
[3]: #Decrypt-Excel-Files-using-Java
[4]: #Verify-Password-of-Encrypted-Excel-File
[5]: #Get-a-Free-API-License
[6]: https://products.aspose.com/cells/java
[7]: https://downloads.aspose.com/cells/java
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/encryptiontype#XOR
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/encryptiontype#COMPATIBLE
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/encryptiontype#ENHANCED_CRYPTOGRAPHIC_PROVIDER_V_1
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/encryptiontype#STRONG_CRYPTOGRAPHIC_PROVIDER
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbooksettings#Password
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#setEncryptionOptions(int,%20int)
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/LoadOptions
[17]: https://apireference.aspose.com/cells/java/com.aspose.cells/loadoptions#Password
[18]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[19]: https://apireference.aspose.com/cells/java/com.aspose.cells/LoadOptions
[20]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbooksettings#Password
[21]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[22]: https://docs.oracle.com/javase/7/docs/api/java/io/FileInputStream.html
[23]: https://apireference.aspose.com/cells/java/com.aspose.cells/fileformatutil#verifyPassword(java.io.InputStream,%20java.lang.String)
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/cells/java/getting-started/
[26]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/





