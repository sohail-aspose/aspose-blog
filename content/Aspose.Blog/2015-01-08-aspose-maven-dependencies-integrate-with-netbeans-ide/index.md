---
title: 'Integrate Aspose Maven Dependencies with NetBeans IDE'
date: Thu, 08 Jan 2015 12:32:18 +0000
draft: false
url: /2015/01/08/aspose-maven-dependencies-integrate-with-netbeans-ide/
author: Adeel Ilyas
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---



{{< figure align=center src="images/vXAQx9q.jpg" alt="">}}


With the advent of [Aspose Maven Dependencies][1] through [Aspose Cloud Maven repository][2] and now with the release of [Aspose Maven Archetype][3], it has been very easy to work with Aspose Java APIs in Maven-based project because of the Aspose Maven projects easy creation on Major IDEs platforms including NetBeans IDE using Maven best practices.

Furthermore, Aspose maven dependencies can also be easily integrated on any other tool/platform that understands the Maven standards and supports Maven project creation from Archetype.

## Aspose Maven Project Archetype - v1.0

This Archetype allows easy creation of the Aspose Maven-based project. You don’t even need to worry about the latest available versions for Aspose Java APIs as all latest version Aspose APIs Maven Dependencies will automatically be imported for the newly created Maven Project.

This will also add the required configuration of the Aspose Cloud Maven Repository to the Maven Project.

The blog will present a step by step tutorial as to how to use [Aspose Maven Archetype][4] for the seamless creation of Aspose Maven-based project on NetBeans IDE platform using NetBeans IDE's native Maven Project Wizard.

## Creating Aspose Maven Project using Aspose Maven Archetype in NetBeans

You can create Maven projects that will contain all the latest Aspose Java APIs Maven Dependencies and necessary Aspose Cloud Maven Repository configuration by following the steps as below:

1.  Fire up NetBeans IDE - In this tutorial I am using NetBeans 8.0.1,
2.  Goto -> **File** > **New Project**
3.  "New Project" Dialog containing project wizards will appear.  
    Select **Maven > Project from Archetype** and Click **Next** as shown below:
4.  On next wizard step, you will see a list of available Archetypes, here please just enter the following information about [Aspose Maven Archetype][5]: **GroupId:** com.aspose  
    **Artifact Id:** aspose-java-for-maven  
    **Version:** 1.0  
    **Repository:** http://maven.aspose.com/artifactory/simple/ext-release-local/ As shown highlighted in the below snapshot, then click **Next.**
5.  On next screen, please provide your creating Maven project's Name, Location and Artifact values as shown in below snapshot and click **Finish**:
6.  Final screen will appear for your created Aspose Maven project, that will contain all latest Aspose Java APIs Maven Dependencies. NetBeans IDE will import all the defined Aspose Maven Dependencies in pom.xml, as shown in below snapshot:

Congratulations! you’ve successfully created your first Aspose Maven Project using **Aspose Maven Archetype** in NetBeans IDE.

### **Important Links:**

*   [Aspose for Java components][6]
*   [Aspose Maven Dependencies Integrate with IntelliJ IDEA][7]
*   [Aspose Maven for JetBrains][8]
*   [Aspose Cloud Maven Repository][9]
*   [Aspose Maven JavaDocs Integration][10]




[1]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-java-for-maven/1.0/
[4]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-java-for-maven/1.0/
[5]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-java-for-maven/1.0/
[6]: https://products.aspose.com/total/java
[7]: https://blog.aspose.com/2014/10/03/aspose-maven-dependencies-integrates-with-jetbrains-ide/
[8]: https://blog.aspose.com/2014/11/26/aspose-maven-for-jetbrains-new-plugin-released/
[9]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[10]: https://blog.aspose.com/2014/12/24/aspose-java-apis-javadocs-now-available-within-maven-based-projects/




