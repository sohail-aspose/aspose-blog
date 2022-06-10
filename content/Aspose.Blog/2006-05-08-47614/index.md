---
title: 'Software Issues Troubleshooting'
date: Mon, 08 May 2006 03:27:00 +0000
draft: false
url: /2006/05/08/47614/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

Just decided to share some small but annoying issues I recently faced on my system as well as the probable ways to resolve. They have to do with several tiny little Microsoft products like Windows XP and its components, Word 2003, and Visual Studio 2003 :) Some of the issues are well known, others are a bit tricky – either way, I hope it will be helpful for people experiencing similar problems and came across this posting.

Please note some of the issues might have several solutions and I’m only posting here those appeared to be helpful to me. There’s no 100% guarantee they will work for you too – you should then search the Internet for other ways of resolving.

So what you should try if…

**…Internet Explorer window size unexpectedly gets ugly?**

**Symptoms.**  You launch IE and notice its window size does not fit your requirements (most likely too small). You resize it as you wish but next time you execute IE, the size of the window is ugly again.  
**Cause.** Never thought of.  
**Resolution.** Close all open IE windows, then run IE again. Right-click on any link and select **Open in New Window** on the popup menu. Resize the resulting secondary window to the size you wish for all secondary windows. Now **hold the Shift key** and close the window by clicking the Close button. Set the remaining window to the size you want IE to have when initially launched, and close it in the same way. IE should now remember your preferred window sizes. If the issue repeats after a while, perform these simple actions again.

**…you see a _Click to activate and use this control_ tooltip when mouse cursor hovers over a Flash animation in Internet Explorer?**

**Symptoms.** When you move mouse over a Flash animation in IE, a _Click to activate and use this control_ tooltip is popped up and the area where the animation is expected to appear gets bordered.  
**Cause.** This is a result of the recent IE update. Some time ago Microsoft lost a legal battle with a patent holder about the way Internet Explorer displays OBJECTs and EMBEDs in Web pages. Microsoft then decided to update the browser with changes requiring user input to display and activate ActiveX based media.  
**Resolution.** I personally do not suffer too much from this issue so I actually did nothing to fix it :) However, if you feel you ought to get rid of it, you can download and install a patch that reverts the default behaviour back to what it was prior to the update. Visit the following page to find the patch and all appropriate info:

[http://support.microsoft.com/default.aspx/kb/917425][1]

Remember you do that at your own risk.

**…some program icons are missed from system tray?**

**Symptoms.** You have several programs expected to put their icons into system tray (and they probably did that earlier) but the icons are just not there yet the programs are successfully loaded and running (seen in Task Manager).  
**Cause.** I read this is considered as a Windows XP bug so the real cause is unknown.  
**Resolution.** First, make sure the missed icons are not simply hidden as inactive :) If they aren’t, try go to _Start > My Network Places_ and click _Hide icons for networked UPnP devices_. Reboot your system. All expected icons should then appear in the tray. Note this action should not damage functioning of your UPnP devices. I have a router with the UPnP feature enabled and all my applications using this feature work fine.

**…system volume free disk space is decreasing constantly?**

**Symptoms.** Free disk space on a system volume is low and keeps decreasing although you do not install new software.  
**Cause.** The real cause is lazy developers who have not taught their programs to clean up what those programs leave on disks :)  
**Resolution.** Go to the _Documents and Settings\\%UserProfile%\\Local Settings\\Temp\\_ folder (note it is hidden by default). This is a default folder where applications store their temporary files during installation and running. Ideally, they should remove these files after they complete installation or working… but there’s nothing ideal in this world :) So there are several ways of cleaning this folder. The most radical way is just delete all the files manually. People over the Internet confirm it is safe; anyway, you will not be able to remove files in use because they are locked by system. I chose this method and successfully got rid of around 2.7 Gb garbage files! However, if you beware of doing something manually, you can use the standard disk cleanup tool (_Start > Control Panel > Performance and Maintenance > Free up space on your hard disk_) or download one of numerous specialized third-party tools from the Web. Other things to check are max amount of disk space occupied by temporary Internet files (_Start > Control Panel > Internet Options > General | Temporary Internet files | Settings > Temporary Internet files folder | Amount of disk space to use)_ and by the System Restore feature (_Start > Control Panel > Performance and Maintenance > System | System Restore | Drive settings | Settings > Disk space usage | Disk space to use_). These values seem to be set to some portion of the total drive space by default so they can be inadequately large.

**…Word 2003 shows strange gray marks at the corners of document pages?**

**Symptoms.** There are annoying gray marks at the corners of document pages when opening in Word looking like this:

The marks seem to outline page margins. And there’s no way to switch them off through Word GUI!!!  
**Cause.** Probably the marks are useful for something but they exasperated me at long last.  
**Resolution.** This issue popped up after I installed Microsoft Proofing Tools for Office 2003 (I selected complete install although I did not need all languages to be installed - just a stupid action). I did not know how to eliminate those marks until I came across a MS KB article (hasn’t kept the link unfortunately). The solution appeared to be simple. Just run _Start > All Programs > Microsoft Office > Microsoft Office Tools > Microsoft Office 2003 Language Settings_ and remove all Asian languages from the **Enabled languages** list. Do the opposite action if you need page margins to be outlined, though.  That’s it!

**…Visual Studio 2003 fails to load Web projects?**

**Symptoms.** When trying to open a Web project in VS2003, it shows the following error message: _Visual Studio .NET cannot create or open the application.  The likeliest problem is that required components are not installed on the local web server.  Run Visual Studio .NET setup and add the web development component.  
_**Cause.** Unknown.  
**Resolution.** This happened to me when I installed both VS2003 and VS2005 onto the same machine. Since many users are currently migrating to .NET 2.0, the issue might be popular. So, the first thing you should try to do is repair IIS by running the _aspnet\_regiis –i_ command in the Visual Studio 2003 command prompt. If this doesn’t help (and this most likely will not), just go to _Documents and Settings\\%UserProfile%\\_ and delete the _VSWebCache_ folder. This folder is created automatically by Visual Studio when you open/create a web project and VS should successfully recreate this folder when you open a Web project next time.




[1]: https://www.microsoft.com/en-pk



