---
title: 'Cell.Style property vs Cell.GetStyle/SetStyle method'
date: Thu, 10 Apr 2008 01:04:00 +0000
draft: false
url: /2008/04/10/cell-style-property-vs-cell-getstyle-setstyle-method/
author: Laurence
summary: ''
tags: ['apply cell style in excel', 'get or set cell style in excel', 'get or set cell style in excel programmatically', 'modify excel cell style', 'update cell style in excel']
categories: ['Aspose.Cells Product Family']
---

Since v4.4.2, we add two new methods to format a cell: Cell.GetStyle method and Cell.SetStyle method. 

So now you can use the following two ways to format a cell:

1\. use Cell.Style property

\[C#\]

```
cell.Style.Font.IsBold = true;
```

\[VB.NET\]

```
cell.Style.Font.IsBold = True
```

 2. use Cell.GetStyle and Cell.SetStyle method

\[C#\]

```
Style style = cell.GetStyle();
style.Font.IsBold = true;
cell.SetStyle(style);
```

\[VB.NET\]

```
Dim style as Style = cell.GetStyle()
style.Font.IsBold = True
cell.SetStyle(style)
```

You can see that the first approach is easy and straight-forward. So why we add the second approach?

When you use the first piece of code, a Style object will be initiated for each cell when formatting it. So if there are a lot of cells to be formatted, a large amount of memory will be consumed because Style object is a large object. These Style objects won't be freed until calling Workbook.Save method.

So we add the second approach to optimize memory usage. After you use Cell.GetStyle method to retrieve a Style object, modify it and use Cell.SetStyle method to set back to this cell,  this Style object won't be preserved and .NET GC will collect it when it's not referenced. 

Actually when calling Cell.SetStyle method, Style object won't be saved for each cell. Instead, we compare this Style object to an internal Style object pool to see if it can be reused. Only different Style objects will be kept for each Workbook object. So there are only several hundred Style objects for each Excel file. For each cell, only an index to this Style object pool will be preserved.

We have tested it and find it will save a large amount of memory when processing very large Excel files.








