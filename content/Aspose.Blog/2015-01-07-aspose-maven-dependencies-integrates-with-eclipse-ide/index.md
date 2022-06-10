---
title: 'Aspose Maven Dependencies Integrate with Eclipse IDE'
date: Wed, 07 Jan 2015 17:45:39 +0000
draft: false
url: /2015/01/07/aspose-maven-dependencies-integrates-with-eclipse-ide/
author: Adeel Ilyas
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---



{{< figure align=center src="images/5oUoZPz.jpg" alt="">}}


With the launch of [Aspose Maven Dependencies through Aspose Cloud Maven repository][1] and the release of [Aspose Maven Archetype][2], it has been now possible to create Aspose Maven-based project on Major IDEs platforms or using any other tool/platform that understands the Maven standards and allow creating Maven-based project through Maven Archetypes quite easily.

## Aspose Maven Project Archetype - v1.0

This Archetype allows easy creation of the Aspose Maven-based project. You don’t even need to worry about the latest available versions for Aspose Java APIs as all latest version Aspose APIs Maven Dependencies will automatically be imported for the newly created Maven Project.

This will also add the required configuration of the Aspose Cloud Maven Repository to the Maven Project.

The blog will present a step by step tutorial as to how to use [Aspose Maven Archetype][3] for the seamless creation of Aspose Maven-based project on Eclipse IDE platform using Eclipse IDE native Maven Project Wizard.

## Configure Aspose Maven Archetype for Eclipse IDE

Below is the step by step guide that will lead you to configure Eclipse IDE for the creation of Aspose Maven Projects through [Aspose Maven Archetype][4].

1.  Fire up Eclipse IDE -in this tutorial I am using Eclipse Luna,
2.  Goto -> **File** > **New** \> **Other**
3.  New Project Wizards Dialog will appear, Select **Maven Project** and click Next as shown in below snapshot:![](http://i.imgur.com/b10CkBG.png)
4.  On next wizard step, uncheck "Create a simple project.." if checked and Click Next as shown below:![](http://i.imgur.com/e4fOKYh.png)
5.  The next screen will show a list of available Archetypes, here you need to add Aspose Maven Archetype for only one time:![](http://i.imgur.com/nxref9P.png)
6.  Click on Add Archetype... then Add Archetype Dialog will appear, provide information about [Aspose Maven Archetype][5] i.e GroupId, Artifact Id, Version and [Aspose Cloud Maven Repository][6] URL. Then click **OK** as shown in the below snapshot:**
    
    

{{< figure align=center src="images/RdVpSrt.png" alt="">}}

    
    **
7.  On adding Aspose Archetype, the new archetype as **aspose-java-for-maven** will appear in the list of Archetypes, as highlighted in the below snapshot:
    
    

{{< figure align=center src="images/S2XMkb3.png" alt="">}}

    

Congratulations! you’ve successfully configured your Eclipse IDE for creating Aspose Maven-based projects.

## Creating Aspose Maven Project

Now you can create Maven projects that will contain all the latest Aspose Java APIs Maven Dependencies and necessary Aspose Cloud Maven Repository configuration by following the steps as below:

1.  Goto -> **File** > **New** \> **Other**
2.  New Project Wizards Dialog will appear, Select **Maven Project** and click **Next** as shown in below snapshot:
    
    

{{< figure align=center src="images/b10CkBG.png" alt="">}}

    
3.  On next wizard step, uncheck **"Create a simple project.."** if checked and Click **Next** as shown below:
    
    

{{< figure align=center src="images/e4fOKYh.png" alt="">}}

    
4.  The next screen will show a list of available Archetypes, including **aspose-java-for-maven**, select it and click **Next**:
    
    

{{< figure align=center src="images/S2XMkb3.png" alt="">}}

    
5.  On screen shown below provide your creating Maven project Artifact values and click **Finish**:
    
    

{{< figure align=center src="images/KRZtxpq.png" alt="">}}

    
6.  The final screen will appear for your created Aspose Maven project, that will contain all latest Aspose Java APIs Maven Dependencies. Eclipse will start importing the Aspose Maven Dependencies to the local user maven repository as shown in below screenshot:
    
    

{{< figure align=center src="images/4jhAZqP.png" alt="">}}

    

Congratulations! you’ve successfully created your first Aspose Maven Project using **Aspose Maven Archetype** in Eclipse IDE.

### **Important Links**

*   [Aspose for Java components][7]
*   [Aspose Maven Dependencies Integrate with IntelliJ IDEA][8]
*   [Aspose Maven for JetBrains][9]
*   [Aspose Cloud Maven Repository][10]
*   [Aspose Maven JavaDocs Integration][11]




[1]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[2]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo
[3]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo
[4]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo
[5]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo
[6]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo
[7]: https://products.aspose.com/total/java
[8]: https://blog.aspose.com/2014/10/03/aspose-maven-dependencies-integrates-with-jetbrains-ide/
[9]: https://blog.aspose.com/2014/11/26/aspose-maven-for-jetbrains-new-plugin-released/
[10]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[11]: https://blog.aspose.com/2014/12/24/aspose-java-apis-javadocs-now-available-within-maven-based-projects/




