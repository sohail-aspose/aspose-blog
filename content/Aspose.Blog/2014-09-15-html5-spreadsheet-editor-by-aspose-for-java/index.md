---
title: 'HTML5 Spreadsheet Editor by Aspose for Java'
date: Mon, 15 Sep 2014 15:32:12 +0000
draft: false
url: /2014/09/15/html5-spreadsheet-editor-by-aspose-for-java/
author: Saqib Masood
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

I have shared some sample projects that worked as tutorial or demonstration for Aspose products. This time, I tried something a little bigger – HTML5 Spreadsheet Editor. Yes, I am sharing a web application that loads a Microsoft Excel file, and lets you view and edit it in a web browser. The initial version is limited in its functionality. I'll release newer versions from time to time to make a complete replacement of desktop software. The best part is – it is open source. Let’s take a look at the editor.

## The Technology

I had defined some constraints for this project, which influenced the technology I chose for the development. The application must not be dependent on plugins and must not require end-users to install extra software. So I had to stick to HTML and Ajax. Because it's one of my favourite languages, I used Java server-side. The next important requirement was server-to-browser end-to-end data interoperability. I didn't want to introduce a new integration layer between JavaScript on the browser-side and Java-based business-logic on the server.

There are some good frameworks out there like [Google Web Toolkit (GWT)][1], [Spring Framework][2], [JavaServer Faces (JSF)][3] and some others.

JSF is a component-based web application framework. It is a part of Java standards. A wide range of third-party components are available for JSF. These components can be plugged into any JSF application. The JSF managed beans technology is yet another technology to split your whole project design into independent self-contained components. Objects are created, serialized, de-serialized, injected, managed and destroyed by the application server.

[](http://www.aspose.com/java/excel-component.aspx)[![Aspose.Cells for Java logo][4]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png)Aspose.Cells for Java is the most comprehensive library to create and manipulate Excel files. I used this library to perform all operations; ranging from fetching worksheets, rows, columns, cells to updating the cells.

## The Editor

HTML5 Spreadsheet Editor is an in-browser viewer and editor for Excel files. It supports XLS, XLSX, XLSM, XLSB, XLTX, SpreadsheetML, CSV, ODS. The file can be opened by specifying it in URL.

[![][5]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/09/2.png)

### Opening a Workbook

To open an Excel workbook, specify it in the URL. For example http://spreadsheet-editor.aspose.com/?url=http://example.com/Sample.xlsx. The editor loads the file and displays it as shown above.

[![][6]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/09/1.png)

### Viewing a Workbook

The contents of workbook are displayed in rows and columns style, as we see in the Microsoft Excel desktop application. The editor supports text formatting too.

### Working with Sheets

At the top right-hand corner of HTML5 Spreadsheet Editor is a drop-down list of sheets. The selected sheet is the one which opened by the editor. To switch to another sheet, select it from the list.

[![][7]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/09/463.png)

### Editing Cells

You can edit any cell by a double-click. When you double-click a cell, it switches to edit-mode. To cancel editing, press the ESC key. To commit the edit value, press ENTER. You can also press TAB to move to the next cell. You can specify static text and numbers. Formulas are supported too. To enter a formula, start the cell value with an equal sign (=). For example =SUM(A1:A5). All formulas supported by Microsoft Excel are supported by HTML5 Spreadsheet Editor too.

[![][8]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/09/38472.png)

### Working with Rows

Adding and removing rows is very easy. The first column of the spreadsheet shows the row ID. Click on a row ID to select the entire row. Right-click and click **Add a Row Below** to add a new row right below the selected row. You can remove a row by following same method and clicking **Delete Row**.

[![][9]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/09/82348.png)

### Saving a File

After you are finished editing, Click **Save** on the **Spreadsheet** menu. The modified file is available for download.

[![][10]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/09/3.png)

## Embed Anywhere

You can embed HTML5 Spreadsheet Editor in any website of your choice using IFRAME. Here is an example code:

`<iframe src="http://spreadsheet-editor.aspose.com/?url=http://example.com/Sample.xlsx" width="800" height="600">  
Your web browser does not support IFRAMEs  
</iframe>`

## Deployment

HTML5 Spreadsheet Editor requires any standard compliant Java application server that supports CDI. I have tested it on Glassfish 4.0. Just download the source code and build using Maven.

## Open Source

We love open source. Our choice of MIT license gives you the freedom to use, copy, modify and distribute our software without additional liabilities. Download the complete source code from your favourite site:

*   [HTML5 Spreadsheet Editor on Github][11]
*   [HTML5 Spreadsheet Editor on Codeplex][12]

## Feedback

Your feedback is very important to us. Download and run the app at your side. Feel free to suggest enhancements and report bugs.




[1]: http://www.gwtproject.org/
[2]: http://projects.spring.io/spring-framework/
[3]: https://javaserverfaces.java.net/
[4]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png "Aspose.Cells for Java logo"
[5]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/09/2.png "Spreadsheet Editor - Opened an Excel file"
[6]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/09/1.png "No document opened"
[7]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/09/463.png "Sheets"
[8]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/09/38472.png "Cell editing"
[9]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/09/82348.png "Adding rows"
[10]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/09/3.png "Save the file"
[11]: https://github.com/AsposeShowcase/Html5_Spreadsheet_Editor_by_Aspose_for_Java
[12]: https://en.wikipedia.org/wiki/CodePlex




