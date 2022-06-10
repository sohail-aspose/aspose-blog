---
title: 'Aspose Maven for NetBeans – New Plugin Released!'
date: Tue, 10 Feb 2015 12:40:08 +0000
draft: false
url: /2015/02/10/aspose-maven-for-netbeans-%e2%80%93-new-plugin-released/
author: Adeel Ilyas
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

Aspose releases new NetBeans IDE plugin to further facilitates Aspose for Java APIs in easy to use in Maven-based projects.



{{< figure align=center src="images/vXAQx9q.jpg" alt="">}}


New plugin **Aspose Maven for NetBeans** \- v1.0 comes with **Aspose Maven Project Wizard** which creates maven project by selecting Aspose Java APIs on the wizard steps (like Aspose.Words, Aspose.Pdf or Aspose.Cells) and add those selected Aspose API's maven dependencies into newly created maven project's pom.xml.

Previously, Aspose also released Aspose Maven Project Archetype 1.0 for the creation of Aspose Maven-based projects in Major IDEs including NetBeans IDE or through maven command line.

But this **Aspose Maven for NetBeans** plugin provides a more sophisticated solution through fine grained and guiding UI for selecting Aspose for Java APIs and Maven project artifact inputs.

The plugin fetches only the latest maven dependencies references from Aspose Cloud Maven repository and adds in the newly created maven project along with the configuration necessary for Aspose Cloud Maven repository.

## How to Install Aspose Maven Plugin for NetBeans IDE

This step by step tutorial will demonstrate you from the installation of the plugin to using Aspose Maven project wizard to create Aspose maven based projects in NetBeans IDE.

The **Aspose Maven Project Wizard** plugin can be directly downloaded from [plugin portal website][1], and then can be installed in NetBeans IDE (using **Tools** > **Plugins** > **Downloaded** > **Add plugin**).

But as this plugin is also available on the NetBeans Plugin Portal Update Center. For more convenient installation of this plugin

1.  Use '**Tools** > **Plugins**' action from the NetBeans IDE main menu
2.  Click '**Available** **Plugins**' Tab and type '**Aspose**' in search box. As shown below:
3.  Select '**Aspose Maven Project Wizard**' plugin and click **Install**
4.  Accept license agreement - MIT License for this plugin and Click **Install** as shown below:
5.  This will trigger installation of the plugin and you may be asked to '**Continue**' and also '**Finish**' the installation after which you can start using the plugin in NetBeans IDE without any restarts.

The Plugin will introduce a new project type – **Aspose Maven Project** – inside '**Maven'** category on New Project (Wizards) dialog in NetBeans, which will allow you to create Aspose Maven based Java projects inside the IDE.

## Aspose Maven Project

The Wizard allows developers to create Maven based project for using Aspose APIs inside NetBeans IDE. The desired [Aspose APIs][2] can be selected on wizards steps to include the maven dependencies in your creating maven based project

1.  Select **New Project** from NetBeans **File** menu
2.  Under **Maven** category of Wizards, select '**Aspose Maven Project'**
3.  Click **Next**.
4.  Provide a **Project Name** and **Location** just like when creating any Java application.
5.  Also provide **Group Id, Artifact Id,** **Version** and **Package** (optional field) for your maven project and click **Next**.
6.  Select **Aspose API(s)** from the list.
7.  Click **Finish**.  
    This will retrieve the selected Aspose APIs latest maven dependencies references from [Aspose Cloud Maven Repository][3].

Congratulations! you have successfully created Aspose maven based project for your selected Aspose APIs using Aspose Maven Project wizard inside the NetBeans IDE.

One cool thing, every time you create Maven project using the wizard will create maven project containing latest maven dependencies for the selected Aspose APIs along with the [Aspose Cloud Maven Repository][4] configuration in the pom.xml. See the snapshot below:



{{< figure align=center src="images/ji1NDF0.png" alt="">}}


Thanks to [Aspose Maven Project wizard][5] Plugin !

Now the created Aspose maven based project is ready to be enhanced as per your project's development needs inside the NetBeans IDE !

## Source Code Available

Aspose Maven Project Wizard for NetBeans is open source and its source code is available on the major social coding websites listed below. Developers can extend the functionality if they want or learn from it to make their own plugins.

*   **[GitHub][6]**
*   **[SourceForge][7]**
*   **[Bitbucket][8]**
*   **[CodePlex][9]**




[1]: https://netbeans.apache.org/
[2]: https://products.aspose.com/total
[3]: http://maven.aspose.com/artifactory/webapp/home.html?0
[4]: http://maven.aspose.com/artifactory/webapp/home.html?0
[5]: https://netbeans.apache.org/
[6]: https://github.com/asposemarketplace/Aspose_Maven_for_NetBeans/
[7]: https://sourceforge.net/p/asposemavenfornetbeans
[8]: https://bitbucket.org/asposemarketplace/aspose-maven-for-netbeans
[9]: https://en.wikipedia.org/wiki/CodePlex




