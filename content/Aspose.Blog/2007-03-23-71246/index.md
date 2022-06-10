---
title: 'Adding glossary in Aspose.Pdf for .Net'
date: Fri, 23 Mar 2007 08:38:00 +0000
draft: false
url: /2007/03/23/71246/
author: Forever
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

Although glossary is not supported directly in Aspose.Pdf for .Net, it is possible to create glossary using the #$REFPAGE symbol. Here is an example:

\[c#\]

   //create Pdf and set license  
   Pdf pdf = new Pdf();  
   Aspose.Pdf.License lic = new Aspose.Pdf.License();  
   lic.SetLicense(@"D:\\CSharp\\Test\\License\\Aspose.Custom.lic.xml");  
   pdf.IsTruetypeFontMapCached = true;  
   pdf.TruetypeFontMapPath = @"d:\\test";

   //create new section  
   Section sec1 = pdf.Sections.Add();

   //create tables and add data  
   Table table1 = new Table();  
   table1.ColumnWidths = "200 100";  
   sec1.Paragraphs.Add(table1);  
     
   Row row1 = table1.Rows.Add();  
   Cell cell1 = row1.Cells.Add();  
   Heading heading1 = new Heading(pdf,sec1,1);  
   heading1.Segments.Add("KeyWord1: this is key word 1");  
   heading1.ID = "KeyWord1";  
   cell1.Paragraphs.Add(heading1);

   Cell cell2 = row1.Cells.Add("cell 2");

   //create another table  
   table1 = new Table();  
   table1.ColumnWidths = "200 100";  
   table1.IsFirstParagraph = true;  
   sec1.Paragraphs.Add(table1);  
     
   row1 = table1.Rows.Add();  
   cell1 = row1.Cells.Add();  
   heading1 = new Heading(pdf,sec1,1);  
   heading1.Segments.Add("KeyWord2: this is key word 2");  
   heading1.ID = "KeyWord2";  
   cell1.Paragraphs.Add(heading1);

   cell2 = row1.Cells.Add("cell 2");

   //add glossary  
   Text glossary = new Text("Glossary");  
   glossary.IsFirstParagraph = true;  
   glossary.TextInfo.FontSize = 20;  
   glossary.TextInfo.Alignment = AlignmentType.Center;  
   sec1.Paragraphs.Add(glossary);

   Text item1 = new Text("KeyWord1#$TAB#$REFPAGE(KeyWord1)");  
   item1.TabStops = new TabStops();  
   TabStop stop1 = item1.TabStops.Add(380,TabLeaderType.Dot);  
   sec1.Paragraphs.Add(item1);

   Text item2 = new Text("KeyWord2#$TAB#$REFPAGE(KeyWord2)");  
   item2.TabStops = new TabStops();  
   TabStop stop2 = item2.TabStops.Add(380,TabLeaderType.Dot);  
   sec1.Paragraphs.Add(item2);

   pdf.Save("d:/test/test.pdf");

\[VB.NET\]

        'create Pdf and set license  
        Dim pdf As Pdf = New Pdf  
        Dim lic As Aspose.Pdf.License = New Aspose.Pdf.License  
        lic.SetLicense("D:\\CSharp\\Test\\License\\Aspose.Custom.lic.xml")  
        pdf.IsTruetypeFontMapCached = True  
        pdf.TruetypeFontMapPath = "d:\\test"

        'create new section  
        Dim sec1 As Section = pdf.Sections.Add()

        'create tables and add data  
        Dim table1 As Table = New Table  
        table1.ColumnWidths = "200 100"  
        sec1.Paragraphs.Add(table1)

        Dim row1 As Row = table1.Rows.Add()  
        Dim cell1 As Cell = row1.Cells.Add()  
        Dim heading1 As Heading = New Heading(pdf, sec1, 1)  
        heading1.Segments.Add("KeyWord1: this is key word 1")  
        heading1.ID = "KeyWord1"  
        cell1.Paragraphs.Add(heading1)

        Dim cell2 As Cell = row1.Cells.Add("cell 2")

        'create another table  
        table1 = New Table  
        table1.ColumnWidths = "200 100"  
        table1.IsFirstParagraph = True  
        sec1.Paragraphs.Add(table1)

        row1 = table1.Rows.Add()  
        cell1 = row1.Cells.Add()  
        heading1 = New Heading(pdf, sec1, 1)  
        heading1.Segments.Add("KeyWord2: this is key word 2")  
        heading1.ID = "KeyWord2"  
        cell1.Paragraphs.Add(heading1)

        cell2 = row1.Cells.Add("cell 2")

        'add glossary  
        Dim glossary As Text = New Text("Glossary")  
        glossary.IsFirstParagraph = True  
        glossary.TextInfo.FontSize = 20  
        glossary.TextInfo.Alignment = AlignmentType.Center  
        sec1.Paragraphs.Add(glossary)

        Dim item1 As Text = New Text("KeyWord1#$TAB#$REFPAGE(KeyWord1)")  
        item1.TabStops = New TabStops  
        Dim stop1 As TabStop = item1.TabStops.Add(380, TabLeaderType.Dot)  
        sec1.Paragraphs.Add(item1)

        Dim item2 As Text = New Text("KeyWord2#$TAB#$REFPAGE(KeyWord2)")  
        item2.TabStops = New TabStops  
        Dim stop2 As TabStop = item2.TabStops.Add(380, TabLeaderType.Dot)  
        sec1.Paragraphs.Add(item2)

        pdf.Save("d:/test/test.pdf")








