---
title: 'Encrypt and Decrypt Excel Files using C#'
seoTitle: "Encrypt or Decrypt Excel Files in C# | .NET Excel API"
description: "Use .NET Excel API to encrypt and decrypt Excel files using C# or VB.NET. Encrypt and password-protect Excel files from within .NET applications."
date: Thu, 14 Jan 2021 13:10:17 +0000
draft: false
url: /2021/01/14/encrypt-and-decrypt-excel-files-using-csharp/
author: Usman Aziz
summary: 'MS Excel provides an encryption mechanism to protect the data in the spreadsheets from unauthorized users. Along with applying encryption, you can specify the password that is required to open the Excel files. This article covers how to perform the encryption of Excel files from within .NET applications. Particularly, you will learn **how to encrypt and decrypt the Excel files using C#**.'
tags: ['Csharp-API-to-Encrypt-or-Decrypt-Excel-Files', 'Decrypt-Excel-Files-using-Csharp', 'Encrypt-Excel-Files-using-Csharp', 'Verify-Password-of-Encrypted-Excel-File']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Encrypt-Decrypt-Excel-Files.jpg" alt="Encrypt Decrypt Excel Files">}}


MS Excel provides an encryption mechanism to protect the data in the spreadsheets from unauthorized users. Along with applying encryption, you can specify the password that is required to open the Excel files. This article covers how to perform the encryption of Excel files from within .NET applications. Particularly, you will learn **how to encrypt and decrypt the Excel files using C#**.

*   [C# API to Encrypt or Decrypt Excel Files][1]
*   [Encrypt Excel Files using C#][2]
*   [Decrypt Excel Files using C#][3]
*   [Verify Password of Encrypted Excel File][4]
*   [Get Free License][5]

## C# API to Encrypt or Decrypt Excel Files {#CSharp-API-to-Encrypt-or-Decrypt-Excel-Files}

In order to perform encryption and decryption operations on Excel files, this article uses [Aspose.Cells for .NET][6] API. The API provides simple ways of encrypting and password protecting Excel files with the desired encryption type. You can either [download][7] the API or install it within your .NET applications using [NuGet][8].

```
Install-Package Aspose.Cells
```

## Encrypt Excel Files using C# {#Encrypt-Excel-Files-using-CSharp}

Aspose.Cells for .NET supports SHA and AES encryption types in order to encrypt Excel files in the same way as MS Excel does. For Excel 2003 files, you can choose between the following encryption types:

*   XOR
*   Compatible (Office 97/2000 compatible)
*   Enhanced Cryptographic Provider V1
*   Strong Cryptographic Provider

The following are the steps to encrypt an Excel file using C#.

*   Load the Excel file using [Workbook][9] class.
*   Use [Workbook.SetEncryptionOptions(EncryptionType, int)][10] method to apply the desired encryption.
*   Set password using [Workbook.Settings.Password][11] property.
*   Save the workbook using [Workbook.Save(string)][12] method.

The following code sample shows how to encrypt Excel file using C#.

{{< gist aspose-com-gists f90033ab91c802a44d474aa181e4f5b4 "encrypt-excel-file.cs" >}}

## Decrypt Excel Files using C# {#Decrypt-Excel-Files-using-CSharp}

The following are the steps to decrypt Excel files using Aspsoe.Cells for .NET API.

*   Load the Excel file by providing the path and password to the constructor of [Workbook][13] class.
*   Set password to null using [Workbook.Settings.Password][14] property.
*   Save the workbook using [Workbook.Save(string)][15] method.

The following code sample shows how to decrypt an Excel file using C#.

{{< gist aspose-com-gists f90033ab91c802a44d474aa181e4f5b4 "decrypt-excel-file.cs" >}}

## Verify Password of Encrypted Excel File using C# {#Verify-the-Password-of-the-Encrypted-Excel-File}

Aspose.Cells for .NET also allows you to verify the password of the encrypted Excel files. For this, you can follow the below steps.

*   Load the Excel file using [FileStream][16] class.
*   To verify the password, use [FileFormatUtil.VerifyPassword(FileStream, string)][17] method that returns a bool value.
*   If the returned value is true then the password is valid else it is invalid.

The following code sample shows how to verify password of an encrypted Excel file using C#.

{{< gist aspose-com-gists f90033ab91c802a44d474aa181e4f5b4 "verify-password.cs" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][18] in order to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to encrypt and decrypt Excel files using C# from within .NET applications. Furthermore, you have seen how to verify the password of the encrypted Excel files. You can explore more about the C# Excel automation API using [documentation][19].

## See Also

*   [Protect and Unprotect Excel Files using C#][20]




[1]: #CSharp-API-to-Encrypt-or-Decrypt-Excel-Files
[2]: #Encrypt-Excel-Files-using-CSharp
[3]: #Decrypt-Excel-Files-using-CSharp
[4]: #Verify-the-Password-of-the-Encrypted-Excel-File
[5]: #Get-Free-License
[6]: https://products.aspose.com/cells/net
[7]: https://downloads.aspose.com/cells/net
[8]: https://nuget.org/packages/Aspose.Cells
[9]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[10]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/methods/setencryptionoptions
[11]: https://apireference.aspose.com/cells/net/aspose.cells/workbooksettings/properties/password
[12]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[13]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[14]: https://apireference.aspose.com/cells/net/aspose.cells/workbooksettings/properties/password
[15]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[16]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream?view=net-5.0
[17]: https://apireference.aspose.com/cells/net/aspose.cells/fileformatutil/methods/verifypassword
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/cells/net/getting-started/
[20]: https://blog.aspose.com/2020/12/14/protect-or-unprotect-excel-files-using-csharp/





