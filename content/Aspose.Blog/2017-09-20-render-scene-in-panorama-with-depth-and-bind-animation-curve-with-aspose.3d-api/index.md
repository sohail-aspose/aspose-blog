---
title: 'Render Scene in Panorama with Depth and Bind Animation Curve using C#'
date: Wed, 20 Sep 2017 20:34:27 +0000
draft: false
url: /2017/09/20/render-scene-in-panorama-with-depth-and-bind-animation-curve-with-aspose.3d-api/
author: Imran Rafique
summary: ''
tags: []
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for .NET logo">}}


We are pleased to announce the availability of [new version 17.9 of Aspose.3D for .NET API][1]. The new version 17.9 of the API has been released with the support of rendering 3D scenes in Panorama mode with depth and also enhanced the way of binding the animation curve. We have enhanced the API usage by incorporating new features, enhancements and regular bug fixes.

## Render 3D Scene in Panorama Mode with Depth

With the help of Aspose.3D for .NET API, developers can render 3D scenes in Panorama mode with depth. In order to achieve this, developers can define a vertex shader with custom script. In following help topic, we have created a camera, two light objects, define vertex shader and define position to render the depth map: [Render 3D Scene with Panorama Mode in Depth][2]

## Bind Animation Curve to the Specified Channel

The BindCurve member of the CurveMapping class allows to create the curve on the component of the animation property. In the past versions, we were using Curve class to do this and now we have enhanced the way of the binding curve to the specified channel.

**Before the version 17.9 to create animation manually, we use:**

```
//create a curve mapping on cube node's transform object, the curve manipulates the property 'Scale'var scale = anode.CreateCurveMapping(cube1.Transform, "Scale");// Create the animation curve on Y component of the scale Curve scaleYCurve = scale.CreateCurve("Y");//let cube1.Transform.Scale.Y to be 1.0f at 0th sec using bezier interpolationscaleYCurve.CreateKeyFrame(0, 1.0f, Interpolation.Bezier);//let cube1.Transform.Scale.Y to be 2.0f at 2th sec using bezier interpolationscaleYCurve.CreateKeyFrame(2, 2.0f, Interpolation.Bezier);//let cube1.Transform.Scale.Y to be 0.2f at 5th sec using linear interpolationscaleYCurve.CreateKeyFrame(5, 0.2f, Interpolation.Linear);//let cube1.Transform.Scale.Y to be 1.0f at 8th sec using bezier interpolationscaleYCurve.CreateKeyFrame(8, 1.0f, Interpolation.Bezier);
```

**In the recent version 17.9, we can implement the same task using the syntax sugar:**

```
//create a curve mapping on cube node's transform object, the curve manipulates the property 'Scale'var scale = anode.CreateCurveMapping(cube1.Transform, "Scale");// Create the animation curve on Y component of the scale scale.BindCurve("Y", new Curve(){ //let cube1.Transform.Scale.Y to be 1.0f at 0th sec using bezier interpolation {0, 1.0f, Interpolation.Bezier}, //let cube1.Transform.Scale.Y to be 2.0f at 2th sec using bezier interpolation {2, 2.0f, Interpolation.Bezier}, //let cube1.Transform.Scale.Y to be 0.2f at 5th sec using linear interpolation {5, 0.2f, Interpolation.Linear}, //let cube1.Transform.Scale.Y to be 1.0f at 8th sec using bezier interpolation {8, 1.0f, Interpolation.Bezier}});
```

The following help topic narrates how to add an animation property in a 3D scene: [Add Animation Property to 3D Scene Document][3]

## Public .NET 3D API Changes

The following API changes in the new version are also worth noticing:

*   CreateAnimationClip member to Aspose.ThreeD.Scene class has been added. It helps in creating animations.
*   CreateAnimationNode member to Aspose.ThreeD.Animation.AnimationClip class has been added. It helps in creating the animation node.
*   The two Add and one GetEnumerator members to Aspose.ThreeD.Animation.Curve class have been added. All these members help in creating key frames.
*   BindCurve member to Aspose.ThreeD.Animation.CurveMapping class has been added. This will bind the curve data on an existing channel in CurveMapping.
*   ShaderSet and PresetShaders members to Aspose.ThreeD.Render.Renderer class have been added. These members help to control the render effects.
*   Aspose.ThreeD.Render.PresetShaders class has been added. It defines the preset internal shaders used by the renderer.
*   Aspose.ThreeD.Render.ShaderSet class has been added. It helps in customizing the ShaderProgram used by each different materials to fully take control of the final render result.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][4]
*   [Download Aspose.3D for .NET][5]
*   [Aspose.3D product family forum][6] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][7] – help documentation and API reference documents.
*   [Aspose.3D for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [Install Aspose.3D NuGet package][9] - We publish each version of Aspose.3D for .NET API as a NuGet package on the NuGet gallery and recommend our clients upgrade old version to the latest one.
*   [Release Notes][10] - For details on API fixes, please check Release Notes having a complete list of the new features.

We hope you will enjoy this new release that save time and huge efforts for related files manipulation. The API is quite simple and can easily be used in any application.




[1]: https://downloads.aspose.com/3d/net/new-releases/aspose.3d-for-.net-17.9/
[2]: https://docs.aspose.com/3d/net/render-3d-scene-with-panorama-mode-in-depth/
[3]: https://docs.aspose.com/3d/net/add-animation-property-and-setup-target-camera-in-3d-document/#setup-the-target-camera-in-3d-file
[4]: https://products.aspose.com/3d/net/
[5]: http://downloads.aspose.com/3d/net
[6]: https://forum.aspose.com/c/3d
[7]: https://docs.aspose.com/3d/net/
[8]: https://github.com/aspose3D/Aspose_3d_NET
[9]: https://www.nuget.org/packages/Aspose.3d
[10]: https://docs.aspose.com/3d/net/aspose-3d-for-net-17-9-release-notes/




