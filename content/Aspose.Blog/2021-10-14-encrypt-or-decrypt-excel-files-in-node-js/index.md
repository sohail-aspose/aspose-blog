---
title: 'Encrypt or Decrypt Excel Files in Node.js'
seoTitle: "Encrypt Decrypt Excel Files in Node.js | Password-Protect Excel Files"
description: "Use Node.js Spreadsheet API to encrypt and decrypt Excel files from within Node.js applications. Encrypt XLSX/XLS files using SHA and AES encryptions."
date: Thu, 14 Oct 2021 15:44:00 +0000
draft: false
url: /2021/10/14/encrypt-or-decrypt-excel-files-in-node-js/
author: Usman Aziz
summary: 'MS Excel is a powerful tool that allows you to perform various spreadsheet manipulation operations. You can organize data, apply computations, generate charts, define your custom logic using VBA modules, and so on. An important feature that MS Excel provides is encryption and decryption of the Excel files. In accordance with that, this article covers **how to encrypt/decrypt and password-protect Excel files in Node.js applications**.'
tags: ['Decrypt Excel Files in Node-js', 'Encrypt Excel Files in Node-js', 'password-protect-excel-files-node-js']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Encrypt-Decrypt-Excel-Files.jpg" alt="Encrypt Decrypt Excel Files Node.js">}}


MS Excel is a powerful tool that allows you to perform various spreadsheet manipulation operations. You can organize data, apply computations, generate charts, define your custom logic using VBA modules, and so on. An important feature that MS Excel provides is encryption and decryption of the Excel files. In accordance with that, this article covers **how to encrypt/decrypt and password-protect Excel files in Node.js applications**.

*   [Node.js API to Encrypt and Decrypt Excel Files][1]
*   [Encrypt Excel Files in Node.js][2]
*   [Decrypt Excel Files in Node.js][3]
*   [Get Free API License][4]

## Node.js API to Encrypt and Decrypt Excel Files {#API-to-Encrypt-and-Decrypt-Excel-Files}

For encryption and decryption of Excel files, we will use [Aspose.Cells for Node.js via Java][5]. It is a feature-rich API that allows you to encrypt and decrypt the workbooks within a few lines of code. In addition, you can password-protect an Excel file seamlessly. You can either [download][6] the API or install it using the following npm command.

`> npm install aspose.cells`

## Encrypt Excel XLSX or XLS Files in Node.js {#Encrypt-Excel-Files}

Aspose.Cells for Node.js via Java provides the following encryption types for Excel 2003 files.

*   XOR
*   COMPATIBLE (Office 97/2000 compatible)
*   ENHANCED CRYPTOGRAPHIC PROVIDER V1
*   STRONG CRYPTOGRAPHIC PROVIDER

Whereas, SHA and AES encryption techniques are used for 2007/2010 workbooks. The following are the steps to encrypt an Excel file in Node.js.

*   Load the Excel file using [Workbook][7] class.
*   Set password using [Workbook.getSettings().setPassword(string)][8] method.
*   Encrypt Excel file using [Workbook.setEncryptionOptions(EncryptionType, int)][9] method.
*   Save the encrypted workbook using [Workbook.save(string)][10] method.

The following code sample shows how to encrypt an Excel XLSX file in Node.js.

{{< gist aspose-com-gists 51e7785a67fa69c534d76021f2b70a1a "encrypt-excel-file.js" >}}

## Decrypt an Excel File in Node.js {#Decrypt-Excel-Files}

To decrypt an encrypted Excel file, you will need to specify its password. The following are the steps to decrypt an Excel file in Node.js.

*   Create an instance of [LoadOptions][11] class.
*   Specify the password using [LoadOptions.setPassword(string)][12] method.
*   Create an instance of the [Workbook][13] class and pass the file's path and _LoadOptions_ object to its constructor.
*   Set password to _null_ using [Workbook.getSettings().setPassword(string)][14] method.
*   Once done, save the decrypted workbook using [Workbook.save(string)][15] method.

The following code sample shows how to decrypt a password-protected Excel file in Node.js.

{{< gist aspose-com-gists 51e7785a67fa69c534d76021f2b70a1a "decrypt-excel-file.js" >}}

## Get a Free API License {#Get-a-Free-API-License}

In case you want to try the API without evaluation limitations, you can [get a free temporary license][16].

## Conclusion

In this article, you have learned how to encrypt or decrypt Excel files in Node.js applications. You can simply integrate the provided code into your Node.js applications to encrypt/decrypt XLSX/XLS files. In case you want to explore more about the Node.js spreadsheet manipulation API, visit the [documentation][17]. Also, you can ask your questions via our [forum][18].

## See Also

*   [Create Excel XLSX/XLS File in Node.js Applications – A Complete Guide][19]
*   [Convert Excel Files to PDF in Node.js][20]
*   [Convert CSV to Excel or Excel to CSV in Node.js][21]




[1]: #API-to-Encrypt-and-Decrypt-Excel-Files
[2]: #Encrypt-Excel-Files
[3]: #Decrypt-Excel-Files
[4]: #Get-a-Free-API-License
[5]: https://products.aspose.com/cells/nodejs-java/
[6]: https://downloads.aspose.com/cells/nodejs
[7]: https://apireference.aspose.com/cells/nodejs/Workbook
[8]: https://apireference.aspose.com/cells/nodejs/WorkbookSettings#setPassword
[9]: https://apireference.aspose.com/cells/nodejs/Workbook#setEncryptionOptions
[10]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[11]: https://apireference.aspose.com/cells/nodejs/LoadOptions
[12]: https://apireference.aspose.com/cells/nodejs/LoadOptions#setPassword
[13]: https://apireference.aspose.com/cells/nodejs/Workbook
[14]: https://apireference.aspose.com/cells/nodejs/WorkbookSettings#setPassword
[15]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/cells/nodejsjava/
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2020/08/05/create-excel-files-in-node.js/
[20]: https://blog.aspose.com/2021/03/05/convert-excel-xlsx-xls-to-pdf-in-node-js/
[21]: https://blog.aspose.com/2021/04/28/convert-csv-to-excel-or-excel-to-csv-in-nodejs/




