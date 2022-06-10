---
title: 'Render Scene into the Cubemap, Create Panorama View and Fisheye Lens Effect in C#'
date: Mon, 21 Aug 2017 17:25:32 +0000
draft: false
url: /2017/08/21/render-scene-into-the-cubemap-create-panorama-view-and-fisheye-lens-effect-with-aspose.3d-for-.net-17.8/
author: Imran Rafique
summary: ''
tags: ['Create Fisheye lens effect', 'Create Panorama view', 'cubemap of 3D Scene']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for .NET logo">}}


We are pleased to announce the availability of [new version 17.8 of Aspose.3D for .NET API][1]. The new version 17.8 of the API has been released with the support of rendering a scene into the Cubemap with six faces and save all faces into the supported image format. Developers can create a Panorama view and render a Fisheye lens effect on the 3D scene, and then save that view into the supported image formats. We have enhanced the API usage by incorporating new features and regular bug fixes.

## Render 3D Scene into Cubemap in C#

With the help of Aspose.3D for .NET API, developers can load 3D models, create six square views in an order that all joined together to form a cube. These six views then form a cubemap which is used to make 3D background sceneries and fillers. Every rendering in 3D graphics has two elements, the scene, and the camera. The renderer then renders the scene relative to the camera. The following code sample shows how to render 3D Scene into Cubemap in C#.

```
string path = @"D:\Projects\glTF-Sample-Models\1.0\VC\glTF-Binary\VC.glb";
//load the scene
Scene scene = new Scene(path);
//create a camera for capturing the cube map
Camera cam = new Camera(ProjectionType.Perspective)
{
    NearPlane = 0.1,
    FarPlane = 200,
    RotationMode = RotationMode.FixedDirection
};
scene.RootNode.CreateChildNode(cam).Transform.Translation = new Vector3(5, 6, 0);
//create two lights to illuminate the scene
scene.RootNode.CreateChildNode(new Light() {LightType = LightType.Point}).Transform.Translation = new Vector3(-10, 7, -10);
scene.RootNode.CreateChildNode(new Light()
{
    Color = new Vector3(Color.CadetBlue)
}).Transform.Translation = new Vector3(49, 0, 49);
  
//create a renderer
using (var renderer = Renderer.CreateRenderer())
{
    //Create a cube map render target with depth texture, depth is required when rendering a scene.
    IRenderTexture rt = renderer.RenderFactory.CreateCubeRenderTexture(new RenderParameters(false), 512, 512);
    //a viewport is required on the render target
    rt.CreateViewport(cam, RelativeRectangle.FromScale(0, 0, 1, 1));
    renderer.Render(rt);
    //now lets get the cubemap texture
    ITextureCubemap cubemap = rt.Targets[0] as ITextureCubemap;
    //we can directly save each face to disk by specifing the file name
    CubeFaceData<string> fileNames = new CubeFaceData<string>()
    {
        Right = "right.png",
        Left = "left.png",
        Back = "back.png",
        Front = "front.png",
        Bottom = "bottom.png",
        Top = "top.png"
    };
    //and call Save method
    cubemap.Save(fileNames, ImageFormat.Png);
    //or we just need to use the render result in memory, we can save it to CubeFaceData<Bitmap>
    //CubeFaceData<Bitmap> bitmaps = new CubeFaceData<Bitmap>();
    //cubemap.Save(bitmaps);
    //bitmaps.Back.Save("back.bmp", ImageFormat.Bmp);
}
```

In the following help topic, we have created a Camera and two Light objects to capture the cubemap: [Render a scene into the cubemap with six faces][2]

## Render Panorama View of 3D Scene

A panorama is a wide-angle view that helps in taking a virtual tour of 3D scenes. With the help of Aspose.3D for .NET API, developers can create panoramas and save them into the supported image format. The following code sample shows how to render panorama view of 3D scene.

```
string path = @"D:\Projects\glTF-Sample-Models\1.0\VC\glTF-Binary\VC.glb";
//load the scene
Scene scene = new Scene(path);
//create a camera for capturing the cube map
Camera cam = new Camera(ProjectionType.Perspective)
{
    NearPlane = 0.1,
    FarPlane = 200,
    RotationMode = RotationMode.FixedDirection
};
scene.RootNode.CreateChildNode(cam).Transform.Translation = new Vector3(5, 6, 0);
  
//create two lights to illuminate the scene
scene.RootNode.CreateChildNode(new Light() {LightType = LightType.Point}).Transform.Translation = new Vector3(-10, 7, -10);
scene.RootNode.CreateChildNode(new Light()
{
    Color = new Vector3(Color.CadetBlue)
}).Transform.Translation = new Vector3(49, 0, 49);
//create a renderer
using (var renderer = Renderer.CreateRenderer())
{
    //Create a cube map render target with depth texture, depth is required when rendering a scene.
    IRenderTexture rt = renderer.RenderFactory.CreateCubeRenderTexture(new RenderParameters(false), 512, 512);
    //create a 2D texture render target with no depth texture used for image processing
    IRenderTexture final = renderer.RenderFactory.CreateRenderTexture(new RenderParameters(false, 32, 0, 0), 1024 * 3 , 1024);
  
    //a viewport is required on the render target
    rt.CreateViewport(cam, RelativeRectangle.FromScale(0, 0, 1, 1));
    renderer.Render(rt);
  
    //execute the equirectangular projection post-processing with the previous rendered cube map as input
    PostProcessing equirectangular = renderer.GetPostProcessing("equirectangular");
    //Specify the cube map rendered from the scene as this post processing's input
    equirectangular.Input = rt.Targets[0];
    //Execute the post processing effect and save the result to render target final
    renderer.Execute(equirectangular, final);
    //save the texture into disk
    ((ITexture2D)final.Targets[0]).Save("panorama.png", ImageFormat.Png);
}
```

The following help topic narrates how to create a spherical (equirectangular) panorama: [Render a Panorama view of 3D scene][3]

## Create a Fisheye Lens Effect on 3D Scene

A fisheye lens is an ultra wide-angle lens that produces strong visual distortion intended to create a wide panoramic image. With the help of Aspose.3D for .NET API, developers can create a fisheye lens effect on the 3D scene, and then save in the supported image format. The following help topic narrates how to create a fisheye lens effect, and then save in the image format: [Create a Fisheye lens effect on 3D scene and save in an image][4]

## Public .NET 3D API Changes

The following API changes in the new version are also worth noticing:

*   Load, Save and ToBitmap methods from ITextureUnit class have been obsoleted. 
*   Aspose.ThreeD.Render.CubeFace enum has been added. It helps to access data as per the face of the cubemap.
*   Aspose.ThreeD.Render.CubeFaceData class has been added. It describes cubemap data per face like file name or bitmap.
*   Aspose.ThreeD.Render.ITextureCubemap interface has been added. It retrieves the cubemap texture.
*   Aspose.ThreeD.Render.ITexture1D interface has been added. It represents a 1D texture object.
*   Aspose.ThreeD.Render.ITexture2D interface has been added. It represents a 2D texture object.
*   CreateRenderTexture, CreateCubeRenderTexture and CreateTextureUnit methods have been added to Aspose.ThreeD.Render.RenderFactory class. All these methods help in rendering textures.
*   Execute method to Aspose.ThreeD.Render.Renderer class has been added.
*   Normalize and Cross methods to Aspose.ThreeD.Utilities.FVector3 struct have been added. These are the two primitive operations of vectors.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][5]
*   [Download Aspose.3D for .NET][6]
*   [Aspose.3D product family forum][7] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   [Aspose.3D for .NET online documentation][8] – help documentation and API reference documents.
*   Enable Blog Subscription – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [Install Aspose.3D NuGet package][10] - We publish each version of Aspose.3D for .NET API as a NuGet package on the NuGet gallery and recommend our clients upgrade old version to the latest one.
*   [Release Notes][11] - For details on API fixes, please check Release Notes having a complete list of the new features.

We hope you will enjoy this new release that saves time and huge efforts for related file manipulation. The API is quite simple and can easily be used in any application.




[1]: https://downloads.aspose.com/3d/net/new-releases/aspose.3d-for-.net-17.8/
[2]: https://docs.aspose.com/display/3dnet/Render+a+scene+into+the+cubemap+with+six+faces
[3]: https://docs.aspose.com/display/3dnet/Render+a+Panorama+view+of+3D+scene
[4]: https://docs.aspose.com/display/3dnet/Create+a+Fisheye+lens+effect+on+3D+scene+and+save+in+an+image
[5]: https://products.aspose.com/3d/net
[6]: http://downloads.aspose.com/3d/net
[7]: https://forum.aspose.com/c/3d
[8]: https://docs.aspose.com/display/3dnet/Home
[9]: https://github.com/aspose3D/Aspose_3d_NET
[10]: https://www.nuget.org/packages/Aspose.3d
[11]: https://docs.aspose.com/display/3dnet/Aspose.3D+for+.NET+17.8+Release+Notes




