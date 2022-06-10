---
title: 'Aspose Maven for JetBrains - New Plugin Released!'
date: Wed, 26 Nov 2014 07:28:31 +0000
draft: false
url: /2014/11/26/aspose-maven-for-jetbrains-new-plugin-released/
author: Adeel Ilyas
summary: ''
tags: ['Aspose.Products', 'AsposeAPI', 'File Format API', 'Intellij', 'JavaAPI', 'MavenPlugin', 'plugin']
categories: ['Aspose.Words Product Family', 'Aspose.Total Product Family', 'Aspose.PDF Product Family', 'Aspose.Cells Product Family', 'Aspose.Email Product Family', 'Aspose.Slides Product Family', 'Aspose.Imaging Product Family', 'Aspose.BarCode Product Family', 'Aspose.Diagram Product Family', 'Aspose.Tasks Product Family', 'Aspose.OCR Product Family']
---

## Aspose Maven Dependencies Integration with IntelliJ IDEA

Aspose takes a further step in making Aspose for Java APIs in easy to use in Maven-based projects by releasing its new plugin for the IntelliJ IDEA platform, **Aspose Maven for JetBrains 1.0** that creates Aspose Maven-based projects by following the steps that come with the plugin in **Aspose Maven Project Wizard**.

Previously, Aspose released Aspose Maven Project Archetype 1.0 for the creation of Aspose Maven-based projects in any IDE including IntelliJ IDEA (which supports Maven) or using Maven command line project archetype generation.

But this **Aspose Maven for JetBrains** plugin provides a more sophisticated solution through fine grained and guiding UI for selecting Aspose for Java APIs and creating Maven project artifact value inputs. The plugin retrieves the latest available Maven artifacts for Aspose's Java APIs from the Aspose server and adds them into the newly created Maven project pom.xml along with the necessary configuration for the [Aspose Cloud Maven Repository][1].

## How to Install Aspose Maven Plugin for IntelliJ IDEA

This step by step tutorial demonstrates the steps to install the plugin and use the Aspose Maven Project Wizard to create Maven-based Aspose projects.

The Aspose Maven Project Wizard plugin is listed on IntelliJ IDEA’s [official website][2], so you don’t need to download it manually and install it from disk, but this extra option still exists in IntelliJ IDEA.

Aspose Maven Plugin can be easily installed from the IntelliJ IDEA CE Plugins repository enlisting the **Aspose Maven Project Wizard** plugin. To open it:

1.  Select **Settings** from the **File** menu.
2.  Click **Plugins**, then browse the repositories in IntelliJ IDEA.

# ![](http://i.imgur.com/Z9GS67H.png)

This plugin will introduce a new project type – ![ Aspose API for Java Integration with Jetbrains IDE][3]**Aspose Maven Project** – into IntelliJ IDEA, which will enable you to create Aspose Java APIs maven based projects.

## ![ Aspose API for Java Integration with Jetbrains IDE][4]Aspose Maven Project

The desired [Aspose APIs][5] can be selected to include the maven dependencies in your maven based project when creating a new maven project.

1\. Select **New Project**.  
2\. Select **Aspose Maven Project**  
3\. Click **Next**.

![](http://i.imgur.com/67EvJbh.png)

4\. Select **Aspose API(s)** from the list and click **Next**.

![](http://i.imgur.com/acjErJW.png)

5\. Provide a **GroupId, ArtifactId** and **Version** for your maven project and click **Next**.

![](http://i.imgur.com/3fOEnc2.png)

6\. Provide a **Project Name** and **Location** just like when creating any Java application

![](http://i.imgur.com/8xQsnur.png)

7\. Click **Finish**.  
This will retrieve the selected Aspose APIs latest maven dependencies references from Aspose Cloud    
Maven Repository.

![](http://i.imgur.com/fcSL6Pz.png)

Congratulations! You have successfully created an Aspose Maven-based project with the selected Aspose APIs' latest Maven dependencies and the Aspose Cloud Maven Repository configuration already present in pom.xml.

![](http://i.imgur.com/v6P09it.png)

The created Aspose Maven project is ready to be extended as per your project's requirements.

## Recommended Links

*   [Aspose Java Components][6]
    
*   [Download Aspose Maven for JetBrains for Manual Installation][7]
    
*   [Video tutorial showing how to use Aspose Maven Project Wizard to create Aspose maven based project in IntelliJ IDEA][8]
    
*   [How to configure Aspose Cloud Maven Repository in your existing maven projects and work with Aspose APIs within IntelliJ IDEA or any other IDE.][9]
    

*   Aspose Blog about Aspose Cloud Maven Repository

*   Aspose Blog about Aspose for IntelliJ Plugin (Aspose Java Project Wizard)  
    

## Source Code Available

Aspose Maven Project Wizard for JetBrains is open source and its source code is available on the major social coding websites listed below. Developers can extend the functionality if they want or learn from it to make their own plugins.

 **[![GitHub Mark icon2 Aspose API for Java Integration with Jetbrains IDE][10]](https://github.com/asposemarketplace/Aspose_for_JetBrains) [GitHub][11]**

 **[![sourceforge icon2 Aspose API for Java Integration with Jetbrains IDE][12]](https://sourceforge.net/projects/asposenetbeans) [SourceForge][13]**

 **[![bitbucket icon3 Aspose API for Java Integration with Jetbrains IDE][14]](https://bitbucket.org/asposemarketplace/aspose-for-netbeans) [Bitbucket][15]**

 **[![codeplex icon2 Aspose API for Java Integration with Jetbrains IDE][16]](https://netbeans.apache.org/) [CodePlex][17]**




[1]: http://maven.aspose.com/artifactory/webapp/home.html
[2]: https://plugins.jetbrains.com/plugin/7612?pr=idea_ce
[3]: https://camo.githubusercontent.com/b360643e823e0236ed55e2ae5a8de8e9c970ee92/687474703a2f2f692e696d6775722e636f6d2f70537a58656f772e706e67 "Aspose API for Java Integration with Jetbrains IDE"
[4]: https://camo.githubusercontent.com/0f4e42aa75ced964d24cf4332a8dfc5f208d882f/687474703a2f2f692e696d6775722e636f6d2f724a67775a73462e706e67 "Aspose API for Java Integration with Jetbrains IDE"
[5]: http://www.aspose.com/java/total-component.aspx
[6]: http://www.aspose.com/java/total-component.aspx
[7]: https://plugins.jetbrains.com/plugin/7612?pr=idea_ce
[8]: http://youtu.be/ChlojcMrWRY
[9]: https://docs.aspose.com/
[10]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/12/GitHub-Mark-icon2.png "GitHub-Mark-icon"
[11]: https://github.com/asposemarketplace/Aspose_Maven_for_JetBrains/ "GitHub"
[12]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/12/sourceforge-icon2.png "sourceforge-icon"
[13]: https://sourceforge.net/p/asposemavenforjetbrains "SourceForge"
[14]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/12/bitbucket-icon3.png "bitbucket-icon"
[15]: https://bitbucket.org/asposemarketplace/aspose-maven-for-jetbrains
[16]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/12/codeplex-icon2.png "codeplex-icon"
[17]: https://en.wikipedia.org/wiki/CodePlex




