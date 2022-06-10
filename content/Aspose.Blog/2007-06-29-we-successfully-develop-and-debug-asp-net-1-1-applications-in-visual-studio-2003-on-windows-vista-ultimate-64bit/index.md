---
title: 'We successfully develop and debug ASP.NET 1.1 applications in Visual Studio 2003 on Windows Vista Ultimate 64bit'
date: Fri, 29 Jun 2007 02:42:00 +0000
draft: false
url: /2007/06/29/we-successfully-develop-and-debug-asp-net-1-1-applications-in-visual-studio-2003-on-windows-vista-ultimate-64bit/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

I've upgraded my development machine recently to Windows Vista Ultimate 64bit because we wanted to fully test Aspose.Words on Vista and on 64bit systems.

We have projects for both Visual Studio 2003 and 2005 as we build Aspose.Words both for .NET 1.1 and 2.0. Although Aspose.Words itself is just a class library (not an ASP.NET application) we do have ASP.NET demo application that ship with Aspose.Words. I had to get Visual Studio 2003 and 2005 with ASP.NET 1.1 and 2.0 working on the development machine, otherwise I would have had to go back Windows XP.

It was no big problem to get Visual Studio 2005 and ASP.NET 2.0 working, the normal installation procedure plus SP1 did the job.

It was more trouble with Visual Studio 2003. It worked okay, but ASP.NET 1.1 did not work. Could not create or open ASP.NET 1.1 application in Visual Studio. I hunted the web and several articles really helped. I just wanted to summarize my successful experience hoping it will help even more people to get Visual Studio 2003 working well on Vista.

Here are the articles that helped:

1\. [http://www.iis.net/articles/view.aspx/IIS7/Hosting-Web-Applications/ASP-NET/How-to-Run-ASP-NET-v1-1-on-IIS7][1]

I did install IIS Metabase Compatibility, .NET Framework 1.1 SP1 and ASP.NET Security Update for 1.1 as the article suggested. Although I did not do the other steps they offered.

2\. [http://citruslime.blogspot.com/2007/04/visual-studio-2003-web-debugging-on.html][2]

I checked my account is in the Debugger Users group. Then I followed the steps outlined in the article they refer to (next article). I also adjusted ISAPI and CGI extensions in the IIS manager (running aspnet\_regiis -enable did not seem to enable that).

After I created an ASP.NET 1.1 application using Visual Studio, I went to the IIS manager and set debugging and authentication settings like they suggested.

Debugging the application was still not possible at this stage. The error was "cannot debug because the URL is in the Internet Zone". I added [http://localhost][3] to the Intranet Zone in Internet Explorer secruty options and after that I was finally able to debug ASP.NET applications.

3\. [http://blogs.iis.net/brian-murphy-booth/archive/2007/03/09/how-to-setup-asp-net-v1-1-visual-studio-net-2003-projects-on-iis7-vista.aspx][4]

This article contains the most important steps.

Disclaimer: Use at your own risk and sorry, I will not have time to help you with problems as debugging ASP.NET 1.1 application on Vista is not my main job.




[1]: http://www.iis.net/articles/view.aspx/IIS7/Hosting-Web-Applications/ASP-NET/How-to-Run-ASP-NET-v1-1-on-IIS7
[2]: http://citruslime.blogspot.com/2007/04/visual-studio-2003-web-debugging-on.html
[3]: http://localhost
[4]: http://blogs.iis.net/brian-murphy-booth/archive/2007/03/09/how-to-setup-asp-net-v1-1-visual-studio-net-2003-projects-on-iis7-vista.aspx



