---
title: 'Create MS Outlook Tasks in Python'
date: Thu, 28 Apr 2022 17:50:26 +0000
draft: false
url: /2022/04/28/create-ms-outlook-tasks-in-python/
author: ''Usman Aziz''
summary: '[MS Outlook][1] allows you to create to-do lists that are comprised of different tasks. Each task is an activity that is to be performed within a particular period of time. Thus, you can keep track of the tasks assigned to you. While automating MS Outlook operations, you may need to work with Outlook tasks. Accordingly, in this article, you will learn **how to create MS Outlook tasks programmatically in Python**.'
tags: ['Add Reminder to Outlook Tasks Python', 'Adding Recurrence to Outlook Task in Python', 'Create a Task on MS Outlook in Python', 'Python Library to Create MS Outlook Tasks', 'python email library']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Create-MS-Outlook-Tasks.png" alt="Create MS Outlook Tasks in Python">}}


[MS Outlook][2] allows you to create to-do lists that are comprised of different tasks. Each task is an activity that is to be performed within a particular period of time. Thus, you can keep track of the tasks assigned to you. While automating MS Outlook operations, you may need to work with Outlook tasks. Accordingly, in this article, you will learn **how to create MS Outlook tasks programmatically in Python**.

*   [Python Library to Create MS Outlook Tasks][3]
*   [Create an MS Outlook Task][4]
*   [Add Reminder to Outlook Tasks][5]
*   [Add Recurrence to Outlook Tasks][6]

## Python Library to Create MS Outlook Tasks {#Python-Library-to-Create-MS-Outlook-Tasks}

To work with tasks in MS Outlook, we will use [Aspose.Email for Python][7]. It is a feature-rich email processing library that lets you create and send emails seamlessly. Furthermore, it allows you to work with popular email clients such as MS Outlook. You can install the library from [PyPI][8] using the following command.

```
> pip install Aspose.Email-for-Python-via-NET
```

## Create an MS Outlook Task in Python {#Create-a-Task-on-MS-Outlook}

The following are the steps to create an MS Outlook task in Python.

*   Create an instance of **MapiTask** class.
*   Set task's name, description, starting date and time, and ending date and time.
*   Set other properties such as percentage complete, history, owner, etc.
*   Save the task using **MapiTask.save()** method.

The following code sample shows how to create an MS Outlook task in Python.

{{< gist aspose-com-gists e671798a702d48e70070f7558eb156d9 "create-task.py" >}}

## Add Reminder to Outlook Tasks in Python {#Add-Reminder-to-Outlook-Tasks}

You can also attach the reminder information to an MS Outlook task. In addition, you can set the reminder's sound from a file on disk. The following are the steps to add reminder information to an Outlook task in Python.

*   Create an instance of **MapiTask** class.
*   Set properties of the task such as name, description, date and time, etc.
*   Enable reminder using **MapiTask.reminder\_set** property.
*   Set reminder time using **MapiTask.reminder\_time** property.
*   Set reminder sound using **MapiTask.reminder\_file\_parameter** property.
*   Save the task using **MapiTask.save()** method.

The following code sample shows how to set reminder information for an MS Outlook task in Python.

{{< gist aspose-com-gists e671798a702d48e70070f7558eb156d9 "add-reminder-to-task.py" >}}

## Add Recurrence to Outlook Tasks in Python {#Adding-Recurrence-to-Outlook-Task}

You can also create a recurring task where the recurrence can be daily, weekly, monthly, or yearly. The following are the steps to add recurrence to an Outlook task in Python.

*   Create an instance of **MapiTask** class.
*   Set properties of the task such as name, description, date and time, etc.
*   Create an instance of **MapiCalendarDailyRecurrencePattern** class.
*   Set pattern type, period, and other recurrence properties.
*   Assign **MapiCalendarWeeklyRecurrencePattern** pattern to task using **MapiTask.recurrence** property.
*   Save the task using **MapiTask.save()** method.

The following code sample shows how to add recurrence to an MS Outlook task in Python.

{{< gist aspose-com-gists e671798a702d48e70070f7558eb156d9 "add-recurrence-to-task.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.Email for Python for free by [getting a temporary license][9].

## Conclusion

In this article, you have learned how to create MS Outlook tasks in Python. Furthermore, you have seen how to add reminder and recurrence information to MS Outlook tasks programmatically. In addition, you can explore more about Aspose.Email for Python using [documentation][10]. Also, you can post your questions or queries on our [forum][11].

## See Also

*   [Send Emails in Python - Python Email API][12]




[1]: https://en.wikipedia.org/wiki/Microsoft_Outlook
[2]: https://en.wikipedia.org/wiki/Microsoft_Outlook
[3]: #Python-Library-to-Create-MS-Outlook-Tasks
[4]: #Create-a-Task-on-MS-Outlook
[5]: #Add-Reminder-to-Outlook-Tasks
[6]: #Adding-Recurrence-to-Outlook-Task
[7]: https://products.aspose.com/email/python-net
[8]: https://pypi.org/project/Aspose.Email-for-Python-via-NET/
[9]: https://purchase.aspose.com/temporary-license
[10]: https://docs.aspose.com/email/python-net/
[11]: https://forum.aspose.com/
[12]: https://blog.aspose.com/2021/05/21/send-emails-in-python/




