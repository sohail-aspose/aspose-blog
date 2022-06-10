---
title: 'Signature Line and Improved Support for Math Content in Aspose.Words 11.3.0'
date: Thu, 03 May 2012 16:05:22 +0000
draft: false
url: /2012/05/03/signature-line-and-improved-support-for-math-content-in-aspose.words-11.3.0/
author: Adam Skelton
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words_logo.png" alt="">}}


We've managed to fit a lot of improvements into this month's release of Aspose.Words. The release of Aspose.Words 11.3.0 provides 127 fixes and new features. For a full list of features and fixes head over to the downloads page and download Aspose.Words 11.3.0:

*   [Aspose.Words for .NET 11.3.0][1]
*   [Aspose.Words for Java 11.3.0][2]

Here is a look at some of the biggest features in this month's release:

## Support for Signature Line

A signature line is a special object found in Microsoft Word documents in the drawing layer.  The signature line can be interacted with and provides an easy way for the end-user to add a digital signature to the document. This feature can be thought in the same way as how one would add a written signature to a printed document.



{{< figure align=center src="images/signature-line.jpg" alt="">}}


Starting with the release of Aspose.Words 10.3.0, signature lines are now supported in the model and this feature is retained when converting between flow formats such as DOCX, RTF, and WML with the exception of DOC format which will follow shortly.

At the moment signature lines are only partially rendered to fixed formats such as PDF with full support planned within a few releases.

## MathML in OpenOffice Format

MathML is the language used to describe mathematical and scientific equations in OpenOffice documents. Aspose.Words now supports import and export of MathML in ODT format and preserve almost all equations during round-trip.

Aspose.Words now boasts wide support for Math content in all types of Word documents. Nearly all types of math content are preserved during open and save using Aspose.Words. In this release we also have further improvements to math content in OOXML which is described next.

## OfficeMath Equations are now Preserved when Saving to Non-OOXML formats.

We are glad to announce that Aspose.Words now supports OfficeMath when saving to almost all formats.

OfficeMath is the main feature used to represent math equations in OOXML documents. Aspose.Words already supports round-trip of OfficeMath when loading and saving back to OOXML formats. However, in earlier versions this feature was lost if the target format did not natively support OfficeMath, for example OfficeMath disappear if the document was converted to DOC or HTML format.

Starting in Aspose.Words 11.3.0, we now mimic Microsoft Word’s behavior and convert OfficeMath to image when saving to any format that does not natively support it. This accurately preserves the appearance of this feature for all formats.

### OfficeMath Supported Features

This is the first version of OfficeMath rendering and we are proud to say that most features are supported. However, there are few limitations which we will be working to support in the next releases. Here is a detailed list of what features are supported or unsupported when rendering OfficeMath.

*   ‘Cambria Math’ font should be installed and accessible in order to properly render equations.
*   Vertical alignment of equation elements is not supported. Elements are always rendered as vertically centered.
*   Not all equation constructions are supported, below is the detailed list of supported elements:

<figure class="wp-block-table"><table class=""><tbody><tr><td>**OfficeMath Object Type</strong></td><td><strong>Level of Support**</td></tr><tr><td>OMath</td><td>Supported. Element is considered as a container for other equation elements.</td></tr><tr><td>OMathPara</td><td>Supported. Element is considered as a container for other equation elements.</td></tr><tr><td>Accent</td><td>Partially supported. Accent mark is not starched to the width of argument.</td></tr><tr><td>Bar</td><td>Supported.</td></tr><tr><td>BorderBox</td><td>Supported. Element is considered as a container for other equation elements with border around.</td></tr><tr><td>Box</td><td>Supported. Element is considered as a container for other equation elements.</td></tr><tr><td>Delimiter</td><td>Supported.</td></tr><tr><td>Degree</td><td>Degree is part of Radical. Supported.</td></tr><tr><td>Argument</td><td>Supported. Element is considered as a container for other equation elements.</td></tr><tr><td>Array</td><td>Array is one column Matrix. Supported.</td></tr><tr><td>Fraction</td><td>Partially supported. Only Bar type of Fraction is supported. Fraction is represented as an Array with two rows with Bar at the middle.</td></tr><tr><td>Denominator</td><td>Part of fraction. Supported.</td></tr><tr><td>Numerator</td><td>Part of fraction. Supported.</td></tr><tr><td>Function</td><td>Partially supported. Currently considered as a simple container, but probably we should add some more advance after function name.</td></tr><tr><td>FunctionName</td><td>Currently considered as a simple container.</td></tr><tr><td>GroupCharacter</td><td>Partially supported. Group character is not stretched to the width of argument.</td></tr><tr><td>Limit</td><td>Part of upper or lower limit. Supported.</td></tr><tr><td>LowerLimit</td><td>Supported.</td></tr><tr><td>UpperLimit</td><td>Supported.</td></tr><tr><td>Matrix</td><td>Partially supported. Row spacing and row spacing rule are not supported. Only single column spacing rule is supported.</td></tr><tr><td>MatrixRow</td><td>Part of Matrix. Supported.</td></tr><tr><td>Nary</td><td>Partially supported. Limits are always placed at the bottom and at the top of the operator.</td></tr><tr><td>Phantom</td><td>It seems is invisible, so no need to support it.</td></tr><tr><td>Radical</td><td>Supported.</td></tr><tr><td>SubscriptPart</td><td>Supported.</td></tr><tr><td>SuperscriptPart</td><td>Supported.</td></tr><tr><td>PreSubSuperscript</td><td>Supported.</td></tr><tr><td>Subscript,</td><td>Supported.</td></tr><tr><td>SubSuperscript,</td><td>Supported.</td></tr><tr><td>Supercript</td><td>Supported.</td></tr></tbody></table></figure>




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java




