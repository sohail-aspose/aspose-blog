---
title: 'Render LaTeX Equations and Math Formulas using C#'
date: Tue, 08 Mar 2022 15:20:34 +0000
draft: false
url: /2022/03/08/render-latex-equations-and-math-formulas-using-csharp/
author: 'Muzammil Khan'
summary: 'You can write basic equations and mathematical formulas in the TEX file programmatically without using LaTeX. In this article, you will learn **how to render equations and math formulas using C#**.'
tags: ['C# API to Render LaTeX Math Formulas', 'Display Equations in C#', 'LaTeX Formulas in C#', 'LaTeX to PNG', 'Render Math Formulas in C#']
categories: ['Aspose.TeX Product Family']
---



{{< figure align=center src="images/render-equations-and-math-formulas-using-csharp.jpg" alt="Render Equations and Math Formulas using C#">}}


LaTeX is a powerful software to typeset math. It allows embedding formulas and mathematical equations in the [TEX](https://docs.fileformat.com/page-description-language/tex/) file, which is a source document prepared by LaTeX. It provides many commands to specify the format of the document, including text, symbols, mathematical expressions, and graphics. We can write basic equations and mathematical formulas programmatically without using LaTeX. In this article, we will learn **how to render LaTeX equations and math formulas using C#**.

The following topics shall be covered in this article:

*   [C# API to Render LaTeX Equations and Math Formulas](#CSharp-API-to-Render-Equations-and-Math-Formulas)
*   [Render LaTeX Inline Math Formulas](#Render-Inline-Math-Formulas-using-CSharp)
*   [Render Complex Equations](#Render-Complex-Equations-in-CSharp)
*   [Display Long Equations](#Display-Long-Equations-in-CSharp)
*   [Align Several Equations](#Align-Several-Equations-using-CSharp)
*   [Group and Center Equations](#Group-and-Center-Equations-using-CSharp)
*   [Render Matrices, Parenthesis, and Brackets](#Render-Matrices,-Parenthesis,-and-Brackets-in-CSharp)
*   [Render Fractions and Binomials](#Render-Fractions-and-Binomials-using-CSharp)

## C# API to Render LaTeX Equations and Math Formulas {#CSharp-API-to-Render-Equations-and-Math-Formulas}

For rendering LaTeX math formulas, we will be using the [Aspose.TeX for .NET](https://products.aspose.com/tex/net) API. It allows typesetting TeX files to different file formats like PDF, XPS, or images. Please either [download](https://downloads.aspose.com/tex/net) the DLL of the API or install it using [NuGet](https://www.nuget.org/packages/Aspose.TeX/).

```
PM> Install-Package Aspose.TeX
```

## Render LaTeX Inline Math Formulas using C# {#Render-Inline-Math-Formulas-using-CSharp}

We can render simple inline math formulas or equations by following the steps given below:

1.  Firstly, create an instance of the **_[MathRendererOptions](https://apireference.aspose.com/tex/net/aspose.tex.features/mathrendereroptions)_** class
2.  Next, specify the LaTeX document preamble.
3.  Optionally, set various properties such as _Scale, TextColor, BackgroundColor_, etc.
4.  After that, create the output stream for the formula image.
5.  Finally, call the **_[Render()](https://apireference.aspose.com/tex/net/aspose.tex.features/mathrenderer/methods/render)_** method to render the formula. It takes formula string, stream, MathRendererOptions, and the output image size as argument.

The following code sample demonstrates **how to render a math formula programmatically using C#**.

{{< gist aspose-com-gists a7c27e237ee752a9e87592207aad51de "RenderEquationsMathFormulas_CSharp_Render.cs" >}}



{{< figure align=center src="images/Render-Inline-Math-Formulas-using-CSharp-1024x57.png" alt="Render Inline Math Formulas using C#" caption="Render Inline Math Formulas using C#">}}


## Render Complex Equations in C# {#Render-Complex-Equations-in-CSharp}

We can render any complex equations or formulas by following the steps mentioned earlier. However, we just need to provide the formula string at step # 4 as shown below:

```
MathRenderer.Render(@"\begin{equation*}
                e^x = x^{\color{red}0} + x^{\color{red}1} + 
                \frac{x^{\color{red}2}}{2} + 
                \frac{x^{\color{red}3}}{6} + 
                \cdots = \sum_{n\geq 0} \frac{x^{\color{red}n}}{n!}
                \end{equation*}", stream, options, out size);
```



{{< figure align=center src="images/Render-Complex-Equations-in-CSharp-1024x170.png" alt="Render Complex Equations in C#" caption="Render Complex Equations in C#">}}


## Display Long Equations in C# {#Display-Long-Equations-in-CSharp}

We can display long equations on multiple lines by following the steps mentioned earlier. However, we just need to provide the formula string at step # 4 as shown below:

```
MathRenderer.Render(@"\begin{document}
                    \begin{multline*}
	            p(x) = x^1+x^2+x^3+x^4\\ 
	            - x^4 - x^3 - x^2 - x
	            \end{multline*}
                    \end{document}", stream, options, out size);
```



{{< figure align=center src="images/Display-Long-Equations-1024x82.png" alt="Display-Long-Equations" caption="Display Long Equations in C#">}}


## Align Several Equations using C# {#Align-Several-Equations-using-CSharp}

We can also align and render several equations or formulas at once by following the steps mentioned earlier. However, we just need to provide the formula string at step # 4 as shown below:

```
MathRenderer.Render(@"\begin{document}
                         \begin{align*}
                         a+b   &  a-b   &  (a+b)(a-b)\\
                         x+y   &  x-y   &  (x+y)(x-y)\\
                         p+q   &  p-q   &  (p+q)(p-q)
                         \end{align*}
                         \end{document}", stream, options, out size);
```



{{< figure align=center src="images/Align-Several-Equations-using-CSharp-1024x220.png" alt="Align Several Equations using C#" caption="Align Several Equations using C#">}}


## Group and Center Equations using C# {#Group-and-Center-Equations-using-CSharp}

We can group and center multiple equations while rendering by following the steps mentioned earlier. However, we just need to provide the formula string at step # 4 as shown below:

```
MathRenderer.Render(@"\begin{gather*} 
                (a+b)=a^2+b^2+2ab \\ 
                (a-b)=a^2+b^2-2ab \\
                (a-b)=a^2+b^2-2ab
                \end{gather*}", stream, options, out size);
```



{{< figure align=center src="images/Group-and-Center-Equations-using-CSharp.png" alt="Group-and-Center-Equations-using-CSharp" caption="Group and Center Equations using C#">}}


## Render Matrices, Parenthesis, and Brackets in C# {#Render-Matrices,-Parenthesis,-and-Brackets-in-CSharp}

We can also render matrices, parenthesis, and brackets by following the steps mentioned earlier. However, we just need to provide the formula string at step # 4 as shown below:

```
MathRenderer.Render(@"\begin{document}
	            \[ 
	            \left \{
	              \begin{tabular}{ccc}
	              1 & 4 & 7 \\
	              2 & 5 & 8 \\
	              3 & 6 & 9 
	              \end{tabular}
	            \right \}
	            \]
	            \end{document}", stream, options, out size);
```



{{< figure align=center src="images/Render-Matrices-Parenthesis-and-Brackets-in-CSharp.png" alt="Render Matrices, Parenthesis, and Brackets in C#" caption="Render Matrices, Parenthesis, and Brackets in C#">}}


## Render Fractions and Binomials using C# {#Render-Fractions-and-Binomials-using-CSharp}

We can render fractions and binomials as well by following the steps mentioned earlier. However, we just need to provide the formula string at step # 4 as shown below:

```
MathRenderer.Render(@"\begin{document}
	            \[
	                \binom{n}{k} = \frac{n!}{k!(n-k)!}
	            \]
	            \end{document}", stream, options, out size);
```



{{< figure align=center src="images/Render-Fractions-and-Binomials-using-CSharp.png" alt="Render Fractions and Binomials using C#" caption="Render Fractions and Binomials using C#">}}


## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license](https://purchase.aspose.com/temporary-license) to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   render simple and complex mathematical formulas and equations in C#
*   align and group equations programmatically
*   render Matrices, Parenthesis, Brackets, Fractions, and Binomials

Besides, you can learn more about Aspose.TeX for .NET API using the [documentation](https://docs.aspose.com/tex/net/). In case of any ambiguity, please feel free to contact us on the [forum](https://forum.aspose.com/c/tex/47).

## See Also

*   [Convert TeX (LaTeX) to PDF or XPS File Programmatically using C#](https://blog.aspose.com/2021/04/13/convert-tex-latex-to-pdf-xps-csharp/)




