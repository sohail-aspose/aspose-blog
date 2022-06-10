---
title: 'Aspose Cloud Java SDK Integrates with Maven Projects'
date: Wed, 24 Sep 2014 10:37:26 +0000
draft: false
url: /2014/09/24/aspose-cloud-java-sdk-integrates-with-maven-projects/
author: Adeel Ilyas
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

## Aspose Cloud Java SDK's Maven Dependency

Aspose has released maven dependency for **Aspose Cloud Java SDK** **tagged as v1.0** supported by **[Aspose Cloud Maven Repository][1]**. Now using Aspose Cloud Java SDK in Maven projects has been quite straight forward by just defining **[Aspose Cloud Maven Respository][2]** url and Maven dependency Artifacts for Aspose Cloud Java SDK into pom.xml without any manual downloads and extra tricks.

To add Aspose Cloud Java SDK dependency in your maven project just follow the below steps:

1.  Need to first setup **[Aspose Cloud Maven Respository][3]** in your Maven project pom.xml by including repository url as below:
```
 <repositories>
    <repository>
        <id>AsposeJavaAPI</id>
        <name>Aspose Java API</name>
        <url>http://maven.aspose.com/artifactory/simple/ext-release-local/</url>
    </repository>
</repositories> 
```3.  And then define the following Maven Dependency into the pom.xml:
```
 <dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-cloud-sdk</artifactId>
    <version>1.0</version>
</dependency>
```

## Source Code Available

Source codes of mavenized - Aspose Cloud SDK for Java is available at the following branch of  GitHub repository:

 **![GitHub Mark icon2 Aspose API for Java Integration with Jetbrains IDE][4] GitHub**(revamp\_mavinized)




[1]: http://maven.aspose.com/artifactory/webapp/browserepo.html?6&pathId=ext-release-local:com/aspose/aspose-cloud-sdk/1.0/aspose-cloud-sdk-1.0.jar
[2]: http://maven.aspose.com/artifactory/webapp/home.html
[3]: http://maven.aspose.com/artifactory/webapp/home.html
[4]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/12/GitHub-Mark-icon2.png "GitHub-Mark-icon"




