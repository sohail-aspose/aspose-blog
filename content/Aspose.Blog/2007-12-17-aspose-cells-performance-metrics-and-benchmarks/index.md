---
title: 'Aspose.Cells - Performance Metrics and Benchmarks'
date: Mon, 17 Dec 2007 15:27:00 +0000
draft: false
url: /2007/12/17/aspose-cells-performance-metrics-and-benchmarks/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

**Aspose.Cells and Competitors**

**Performance Metrics and Benchmarks**

**_Are you getting the performance that you’re paying for?_**

**Purpose**

Performance is very critical factor when choosing a component. This article measures the performance of **Aspose.Cells** and some similar products. The simple tests are conducted across the same operating system, .NET Framework, hardware components, and similar configurations.

This article presents performance measurements for different products including **Aspose.Cells**. Performance estimates presented here are intended to help you understand what to expect from different components in some commonly used scenarios under similar configurations on commodity hardware running widely used operating systems. Naturally, your application performance depends on your data, data access patterns, cache size, other configuration parameters, operating system and hardware etc. The benchmark aims to illustrate how the components perform under minimum hardware conditions, the faster the hardware, the faster the tasks will be processed by the components.

**Declaration**

This document is provided for information purposes only and the contents hereof are subjected to change without notice. This document is not warranted to be error-free, nor subject to any other warranties or conditions, whether expressed orally or implied in law, including implied warranties and conditions of merchantability or fitness for a particular purpose. We specifically disclaim any liability with respect to this document and no contractual obligations are formed either directly or indirectly by this document. This document may not be reproduced or transmitted in any form or by any means, electronic or mechanical, for any purpose.

**Introduction**

Benchmarks provide guidelines and help to set basic operational expectations. The topic shows benchmark tests that have been performed with different potential components. The Performance Measures allow even novice users to benchmark the performance the component they are using. By running through a battery of tests, taking only a few seconds / minutes, it will measure the speed of each component and gives an overall rating. The tests will  allow you to objectively benchmark a component using a variety of different speed tests then compare the results to other components. All the tasks are common and carefully chosen exploring each component’s features to make sure that all the components may complete the tasks with ease. Moreover, the APIs to perform a test by each component are carefully chosen and selected to get the best possible results that a component can produce while evaluating its performance and all the tasks were implemented twice / thrice to better judge the figures.

The benchmark results are presented as easy to read using tables and bar charts.

In addition to benchmarking, these tests  can be used to measure the effect of configuration changes and upgrades. Overall, the benchmark results are useful for evaluating the following key points:

 **• Find out if your component is performing at its best.**

 **• Compare the performance of one component to other similar components.**

 **• Measure the effect of configuration changes and upgrades.**

 **• Avoid paying for overpriced components only to get poor performance.**

 **• Make objective independent measurements on which to base your purchasing**

 **decision.**

 **• Measure the graph performance of the benchmarks related to a component.**

**Components Participating in the Quest**

After searching the potential products in the market we come up with some products / components. According to our policies, we don’t mention the names of our competitors. We do not disrespect our competitors and don’t want to disregard them either. This document has only informative purpose for the users. So, we will only call them as Product1, Product2 etc. We choose **4** components including **Aspose.Cells**. (**Note:** To make them equal we chose the evaluation versions of all the products involved):

 **• Aspose.Cells**

 **• Product1**

 **• Product2**

 **• Product3**

**System Hardware**

The benchmark aims to illustrate how the components perform under the minimum hardware conditions. We performed all the tests on a single processor Intel Celeron(R) CPU 2.40GHz with 512 MB RAM and running Windows XP.

**Note:** These tests were conducted at some time using a specific version of **Aspose.Cells** component. **Aspose.Cells** team always try to optimize the component related quality and performance with every new release of the product. So, it is quite possible that you can get even better results using the same hardware and system configurations.

**Testing Methodology**

All the performance tests were conducted on a common hardware and  operating system combinations, without customized configuration, tuning or any  other performance enhancing techniques. All tests were run with the component installations  on the same system that were otherwise quiescent. To get accurate readings, we performed all the tasks twice / thrice at a time to better evaluate a component and to get accurate readings.

**Task Categories**

We chose some common tasks under the following two categories in **WinForms**, both the categories consisted of some common scenarios, each scenario represented a common task which was performed by each component:

**1.** **Creating Excel File(s) from the scratch.**

**2.** **Reading** **/ Updating existing Excel File(s).**

**Creating Excel File(s) from the scratch**

In this category, there were three scenarios used. i.e. Scenario1, Scenario2, Scenario3.

**Scenario1**

This scenario denotes a common **Task** that  presents how and at which speed the different components would achieve and complete a task on the same system. In this scenario, a certain number of excel files filled with common data are to be created from the scratch. Each file represents a workbook with a fixed number of worksheets in it. In this scenario, we measured benchmarking results of **Aspose.Cells**, **Product1**, **Product2** and **Product3**.

**Task:**

Create 50 XLS File(s). Each Workbook contains five worksheets with 150 \* 50 records in each worksheet. Each worksheet is filled with constant (similar) data into the cells.

**Code Snippets**

We wrote code snippets used by different components with awareness to accomplish the task. The APIs to perform the task for each component are parallel and carefully selected to specify the best possible way to obtain the results to measure the performance. Due to some internal reasons and our policies, we only provide **Aspose.Cells** code segment here.

using Aspose.Cells;  
.  
.  
.  
.  
private void button2\_Click(object sender, System.EventArgs e)  
{  
try  
         {  
         saveFileDialog.FileName = "AsposeSample.xls";  
         saveFileDialog.Filter = "Microsoft Excel Workbooks (\*.xls) | \*.xls";  
         if (saveFileDialog.ShowDialog() == DialogResult.OK)  
                  {  
                         CreateAsposeCellsFiles(saveFileDialog.FileName);  
                  }  
         }  
  
         catch (Exception ex)  
         {  
          MessageBox.Show(ex.Message,"Error",MessageBoxButtons.OK,MessageBoxIcon.Error);  
         }  
}  
private void CreateAsposeCellsFiles(string filename)  
{  
       DateTime start = DateTime.Now;  
         for (int wkb = 0; wkb<50;wkb++)  
         {  
             Workbook workbook = new Workbook();  
             workbook.Worksheets.RemoveAt(0);   

             for(int i = 0;i<5;i++)  
             {  
                  Worksheet ws = workbook.Worksheets\[workbook.Worksheets.Add()\];  
                  ws.Name = i.ToString();  
                  for (int row=0;row<150;row++)  
                         {  
                            for (int col =0;col<50; col++ )  
                              {  
                                  ws.Cells\[row,col\].PutValue("row" + row.ToString() + " col" + col.ToString());  
                               }  
  
                           }  
                  }  
                  workbook.Save(filename + wkb.ToString()+ ".xls");   
         }  
         DateTime end = DateTime.Now;  
         TimeSpan time = end -start;  
        MessageBox.Show("50 File(s) Created! \\n" + "Time consumed (Seconds): " + time.TotalSeconds.ToString(),"I n f o",MessageBoxButtons.OK,MessageBoxIcon.Information);  
  
}

**Task Results (Scenario1)**

The results show that **Aspose.Cells** used 17.21 seconds to complete the task, **Product1** consumed 33.67 seconds to complete the task, **Product2** spent 23.62 seconds to complete the task and **Product3** utilized 70.95 seconds to complete the task. So, **Aspose.Cells** took the least time to finish the task and **Product3** took the utmost time for the task. We reviewed the file(s) created by each component to check data, they are fine tuned as described in response to their respective code snippets. The following table provides a quick view for the **Task** results:

**Component**

**Name**

**Scenario1 **

**(Task Completion Time in Sec)**

**Achieved Results**

**Status**

**Aspose.Cells**

17.21

OK

**Product1**

33.67

OK

**Product2**

23.62

OK

**Product3**

70.95

OK

**Scenario2**

This scenario denotes a common **Task** that  specifies how and at which speed the different components would achieve and complete a task on the same system. In this scenario, an excel file filled with some dummy data are to be created from the scratch. The file represents a workbook with a single worksheet in it. In this scenario, we measured benchmarking results of **Aspose.Cells**, **Product1** and **Product3**. **Product2** does not qualify to participate in this expedition as its evaluation version does not allow this.

**Task:**

Create an XLS File. The Workbook contains a single worksheet with 10,000 \* 30 records. The worksheet is filled with similar dummy data into the cells.

**Code Snippets**

We wrote code snippets used by different components with awareness to accomplish the task. The APIs to perform the task for each component are parallel and carefully selected to specify the best possible way to obtain the results to measure the performance. Due to our policies, we only provide **Aspose.Cells** code segment here.

using Aspose.Cells;  
.  
.  
.  
.  
private void button2\_Click(object sender, System.EventArgs e)  
{  
         try  
         {  
         saveFileDialog.FileName = "CellsSample.xls";  
         saveFileDialog.Filter = "Microsoft Excel Workbooks (\*.xls) | \*.xls";  
         if (saveFileDialog.ShowDialog() == DialogResult.OK)  
            {  
                CreateAsposeCellsFile(saveFileDialog.FileName);  
            }  
         }  
         catch (Exception ex)  
         {  
          MessageBox.Show(ex.Message,"Error",MessageBoxButtons.OK,MessageBoxIcon.Error);  
  
         }  
}  
private void CreateAsposeCellsFile(string filename)  
{  
         DateTime start = DateTime.Now;  
         Workbook workbook = new Workbook();  
         Worksheet ws = workbook.Worksheets\[0\];  
         for (int row=0;row<10000;row++)  
         {  
                  for (int col =0;col< 30; col++ )  
                  {  
                           ws.Cells\[row,col\].PutValue(row.ToString() + "," + col.ToString());  
                  }  
         }  
        workbook.Save(filename);   
        DateTime end = DateTime.Now;  
        TimeSpan time = end -start;  
        MessageBox.Show("File Created! \\n" + "Time consumed (Seconds): " + time.TotalSeconds.ToString(),"I n f o",MessageBoxButtons.OK,MessageBoxIcon.Information);  
  
}

**Task Results (Scenario2)**

The results show that **Aspose.Cells** used 7.51 seconds to complete the task, **Product1** consumed 9.30 seconds to complete the task, and **Product3** spent 14.14 seconds to complete the task. So, **Aspose.Cells** took the least time to finish the task and **Product3** took the utmost time for the task. We reviewed the file created by each component to check data, it is fine tuned as described in response to their code snippets. The following table provides a quick view for the **Task** results:

**Component**

**Name**

**Scenario2 **

**(Task Completion Time in Sec)**

**Achieved Results**

**Status**

**Aspose.Cells**

7.51

OK

**Product1**

9.30

OK

**Product3**

14.14

OK

**Scenario3**

This scenario denotes a common **Task** that  represents how and at which speed the different components would achieve and complete a task on the same system. In this scenario, an excel file filled with similar data are to be created from the scratch. The file represents a workbook with a fixed number of worksheets in it. In this scenario, we measured benchmarking results of **Aspose.Cells**, **Product1**, **Product2** and **Product3**.

**Task:**

Create an XLS File. The Workbook contains five worksheets with 150 \* 56 records in each worksheet. Each worksheet is filled with similar data into the cells.

**Code Snippets**

We wrote code snippets used by different components with awareness to accomplish the task. The APIs to perform the task for each component are parallel and carefully selected to specify the best possible way to obtain the results to measure the performance. Due to some internal reasons and our policies, we only provide **Aspose.Cells** code segment here.

using Aspose.Cells;  
.  
.  
.  
.  
private void button2\_Click(object sender, System.EventArgs e)  
{  
         try  
         {  
         saveFileDialog.FileName = "ACellsSample.xls";  
         saveFileDialog.Filter = "Microsoft Excel Workbooks (\*.xls) | \*.xls";  
         if (saveFileDialog.ShowDialog() == DialogResult.OK)  
                  {  
                           CreateAsposeCellsFile(saveFileDialog.FileName);  
                  }  
         }  
         catch (Exception ex)  
         {  
         MessageBox.Show(ex.Message,"Error",MessageBoxButtons.OK,MessageBoxIcon.Error);   
         }  
}  
private void CreateAsposeCellsFile(string filename)  
{  
         DateTime start = DateTime.Now;  
         Workbook workbook = new Workbook();  
         workbook.Worksheets.RemoveAt(0);  
         for(int i = 0;i<5;i++)  
         {  
               Worksheet ws = workbook.Worksheets\[workbook.Worksheets.Add()\];  
               ws.Name = i.ToString();  
               for (int row=0;row<150;row++)  
               {  
                      for (int col =0;col<56; col++ )  
                         {  
                                 ws.Cells\[row,col\].PutValue("row" + row.ToString() + " col" + col.ToString());  
                         }  
                }  
        }  
        workbook.Save(filename);   
        DateTime end = DateTime.Now;  
        TimeSpan time = end -start;  
        MessageBox.Show("File Created! \\n" + "Time consumed (Seconds): " + time.TotalSeconds.ToString(),"I n f o",MessageBoxButtons.OK,MessageBoxIcon.Information);  
  
}

**Task Results (Scenario3)**

The results show that **Aspose.Cells** used 0.42 seconds to complete the task, **Product1** consumed 0.78 seconds to complete the task, **Product2** spent 0.56 seconds to complete the task and **Product3** utilized 1.51 seconds to complete the task. So, **Aspose.Cells** took the least time to finish the task and **Product3** took the utmost time for the task. We reviewed the file created by each component to check data, it is fine tuned as described in response to their code snippets. The following table provides a quick view for the **Task** results:

**Component**

**Name**

**Scenario3 **

**(Task Completion Time in Sec)**

**Achieved Results**

**Status**

**Aspose.Cells**

0.42

OK

**Product1**

0.78

OK

**Product2**

0.56

OK

**Product3**

1.51

OK

**Graphical Display…….Creating Excel File(s) Scenarios**

The following image shows the graphical representation of Creating Excel File(s) Scenarios:

Note: Evaluation version of Product2 doesn’t allow us to test it on scenario2.

**Reading** **/ Updating existing Excel File(s)**

In this category, there were three scenarios used. i.e. Scenario1, Scenario2, Scenario3.

**Scenario1**

This scenario denotes a common **Task** that  presents how and at which speed the different components would achieve and complete a task on the same system. Here, we use a large excel file filled with common data. The file consists of a workbook with a fixed number of worksheets in it. We opened the file, replaced data into the cells in each worksheet and updated the file. In this scenario, we measured benchmarking results of **Aspose.Cells**, **Product1**, **Product2** and **Product3**.

**Task:**

Load a 10 MB XLS Template File. The Workbook contains 100 worksheets with 377 \* 18 records in each worksheet. Each worksheet is filled with similar data into the cells. Replace a string value of a cell in each worksheet and Save As the updated file.

**Code Snippets**

We wrote code snippets used by different components with awareness to accomplish the task. The APIs to perform the task for each component are parallel and carefully selected to specify the best possible way to obtain the results to measure the performance. Due to our policies, we only provide **Aspose.Cells** code segment here.

using Aspose.Cells;  
.  
.  
.  
.  
private void button2\_Click(object sender, System.EventArgs e)  
{  
       try  
         {  
         saveFileDialog.FileName = "CellsSample.xls";  
         saveFileDialog.Filter = "Microsoft Excel Workbooks (\*.xls) | \*.xls";  
         if (saveFileDialog.ShowDialog() == DialogResult.OK)  
                  {  
                           CreateAsposeCellsFile(saveFileDialog.FileName);  
                  }  
         }  
         catch (Exception ex)  
         {  
         MessageBox.Show(ex.Message,"Error",MessageBoxButtons.OK,MessageBoxIcon.Error);  
         }  
}  
private void CreateAsposeCellsFile(string filename)  
{  
        DateTime start = DateTime.Now;  
        Workbook workbook = new Workbook();  
        string path = Path.Combine(Path.GetDirectoryName(Application.ExecutablePath), @"..\\..\\");  
        string designerFile = path + "Templates\\\\SampleBook.xls";   
        workbook.Open(designerFile);  
        for(int i = 0;i<100;i++)  
        {  
                 Worksheet ws = workbook.Worksheets\[i\];   
                 ws.Cells\[0,0\].PutValue("Data" + i.ToString());  
        }  
        workbook.Save(filename);   
        DateTime end = DateTime.Now;  
        TimeSpan time = end -start;  
        MessageBox.Show("File Updated! \\n" + "Time consumed (Seconds): " + time.TotalSeconds.ToString(),"I n f o",MessageBoxButtons.OK,MessageBoxIcon.Information);  
  
}

**Task Results (Scenario1)**

The results show that **Aspose.Cells** used 5.23 seconds to complete the task, **Product1** consumed 18.35 seconds to complete the task, **Product2** spent 69.78 seconds to complete the task and **Product3** utilized 10.71 seconds to complete the task. So, **Aspose.Cells** took the least time to finish the task and **Product2** took the utmost time for the task. We reviewed the file(s) created by each component to check the data. Since **Product2** partially completed the task as its evaluation version only supports to create a workbook of maximum five worksheets with 150 records per sheet. All other components performed the task with 100% results. They are fine tuned as described in response to their code snippets. The following table provides a quick view for the **Task** results:

**Component**

**Name**

**Scenario1  **

**(Task Completion Time in Sec)**

**Achieved Results**

**Status**

**Aspose.Cells**

5.23

OK

**Product1**

18.35

OK

**Product2**

69.78

Partially Done

**Product3**

10.71

OK

**Scenario2**

This scenario denotes a common **Task** that  specifies how and at which speed the different components would achieve and complete a task on the same system. Here, we use a large excel file filled with common data. The file consists of a workbook with a fixed number of worksheets in it. We opened the file, inserted a fixed number of rows in each worksheet and updated the file. In this scenario, we measured benchmarking results of **Aspose.Cells**, **Product1**, **Product2** and **Product3**.

**Task:**

Load a 10 MB XLS Template File. The Workbook contains 100 worksheets with 377 \* 18 records in each worksheet. Each worksheet is filled with similar data into the cells. Insert 100 rows in each worksheet, fill them with string values and Save As the updated file.

**Code Snippets**

We wrote code snippets used by different components with awareness to accomplish the task. The APIs to perform the task for each component are parallel and carefully selected to specify the best possible way to obtain the results to measure the performance. Due to our policies, we only provide **Aspose.Cells** code segment here.

using Aspose.Cells;  
.  
.  
.  
.  
private void button2\_Click(object sender, System.EventArgs e)  
{  
       try  
         {  
         saveFileDialog.FileName = "CellsTest.xls";  
         saveFileDialog.Filter = "Microsoft Excel Workbooks (\*.xls) | \*.xls";  
         if (saveFileDialog.ShowDialog() == DialogResult.OK)  
                  {  
                           CreateAsposeCellsFile(saveFileDialog.FileName);  
                  }  
         }  
         catch (Exception ex)  
         {  
         MessageBox.Show(ex.Message,"Error",MessageBoxButtons.OK,MessageBoxIcon.Error);  
         }  
}  
private void CreateAsposeCellsFile(string filename)  
{  
        DateTime start = DateTime.Now;  
        Workbook workbook = new Workbook();  
        string path = Path.Combine(Path.GetDirectoryName(Application.ExecutablePath), @"..\\..\\");  
        string designerFile = path + "Templates\\\\SampleBook.xls";   
        workbook.Open(designerFile);   
        for(int i = 0;i<100;i++)  
         {  
                  Worksheet ws = workbook.Worksheets\[i\];  
                  Cells cells = ws.Cells;  
                  cells.InsertRows(0,100);  
                  for(int r=0;r<100;r++)  
                  {  
                           cells\[r,0\].PutValue("This is testing row #: " + r.ToString());  
                  }  
         }  
        workbook.Save(filename);   
        DateTime end = DateTime.Now;  
        TimeSpan time = end -start;  
        MessageBox.Show("File Updated! \\n" + "Time consumed (Seconds): " + time.TotalSeconds.ToString(),"I n f o",MessageBoxButtons.OK,MessageBoxIcon.Information);  
  
}

**Task Results (Scenario2)**

The results show that **Aspose.Cells** used 6.12 seconds to complete the task, **Product1** consumed 17.59 seconds to complete the task, **Product2** spent 69.04 seconds to complete the task and **Product3** utilized 27.32 seconds to complete the task. So, **Aspose.Cells** took the least time to finish the task and **Product2** took the utmost time for the task. We reviewed the file(s) created by each component to check the data. Since **Product2** partially completed the task as its evaluation version only supports to create a workbook of maximum five worksheets with 150 records per sheet. All other components performed the task with 100% results. They are fine tuned as described in response to their code snippets. The following table provides a quick view for the **Task** results:

**Component**

**Name**

**Scenario2 **

**(Task Completion Time in Sec)**

**Achieved Results**

**Status**

**Aspose.Cells**

6.12

OK

**Product1**

17.59

OK

**Product2**

69.04

Partially Done

**Product3**

27.32

OK

**Scenario3**

This scenario denotes a common **Task** that  specifies how and at which speed the different components would achieve and complete a task on the same system. Here, we use a large excel file filled with common data. The file consists of a workbook with a fixed number of worksheets in it. We opened the file, inserted a fixed number of columns in each worksheet and updated the file. In this scenario, we measured benchmarking results of **Aspose.Cells**, **Product1**, **Product2** and **Product3**.

**Task:**

Load a 10 MB XLS Template File. The Workbook contains 100 worksheets with 377 \* 18 records in each worksheet. Each worksheet is filled with similar data into the cells. Insert 10 columns in each worksheet, fill them with string values and Save As the updated file.

**Code Snippets**

We wrote code snippets used by different components with awareness to accomplish the task. The APIs to perform the task for each component are parallel and carefully selected to specify the best possible way to obtain the results to measure the performance. Due to our policies, we only provide **Aspose.Cells** code segment here.

using Aspose.Cells;  
.  
.  
.  
.  
private void button2\_Click(object sender, System.EventArgs e)  
{  
         try  
         {  
         saveFileDialog.FileName = "SampleCells.xls";  
         saveFileDialog.Filter = "Microsoft Excel Workbooks (\*.xls) | \*.xls";  
         if (saveFileDialog.ShowDialog() == DialogResult.OK)  
                  {  
                           CreateAsposeCellsFile(saveFileDialog.FileName);  
                  }  
         }  
         catch (Exception ex)  
         {  
         MessageBox.Show(ex.Message,"Error",MessageBoxButtons.OK,MessageBoxIcon.Error);  
         }  
}  
private void CreateAsposeCellsFile(string filename)  
{  
        DateTime start = DateTime.Now;  
        Workbook workbook = new Workbook();  
        string path = Path.Combine(Path.GetDirectoryName(Application.ExecutablePath), @"..\\..\\");  
        string designerFile = path + "Templates\\\\SampleBook.xls";   
        workbook.Open(designerFile);   
        for(int i = 0;i<100;i++)  
        {  
                 Worksheet ws = workbook.Worksheets\[i\];   
                 Cells cells = ws.Cells;   
                 for(int c=0;c<10;c++)  
                 {  
                          cells.InsertColumn(c);   
                          cells\[0,c\].PutValue("Column" + c.ToString());   
                 }   
        }  
        workbook.Save(filename);   
        DateTime end = DateTime.Now;  
        TimeSpan time = end -start;  
        MessageBox.Show("File Updated! \\n" + "Time consumed (Seconds): " + time.TotalSeconds.ToString(),"I n f o",MessageBoxButtons.OK,MessageBoxIcon.Information);  
  
}

 

**Task Results (Scenario3)**

The results show that **Aspose.Cells** used 7.10 seconds to complete the task, **Product1** consumed 16.81 seconds to complete the task, **Product2** spent 66.25 seconds to complete the task and **Product3** utilized 25.93 seconds to complete the task. So, **Aspose.Cells** took the least time to finish the task and **Product2** took the utmost time for the task. We reviewed the file(s) created by each component to check the data. Since **Product2** partially completed the task as its evaluation version only supports to create a workbook of maximum five worksheets with 150 records per sheet. All other components performed the task with 100% results. They are fine tuned as described in response to their code snippets. The following table provides a quick view for the **Task** results:

**Component**

**Name**

**Scenario3 **

**(Task Completion Time in Sec)**

**Achieved Results**

**Status**

**Aspose.Cells**

7.10

OK

**Product1**

16.81

OK

**Product2**

66.25

Partially Done

**Product3**

25.93

OK

**Graphical Display……. Reading / Updating existing Excel File(s) Scenarios**

The following image shows the graphical representation of Reading / Updating existing Excel File(s) Scenarios:








