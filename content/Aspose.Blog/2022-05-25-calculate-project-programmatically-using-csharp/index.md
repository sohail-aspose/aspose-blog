---
title: 'Calculate Project Programmatically using C#'
date: Wed, 25 May 2022 07:47:21 +0000
draft: false
url: /2022/05/25/calculate-project-programmatically-using-csharp/
author: 'Muzammil Khan'
summary: '. As a C# developer, you can easily set project calculation mode in .NET applications and calculate project properties. In this article, you will learn **how to calculate a project programmatically using C#**.'
tags: ['Automatic Project Calculation C#', 'Calculate Task Finish Date C#', 'Manual Project Calculation C#', 'Project Calculation in C#', 'Project Duration Calculation']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/calculate-project-programmatically-using-csharp.jpg" alt="Calculate Project Programmatically using C#">}}


We can calculate project schedules or costs using calculation modes defined in Project options for Microsoft Project. A project schedule shows the start and end date of all project tasks. Microsoft Project allows the project calculation manually or automatically. As a C# developer, we can easily set project calculation mode in .NET applications and calculate project properties. In this article, we will learn **how to calculate a project programmatically using C#**.

The following topics shall be covered in this article:

*   [C# API to Calculate Project Programmatically][1]
*   [Manual Project Calculation][2]
*   [Automatic Project Calculation][3]
*   [No Project Calculation Mode][4]

## C# API to Calculate Project Programmatically {#CSharp-API-to-Calculate-Project-Programmatically}

For setting project calculation modes, we will be using the [Aspose.Tasks for .NET][5] API. It provides three project calculation modes, to calculate the values of dependent properties. These calculation modes are:

*   None – it sets only necessary properties and does not recalculate project dates and costs.
*   Manual – it sets only dependent object properties without recalculation of project dates and costs.
*   Automatic – it recalculates project dates and cost properties automatically.

The API defines above-mentioned calculation modes in the **_[CalculationMode][6]_** enumeration. The **_[CalculationMode][7]_** property of the **_[Project][8]_** class allows setting or getting the value of the **_CalculationMode_**. The API also allows manipulating an existing project in order to add some modifications. Moreover, it facilitates performing basic as well as advanced project management operations seamlessly. Please either [download][9] the DLL of the API or install it using [NuGet][10].

```
PM> Install-Package Aspose.Tasks
```

## Manual Project Calculation using C# {#Manual-Project-Calculation-using-CSharp}

We can set the calculation mode to manual and verify it by following the steps given below:

1.  Firstly, create an instance of the **_Project_** class.
2.  Next, set calculation mode to **_Manual_**.
3.  Then, specify the project start date.
4.  Next, add new tasks, e.g., Task 1, and Task 2.
5.  Then, read task properties set in manual mode.
6.  After that, initialize an object of the **_[TaskLinks][11]_** class and link tasks.
7.  Finally, verify the start and end date of Task 2.

The following code sample shows **how to manually calculate a project using C#**.

{{< gist aspose-tasks-gists 0ed2869bae1ffd5a983265ad5df2452c "Calculate-Project-Programmatically-CSharp_ManualCalculation.cs" >}}

```
Task1.Id Equals 1 : True
Task1 OutlineLevel Equals 1 : True
Task1 Start Equals 15/04/2015 08:00 AM : True
Task1 Finish Equals 15/04/2015 05:00 PM : True
Task1 Duration Equals 1 day : True
Task2 Start Equals 15/04/2015 08:00 AM : True
Task2 Finish Equals 15/04/2015 05:00 PM : True
Task2 Duration Equals 1 day : True
Task1 Start Equals Task2 Start : True
Task1 Finish Equals Task2 Finish : True
```

## Automatic Project Calculation using C# {#Automatic-Project-Calculation-using-CSharp}

We can set the calculation mode to automatic and verify it by following the steps given below:

1.  Firstly, create an instance of the **_Project_** class.
2.  Next, set calculation mode to **_Automatic_**.
3.  Then, set the project start date.
4.  Now, add new tasks, e.g., Task 1, and Task 2.
5.  After that, initialize an object of the **_[TaskLinks][12]_** class and link tasks.
6.  Finally, verify the recalculated dates.

The following code sample shows **how to calculate the project automatically using C#**.

{{< gist aspose-tasks-gists 0ed2869bae1ffd5a983265ad5df2452c "Calculate-Project-Programmatically-CSharp_AutomaticCalculation.cs" >}}

```
Task1 Start + 1 Equals Task2 Start : True
Task1 Finish + 1 Equals Task2 Finish : True
RootTask Finish Equals Task2 Finish : True
Project Finish Date Equals Task2 Finish : True
```

## No Project Calculation Mode in C# {#No-Project-Calculation-Mode-in-CSharp}

We can set the calculation mode to automatic and verify it by following the steps given below:

1.  Firstly, create an instance of the **_Project_** class.
2.  Next, set calculation mode to **_None_**.
3.  Then, specify the project start date.
4.  Next, add a new task, e.g., Task 1.
5.  Then, read task properties.
6.  After that, set task duration in days.
7.  Finally, verify the start and end date of the Task.

The following code sample shows **how to set project calculation to none using C#**.

{{< gist aspose-tasks-gists 0ed2869bae1ffd5a983265ad5df2452c "Calculate-Project-Programmatically-CSharp_NoCalculation.cs" >}}

```
Task.Id Equals 0 : True
Task.OutlineLevel Equals 0 : False
Task Start Equals DateTime.MinValue : True
Task Finish Equals DateTime.MinValue : True
Task Duration Equals 0 mins : True
Task Duration Equals 2 days : True
Task Start Equals DateTime.MinValue  : True
Task Finish Equals DateTime.MinValue  : True
```

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][13] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned **how to set project calculation modes programmatically**. We have also seen how values of dependent properties are calculated in each calculation mode using C#. Besides, you can learn more about Aspose.Tasks for .NET API using the [documentation][14]. In case of any ambiguity, please feel free to contact us on the [forum][15].

## See Also

*   [Create or Read Projects on Project Server or Project Online][16]




[1]: #CSharp-API-to-Calculate-Project-Programmatically
[2]: #Manual-Project-Calculation-using-CSharp
[3]: #Automatic-Project-Calculation-using-CSharp
[4]: #No-Project-Calculation
[5]: https://products.aspose.com/tasks/net/
[6]: https://apireference.aspose.com/tasks/net/aspose.tasks/calculationmode/
[7]: https://apireference.aspose.com/tasks/net/aspose.tasks/project/calculationmode/
[8]: https://apireference.aspose.com/tasks/net/aspose.tasks/project/#project-class
[9]: https://downloads.aspose.com/tasks/net
[10]: https://www.nuget.org/packages/Aspose.Tasks/
[11]: https://apireference.aspose.com/tasks/net/aspose.tasks/tasklink/
[12]: https://apireference.aspose.com/tasks/net/aspose.tasks/tasklink/
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/tasks/net/
[15]: https://forum.aspose.com/c/tasks/
[16]: https://blog.aspose.com/2020/03/20/create-read-projects-on-project-server-and-project-online-in-csharp-asp-net/




