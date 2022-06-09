---
title: 'Render LaTeX Math Formulas and Equations in Java'
seoTitle: "Render LaTeX Math Formulas and Equations in Java"
description: ""
date: Wed, 18 May 2022 06:46:04 +0000
draft: false
url: /2022/05/18/render-latex-math-formulas-and-equations-in-java/
author: Muzammil Khan
summary: 'As a Java programmer, you can write basic equations and mathematical formulas in the TEX file programmatically without using LaTeX. In this article, you will learn **how to render equations and math formulas using Java**.'
tags: ['Java API to Render LaTeX Math', 'LaTeX Formulas in Java', 'LaTeX Math Equation in Java', 'LaTeX Math Symbols in Java', 'LaTeX to PNG', 'LaTeX to SVG', 'Render LaTeX Math Formulas Java', 'Render Math Formulas in Java']
categories: ['Aspose.TeX Product Family']
---



{{< figure align=center src="images/render-latex-math-formulas-and-equations-in-java.jpg" alt="Render LaTeX Math Formulas and Equations in Java">}}


We can embed formulas and mathematical equations in the [TeX][1] file. LaTeX uses the TeX file as a source document that contains a set of commands. These commands specify the document's format, including text, symbols, mathematical expressions, and graphics. We can write and render any kind of equations and mathematical formulas programmatically without using LaTeX. In this article, will learn **how to render LaTeX math formulas and **equations**** **in Java**.

The following topics shall be covered in this article:

*   [Java API to Render LaTeX Math Formulas & Equations][2]
*   [Render LaTeX Math Formulas as PNG][3]
*   [Render Complex Equations][4]
*   [Display Long Equations][5]
*   [Align Several Equations][6]
*   [Group and Center Equations][7]
*   [Render Parenthesis and Brackets][8]
*   [Matrices in LaTeX][9]
*   [Render Fractions and Binomials][10]
*   [Mathematical Operators in LaTeX][11]
*   [Render LaTeX Math Formulas as SVG][12]

## Java API to Render LaTeX Math Formulas & Equations {#Java-API-to-Render-LaTeX-Math-Formulas-&-Equations}

For rendering LaTeX math formulas, we will be using the [Aspose.TeX for Java][13] API. It provides the _PngMathRendererOptions_ class for specifying the rendering options to save the Math formula as a [PNG][14]. Similarly, it also provides the _SvgMathRendererOptions_ class for specifying the rendering options to save the Math formula as an [SVG][15]. Moreover, for the rendering of math formulas, it provides _PngMathRenderer_ and _SvgMathRenderer_ classes derived from the _MathRenderer_ class. The [render()][16] method of this class renders the provided math formula. Furthermore, the API also allows typesetting TeX files to different file formats like [PDF][17], [XPS][18], or images.

Please either [download][19] the JAR of the API or add the following _**pom.xml**_ configuration in a Maven-based Java application.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-tex</artifactId>
    <version>22.4</version>
    <type>jar</type>
</dependency>
```

## Render LaTeX Math Formulas as PNG using Java {#Render-LaTeX-Math-Formulas-as-PNG-using-Java}

We can render simple inline math formulas or equations by following the steps given below:

1.  Firstly, create an instance of the **_[PngMathRendererOptions][20]_** class.
2.  Next, specify the image [resolutions][21], such as 150 DPI.
3.  Then, specify the LaTeX document preamble.
4.  Optionally, set various properties such as _Scale, TextColor, BackgroundColor_, etc.
5.  After that, create the output stream for the formula image.
6.  Finally, call the **_[render()][22]_** method to render the formula. It takes formula string, stream, rendering options, and the output image size as arguments.

The following code sample shows **how to render a math formula as a PNG programmatically using Java**.

{{< gist aspose-tex-gists c2c60da14dd442bd04933bdbf860d05f "Render-LaTeX-Math-Formulas-Java_RenderPNG.java" >}}



{{< figure align=center src="images/math-formula-1024x57.png" alt="Render LaTeX Math Formulas as PNG using Java." caption="Render LaTeX Math Formulas as PNG using Java">}}


## Render Complex Equations using Java {#Render-Complex-Equations-using-Java}

We can render any complex equations or formulas by following the steps mentioned earlier. However, we just need to set the formula string in step # 5 as shown below:

```
mathRenderer.render("\\begin{equation*}"
		+ "(1+x)^n = 1 + nx + \\frac{n(n-1)}{2!}x^{\\color{red}2}"
		+ "+ \\frac{n(n-1)(n-2)}{3!}x^{\\color{red}3}"
                + "+ \\frac{n(n-1)(n-2)(n-3)}{4!}x^{\\color{red}4}" 
                + "+ \\cdots"
                + "\\end{equation*}", stream, options, size);
```



{{< figure align=center src="images/Render-Complex-Equations-using-Java-1024x62.png" alt="Render Complex Equations using Java" caption="Render Complex Equations using Java">}}


## Display Long Equations using Java {#Display-Long-Equations-using-Java}

We can display long equations on multiple lines by following the steps mentioned earlier. However, we just need to set the formula string in step # 5 as shown below:

```
mathRenderer.render("\\begin{multline*}"
		+ "p(x) = 3x^6 + 14x^5y + 590x^4y^2 + 19x^3y^3\\\\"
		+ "- 12x^2y^4 - 12xy^5 + 2y^6 - a^3b^3"
		+ "\\end{multline*}", stream, options, size); 
```



{{< figure align=center src="images/Display-Long-Equations-using-Java-1024x85.png" alt="Display Long Equations using Java." caption="Display Long Equations using Java.">}}


## Align Several Equations using Java {#Align-Several-Equations-using-Java}

We can also align and render several equations or formulas at once by following the steps mentioned earlier. However, we just need to set the formula string in step # 5 as shown below:

```
mathRenderer.render("\\begin{align}"
		+ "f(u) & =\\sum_{j=1}^{n} x_jf(u_j)\\\\"
		+ "& =\\sum_{j=1}^{n} x_j \\sum_{i=1}^{m} a_{ij}v_i\\\\"
		+ "& =\\sum_{j=1}^{n} \\sum_{i=1}^{m} a_{ij}x_jv_i"
		+ "\\end{align}", stream, options, size);
```



{{< figure align=center src="images/Align-Several-Equations-using-Java-1024x455.png" alt="Align Several Equations using Java." caption="Align Several Equations using Java.">}}


## Group and Center Equations using Java {#Group-and-Center-Equations-using-Java}

We can group and center multiple equations while rendering by following the steps mentioned earlier. However, we just need to set the formula string in step # 5 as shown below:

```
mathRenderer.render("\\begin{gather*}"
		+ "2x - 5y =  8 \\\\"
		+ "3x^2 + 9y =  3a + c\\\\"
		+ "(a-b) = a^2 + b^2 -2ab"
		+ "\\end{gather*}", stream, options, size);
```



{{< figure align=center src="images/Group-and-Center-Equations-using-Java.png" alt="Group and Center Equations using Java." caption="Group and Center Equations using Java.">}}


## Render Parenthesis and Brackets using Java {#Render-Parenthesis-and-Brackets-using-Java}

We can also render parenthesis and brackets by following the steps mentioned earlier. However, we just need to set the formula string in step # 5 as shown below:

```
mathRenderer.render("\\begin{document}"
	     + "\\["
	     + " \\left[  \\frac{ N } { \\left( \\frac{L}{p} \\right)  - (m+n) }  \\right]"
	     + "\\]"
	     + "\\end{document}", stream, options, size);
```



{{< figure align=center src="images/Render-Parenthesis-and-Brackets-using-Java.png" alt="Render Parenthesis and Brackets using Java." caption="Render Parenthesis and Brackets using Java.">}}


## Matrices in LaTeX using Java {#Matrices-in-LaTeX-using-Java}

Similarly, we can render matrices by following the steps mentioned earlier. However, we just need to set the formula string in step # 5 as shown below:

```
mathRenderer.render("\\begin{document}"
	            + "\\["
	            + "\\left \\{"
	            + "\\begin{tabular}{ccc}"
	            + "  1 & 4 & 7 \\\\"
	            + "  2 & 5 & 8 \\\\"
	            + "  3 & 6 & 9 "
	            + "\\end{tabular}"
	            + "\\right \\}"
	            + "\\]"
	            + "\\end{document}", stream, options, size);
```



{{< figure align=center src="images/Matrices-in-LaTeX-using-Java.png" alt="Matrices in LaTeX using Java." caption="Matrices in LaTeX using Java.">}}


## Render Fractions and Binomials using Java {#Render-Fractions-and-Binomials-using-Java}

We can render fractions and binomials as well by following the steps mentioned earlier. However, we just need to set the formula string in step # 5 as shown below:

```
mathRenderer.render("\\begin{document}"
	            + "\\["
	            + "\\binom{n}{k} = \\frac{n!}{k!(n-k)!}"
	            + "\\]"
	            + "\\end{document}", stream, options, size);
```



{{< figure align=center src="images/Render-Fractions-and-Binomials-using-Java.png" alt="Render Fractions and Binomials using Java." caption="Render Fractions and Binomials using Java.">}}


## Mathematical Operators in LaTeX using Java {#Mathematical-Operators-in-LaTeX-using-Java}

The mathematical operator symbols represent various mathematical functions such as log, cos, sin, etc. We can render trigonometrical functions and logarithms in LaTeX by following the steps mentioned earlier. However, we just need to set the formula string in step # 5 as shown below:

```
mathRenderer.render("\\begin{document}"
	            + "\\["
	            + "\\sin(a + b) = \\sin a \\cos b + \\cos b \\sin a"
	            + "\\]"
	            + "\\end{document}", stream, options, size);
```



{{< figure align=center src="images/Mathematical-Operators-in-LaTeX-using-Java.png" alt="Mathematical Operators in LaTeX using Java." caption="Mathematical Operators in LaTeX using Java.">}}


## Render LaTeX Math Formulas in SVG using Java {#Render-LaTeX-Math-Formulas-in-SVG-using-Java}

We can also save the rendered math formulas or equations in SVG image format by following the steps given below:

1.  Firstly, create an instance of the **_[SvgMathRendererOptions][23]_** class.
2.  Next, specify the LaTeX document preamble.
3.  Optionally, set various properties such as _Scale, TextColor, BackgroundColor_, etc.
4.  After that, create the output stream for the formula image.
5.  Finally, call the **_[render()][24]_** method to render the formula. It takes formula string, stream, rendering options, and the output image size as arguments.

The following code sample shows **how to render a math formula in an SVG image using Java**.

{{< gist aspose-tex-gists c2c60da14dd442bd04933bdbf860d05f "Render-LaTeX-Math-Formulas-Java_RenderSVG.java" >}}



{{< figure align=center src="images/Render-LaTeX-Math-Formulas-in-SVG-using-Java-1024x337.jpg" alt="Render LaTeX Math Formulas in SVG using Java." caption="Render LaTeX Math Formulas in SVG using Java.">}}


## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][25] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   render simple and complex mathematical formulas and equations in Java;
*   align and group equations programmatically;
*   render Matrices, Parenthesis, Brackets, Fractions, and Binomials;
*   save the rendered formula images in PNG or SVG using Java.

Besides, you can learn more about Aspose.TeX for Java API using the [documentation][26]. In case of any ambiguity, please feel free to contact us on the [forum][27].

## See Also

*   [Create PDF from LaTeX in Java][28]
*   [Convert LaTeX TeX LTX to PNG JPG Image in Java][29]




[1]: https://docs.fileformat.com/page-description-language/tex/
[2]: #Java-API-to-Render-LaTeX-Math-Formulas-&-Equations
[3]: #Render-LaTeX-Math-Formulas-as-PNG-using-Java
[4]: #Render-Complex-Equations-using-Java
[5]: #Display-Long-Equations-using-Java
[6]: #Align-Several-Equations-using-Java
[7]: #Group-and-Center-Equations-using-Java
[8]: #Render-Parenthesis-and-Brackets-using-Java
[9]: #Matrices-in-LaTeX-using-Java
[10]: #Render-Fractions-and-Binomials-using-Java
[11]: #Mathematical-Operators-in-LaTeX-using-Java
[12]: #Render-LaTeX-Math-Formulas-in-SVG-using-Java
[13]: https://products.aspose.com/tex/java/
[14]: https://docs.fileformat.com/image/png/
[15]: https://docs.fileformat.com/page-description-language/svg/
[16]: https://apireference.aspose.com/tex/java/com.aspose.tex/MathRenderer#render-java.lang.String-java.io.OutputStream-com.aspose.tex.MathRendererOptions-com.aspose.tex.Size2D-
[17]: https://docs.fileformat.com/pdf/
[18]: https://docs.fileformat.com/page-description-language/xps/
[19]: https://downloads.aspose.com/tex/java
[20]: https://apireference.aspose.com/tex/java/com.aspose.tex/PngMathRendererOptions
[21]: https://apireference.aspose.com/tex/java/com.aspose.tex/PngMathRendererOptions#setResolution-int-
[22]: https://apireference.aspose.com/tex/java/com.aspose.tex/MathRenderer#render-java.lang.String-java.io.OutputStream-com.aspose.tex.MathRendererOptions-com.aspose.tex.Size2D-
[23]: https://apireference.aspose.com/tex/java/com.aspose.tex/SvgMathRendererOptions
[24]: https://apireference.aspose.com/tex/java/com.aspose.tex/MathRenderer#render-java.lang.String-java.io.OutputStream-com.aspose.tex.MathRendererOptions-com.aspose.tex.Size2D-
[25]: https://purchase.aspose.com/temporary-license
[26]: https://docs.aspose.com/tex/java/
[27]: https://forum.aspose.com/c/tex/47
[28]: https://blog.aspose.com/2022/04/07/create-pdf-from-latex-in-java/
[29]: https://blog.aspose.com/2021/11/28/convert-latex-to-png-or-jpg-image-in-java/




