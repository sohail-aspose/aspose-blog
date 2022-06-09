---
title: 'Encrypt and Decrypt Excel Files in Python'
seoTitle: "Encrypt Decrypt Excel Files in Python | Password-Protect Excel Files"
description: "Use Python spreadsheet API to encrypt or decrypt Excel files in Python. Protect Excel XLSX and XLS files with password programmatically."
date: Tue, 01 Jun 2021 12:28:28 +0000
draft: false
url: /2021/06/01/encrypt-and-decrypt-excel-files-in-python/
author: Usman Aziz
summary: 'Security and privacy have always been important aspects of safeguarding data. Since Excel files are widely used to store data, safety is ensured to avoid tampering and unauthorized access. In accordance with that, this article covers **how to encrypt and decrypt Excel files in Python**.'
tags: ['Decrypt Excel Files using Python', 'Encrypt Excel Files using Python', 'Protect Excel Files with Password in Python']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Encrypt-Decrypt-Excel-Files.jpg" alt="Encrypt Decrypt Excel Files Python">}}


Security and privacy have always been important aspects of safeguarding data. Since Excel files are widely used to store data, safety is ensured to avoid tampering and unauthorized access. In accordance with that, this article covers **how to encrypt and decrypt Excel files in Python**.

*   [Python API to Encrypt and Decrypt Excel Files][1]
*   [Encrypt Excel Files using Python][2]
*   [Decrypt Excel Files using Python][3]

## Python API to Encrypt and Decrypt Excel Files {#Python-API-to-Encrypt-and-Decrypt-Excel-Files}

In order to encrypt and decrypt Excel files, we'll use [Aspose.Cells for Python via Java][4]. Apart from the protection of Excel files, the API supports generating, modifying, and converting Excel files dynamically. You can install the API using the following pip command.

*   `pip install aspose-cells`

## Encrypt Excel Files using Python {#Encrypt-Excel-Files-using-Python}

The following are the steps to encrypt Excel files in Python.

*   Load the Excel file using the [Workbook][5] class.
*   Set password using [Workbook.getSettings().setPassword(string)][6] method.
*   Set type of the encryption using [Workbook.setEncryptionOptions(EncryptionType, KeyLength)][7] method.
*   Save the encrypted Excel file using [Workbook.save(string)][8] method.

The following code sample shows how to encrypt Excel files in Python.

{{< gist aspose-com-gists 88e08b1a02d10eb9aa89097ff12e1e3c "encrypt-excel-file.py" >}}

## Decrypt Excel Files using Python {#Decrypt-Excel-Files-using-Python}

The following are the steps to decrypt Excel files in Python.

*   Create an object of [LoadOptions][9] class and initialize it with XLSX format.
*   Provide password using [LoadOptions.setPassword(string)][10] method.
*   Create an object of the [Workbook][11] class and initialize it with an encrypted Excel file's path and _LoadOptions_ object.
*   Decrypt Excel file by setting the password to _None_ using [Workbook.getSettings().setPassword(None)][12].
*   Save the decrypted Excel file using [Workbook.save(string)][13] method.

The following code sample shows how to decrypt an Excel file in Python.

{{< gist aspose-com-gists 88e08b1a02d10eb9aa89097ff12e1e3c "decrypt-excel-file.py" >}}

## Get a Free API License

You can use the API without evaluation limitations by requesting a [free temporary license][14].

## Conclusion

In this article, you have learned how to protect Excel files by applying encryption using Python. Furthermore, you have seen how to decrypt encrypted Excel files in Python. You can explore more about the Python spreadsheet API using the [documentation][15]. In case you would have any questions or queries, feel free to let us know via our [forum][16].

## See Also

*   [Create MS Excel Files using Python][17]
*   [Convert Excel to PDF in Python][18]




[1]: #Python-API-to-Encrypt-and-Decrypt-Excel-Files
[2]: #Encrypt-Excel-Files-using-Python
[3]: #Decrypt-Excel-Files-using-Python
[4]: https://products.aspose.com/cells/python-java
[5]: https://apireference.aspose.com/cells/python/asposecells.api/workbook
[6]: https://apireference.aspose.com/cells/python/asposecells.api/workbooksettings#Password
[7]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#setEncryptionOptions(int,%20int)
[8]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[9]: https://apireference.aspose.com/cells/python/asposecells.api/LoadOptions
[10]: https://apireference.aspose.com/cells/python/asposecells.api/loadoptions#Password
[11]: https://apireference.aspose.com/cells/python/asposecells.api/workbook
[12]: https://apireference.aspose.com/cells/python/asposecells.api/workbooksettings#Password
[13]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/cells/pythonjava/
[16]: https://forum.aspose.com/
[17]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/
[18]: https://blog.aspose.com/2021/04/02/convert-excel-files-to-pdf-in-python/





