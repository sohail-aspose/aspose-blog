---
title: 'PCL to PDF, better TrueTypeFont, stable image to PDF conversion'
date: Mon, 19 Sep 2011 16:00:25 +0000
draft: false
url: /2011/09/19/pcl-to-pdf-better-truetypefont-stable-image-to-pdf-conversion/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Convert PCL to PDF', 'Convert PCL to PDF in Java', 'PCL to PDF', 'java', 'product release']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose.pdf-logo2.jpg" alt="PCL to PDF conversion">}}


The new version of Aspose.Pdf for Java 3.0.1 has been released. It provides with you the option to convert PCL files into PDF format. PCL (Printer Command Language) is a Hewlett-Packard printer language developed to access standard printer features. With this latest version of Aspose.Pdf you can convert these files into PDF format.

Here's a detailed description of supported commands by versions of the Aspose.Pfd for Java:

<figure class="wp-block-table"><table class=""><tbody><tr><td>**Sets of commands</strong></td><td><strong>Support</strong></td><td><strong>Exceptions**</td></tr><tr><td>Job control commands</td><td>2.8</td><td>Duplex printing mode.</td></tr><tr><td>Page control commands</td><td>2.8</td><td>Perforation Skip command.</td></tr><tr><td>Cursor Positioning Commands</td><td>2.8</td><td>Transparent Print Data Command.</td></tr><tr><td>Font selection commands</td><td>2.8</td><td>Embedded soft fonts. In current version instead of creating<br>soft font our library selects</td></tr><tr><td>suitable font from existing TrueType fonts.</td><td></td><td>Suitability is defined by width/height ratio.<br>User Defined Symbol Sets.</td></tr><tr><td>Raster graphics commands</td><td>2.8</td><td></td></tr><tr><td>Color commands</td><td>3.0.1</td><td></td></tr><tr><td>Print Model commands</td><td>3.0.1</td><td></td></tr><tr><td>Rectangle area fill commands</td><td>3.0.1</td><td></td></tr><tr><td>HP-GL/2 Vector Graphics commands</td><td>2.8</td><td>Screened Vector Command, Transparency Mode Command, Character Fill Mode Command,Transparent Data Command,<br>Extra Space Command, Scalable or Bitmap Fonts Command,</td></tr><tr><td>Character Slant Command, Rotate Coordinate System Command</td><td></td><td>Define variable Text Path Command is in beta version.</td></tr></tbody></table></figure>

In upcoming releases, we plan to include complete support for soft fonts.

As well as support for PCL files, this release also introduces the following improvements:

*   Converting medium and large XML files to PDF is now 5-10 times faster.
*   Added feature for setting DPI manually for headless systems by setting system property aspose.pdf.dpi.  
    For example:  
    java -Djava.awt.headless=true -Daspose.pdf.dpi=120 -cp aspose.pdf-3.0.1.jdk15.jar:. your.entry.Point

Please download and try using the latest release version from [Aspose.Pdf for Java 3.0.1][1].




[1]: https://docs.aspose.com/display/pdfjava/Home




