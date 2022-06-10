---
title: 'How to Insert Check Boxes or Other Form Fields During Mail Merge'
date: Sun, 14 Jan 2007 20:08:00 +0000
draft: false
url: /2007/01/14/65290/
author: Romank
summary: ''
tags: ['Insert Checkbox to Word Document', 'Insert checkbox to word during mail merge', 'insert form fields to word mail merge']
categories: ['Aspose.Words Product Family']
---

As you probably know, one of the interesting Aspose.Words features is the reporting (mail merge) engine. The mail merge engine takes a document on input, looks for MERGEFIELD fields in it and replaces them with data it obtains from the data source. Normally, simple text is inserted, but a customer asked if it is possible to generate a document where boolean data values are output as check box form fields.

The answer is yes - it is possible and it is very easy, thanks to the ability to extend the mail merge process using event handlers. The [Aspose.Words.Reporting.MailMerge][1] object provides [MergeField][2] and [MergeImageField][3] event handlers.

Other interesting examples of extending standard mail merge using event handlers are:

*   Insert HTML into merge fields (sample code in the documentation for the MergeField event).
*   Insert images from any custom storage (files, BLOB fields etc).
*   Insert text with formatting (font, size, style etc).

This thread is the original discussion about inserting check boxes and also contains the complete sample project you can use.

**This screenshot of Microsoft Word shows the template document with merge fields:**

**This screenshot of Microsoft Word shows the generated document. Note some fields were replaced with simple text, some fields were replaced with check box form fields and the Subject field was replaced with a text input form field.**

Here is the code if you need it quickly. Sorry it is hard to format code snippets in this blog nicely.

```
using System;

using System.Data;

using System.IO;

using System.Reflection;

using Aspose.Words;

using Aspose.Words.Reporting;

namespace Project

{

/// <summary>

/// This sample shows how to insert check boxes and text input form fields during mail merge into a document.

/// </summary>

class Demo

{

/// <summary>

/// The main entry point for the application.

/// </summary>

[STAThread]

static void Main(string[] args)

{

Demo demo = new Demo();

demo.Execute();

}

private void Execute()

{

// Get the bin directory.

string binDir = Path.GetDirectoryName(Assembly.GetExecutingAssembly().Location);

// The templates are stored in the directory one level up.

string templateDir = Path.GetDirectoryName(binDir);

// Load the template document.

Document doc = new Document(Path.Combine(templateDir, "Template.doc"));

// Setup mail merge event handler to do the custom work.

doc.MailMerge.MergeField += new MergeFieldEventHandler(HandleMergeField);

// The mail merge event handler will use this document builder object to do its work.

mBuilder = new DocumentBuilder(doc);

// Get the data for mail merge.

DataTable table = GetDataTable();

// Execute the mail merge.

doc.MailMerge.Execute(table);

// Save the finished document.

doc.Save(Path.Combine(templateDir, "Template Out.doc"));

}

private DataTable GetDataTable()

{

// We create a hardcoded table here. In the real application you would get the data from a database.

DataTable table = new DataTable();

// Create some columns in the data table.

table.Columns.Add("RecipientName", typeof(string));

table.Columns.Add("SenderName", typeof(string));

table.Columns.Add("FaxNumber", typeof(string));

table.Columns.Add("PhoneNumber", typeof(string));

table.Columns.Add("Subject", typeof(string));

table.Columns.Add("Body", typeof(string));

table.Columns.Add("Urgent", typeof(bool));

table.Columns.Add("ForReview", typeof(bool));

table.Columns.Add("PleaseComment", typeof(bool));

// Add some rows.

table.Rows.Add(new object[] {"Josh", "Jenny", "123456789", "", "Hello", "Test message 1", true, false, true});

table.Rows.Add(new object[] {"Bob", "Jenny", "444 327589", "", "Bye", "Test message 2", false, true, false});

return table;

}

/// <summary>

/// This handler is called for every mail merge field found in the document,

/// for every record found in the data source.

/// </summary>

private void HandleMergeField(object sender, MergeFieldEventArgs e)

{

// We decided that we want all boolean values to be output as check box form fields.

if (e.FieldValue is bool)

{

// Move the "cursor" to the current merge field.

mBuilder.MoveToMergeField(e.FieldName);

// It is nice to give names to check boxes. Lets generate a name such as MyField21 or so.

string checkBoxName = string.Format("{0}{1}", e.FieldName, e.RecordIndex);

// Insert a check box.

mBuilder.InsertCheckBox(checkBoxName, (bool)e.FieldValue, 0);

// Nothing else to do for this field.

return;

}

// Another example, we want the Subject field to come out as text input form field.

if (e.FieldName == "Subject")

{

mBuilder.MoveToMergeField(e.FieldName);

string textInputName = string.Format("{0}{1}", e.FieldName, e.RecordIndex);

mBuilder.InsertTextInput(textInputName, TextFormFieldType.RegularText, "", (string)e.FieldValue, 0);

}

}

private DocumentBuilder mBuilder;

}

}
```




[1]: https://blog.aspose.com/category/words/
[2]: https://blog.aspose.com/category/words/
[3]: https://blog.aspose.com/category/words/




