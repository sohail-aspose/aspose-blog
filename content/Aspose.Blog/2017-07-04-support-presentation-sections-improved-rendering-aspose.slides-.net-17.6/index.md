---
title: 'Support for Presentation Sections in Aspose.Slides for .NET 17.6'
date: Tue, 04 Jul 2017 16:05:58 +0000
draft: false
url: /2017/07/04/support-presentation-sections-improved-rendering-aspose.slides-.net-17.6/
author: Adnan Ahmad
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/aspose-Slides-for-net_100.png" alt="">}}


We like to share the release announcement for Aspose.Slides for .NET 17.6. We have added some new features related to adding sections inside the presentation and improved rendering options.

## New Features

We have included the support for managing sections inside the presentation to hold a group of slides for providing better organization of slides. Please visit documentation article, Adding or Removing Sections for further details. We have also improved the presentation rendering by the addition of an option to include slide comments inside exported HTML, PDF, SWF, TIFF, and XPS. Please visit documentation articles, [Converting Presentation to HTML][1], and [Converting Presentation to SWF][2] for example codes.

## Resolved Issues

The following issues have been resolved in this release.

*   Allow Latin text to wrap in the middle of the word ISSUE.
*   Right-To-Left\\Left-To-Right text direction issues.
*   Graphs get missing in exported PDF.
*   Tables are rendered incorrectly in the saved presentations.
*   Bullet numbering did not reset for text in exported PDF.
*   Exception when instantiating presentation with the signed file.
*   Presentation protection does not work if saved as PPT.
*   The font substation does not work for bullets and symbols.
*   Application hangs when converting a slide to SVG.
*   Bullet/Text offset lost on saving presentation.
*   Shape.TextFrame returns null for Title shape.
*   Cannot access the presentation properties for Aspose.Slides unprotected presentation using Filtdump.exe.
*   Ability to convert read-only PPT to PDF no longer works.
*   Comments Count issue for PPT file.
*   Slide comments are not read for PPT files.
*   The text is missing in the generated PPT file.
*   The wrong exception message is thrown on loading password-protected presentation without the password.
*   Text is improperly rendered in generated PDF.
*   Symbols' orientation changed on presentation load and saved.
*   Applying password to PPTX removes custom properties.
*   Zoom level changed, Notes box appeared on load and save.
*   PPTM to SVG not properly converted.
*   Hyperlink changes upon text changes.
*   Embedded excel Ole object once extracted corrupts the excel file.
*   Unsupported format exception on load the excel workbook from OLE Data.
*   Problem with GetEffectsByShape.
*   Text is improperly rendered in generated HTML.
*   InvalidCastException on converting ODP to PDF.
*   LastSavedTime on PPT files doesn't work.
*   Presentation date property converted by default.
*   Bullet numbering gets changed in generated HTML.
*   Text strings are improperly aligned in the saved presentations.
*   Text position getting changed in saved PPT.
*   Actions on animations are lost on saving presentation.
*   Invert if the negative property in PPTX being set.
*   Exception on loading presentation.
*   Text overlapping in generated image result.
*   The hyperlink is wrongly associated with text in exported HTML.
*   Drop Shadow effects are lost when saving a presentation.
*   Text formatting changes after cloning.
*   Bar chart not properly rendered after cloning.
*   Chart styles are not getting applied to saved presentations.
*   NullReference exception is thrown on WriteWorkbookStream for the chart.

We have made several enhancements to the new API. Please refer to [Aspose.Slides for .NET 17.6 Release Notes][3] for further reference.

To download Aspose.Slides for .NET 17.6, [please visit the download page][4].




[1]: https://docs.aspose.com/display/slidesnet/Converting+a+Presentation#ConvertingaPresentation-ConvertingWholePresentationtoHTML
[2]: https://docs.aspose.com/display/slidesnet/Converting+a+Presentation#ConvertingaPresentation-ConvertingPresentationtoSWF
[3]: https://docs.aspose.com/display/slidesnet/Aspose.Slides+for+.NET+17.6+Release+Notes
[4]: https://downloads.aspose.com/slides/net/




