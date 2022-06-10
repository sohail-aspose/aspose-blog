---
title: 'OOXML Charts Rendering and Right-to-Left Mail Merge in .NET and Java'
date: Tue, 09 Oct 2012 12:13:13 +0000
draft: false
url: /2012/10/09/ooxml-charts-rendering-control-over-external-resources-and-right-to-left-mail-merge-support-included-in-aspose.words-11.8.0/
author: Adam Skelton
summary: ''
tags: ['External Resource', 'Network', 'OOXML', 'RTL', 'Supported Features', 'URL', 'charts', 'mail merge']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="">}}


We have just released this month’s improvements to Aspose.Words for .NET and Java. This month’s release includes 150 improvements to many areas of our component and includes many new exciting features which are explained in detail below.

You can immediately download our latest Aspose.Words release from the following links:

*   [Aspose.Words for .NET 11.8.0][1]
*   [Aspose.Words for Java 11.8.0][2]

## List of Public API Changes with Each Release

In order to make it easier to keep up with any changes to the public API we have begun publishing a list of changes with the release of Aspose.Words. Check out the list for this month’s release in the documentation:

*   [Public API Changes in Aspose.Words for .NET 11.8.0][3]
*   [Public API Changes in Aspose.Words for Java 11.8.0][4]

You can use this handy guide to check for new, deprecated or removed members from the public API, as well as any changes to the internal workings of Aspose.Words that might affect your existing code.

Such documentation will become a standard procedure and will accompany all future releases of Aspose.Words.

## Rendering of OOXML Charts is now Supported

Office Open XML (OOXML) is the name given to the XML based format used to represent documents produced by the latest versions of Microsoft Word. Such documents can contain charts that are also described in XML format; these are called “OOXML Charts”.

Starting with Aspose.Words 11.8.0 rendering of these charts has become available. This is the first iteration of chart rendering and most of the general features are implemented. The full list of supported and unsupported features can found in the documentation.

*   [OOXML Chart Rendering Supported Features for .NET][5]
*   [OOXML Chart Rendering Supported Features for Java][6]

## Full Control Over How External Resources are Handled

Often a document can contain a link to an external resource, such as an image hosted on a network or on the internet. Such resources are downloaded automatically when required by Aspose.Words.

You may wish to intercept these calls to download external resources to either stop them or provide your own logic. In previous versions of Aspose.Words, you could achieve this  by using the **IResourceLoadingCallback** but this would only work when loading an HTML Document.

Starting with this release of Aspose.Words this callback has been fully extended this to work for all load formats as well as for cases when external data is downloaded by Aspose.Words.  Now you can use the **IResourceLoadingCallback** callback in almost any situation to customize control over external resources being downloaded. For instance you may wish to use this callback when:

*   Some external resources requires authentication in order to download them.
*   When you want to substitute a local image instead of downloading the resource.
*   When you want your application to avoid downloading any external resources at all.

In addition to when a document is loaded, these are some of the instances where the **IResourceLoadingCallback** callback can be used:

<figure class="wp-block-table"><table class=""><tbody><tr><td>**Scenario</strong></td><td><strong>Comments</strong></td></tr><tr><td><strong><em>DocumentBuilder.InsertImage</em></strong></td><td>This method allows you to pass a URL to insert an image from an external address. If the image is stored on a private network it may require authentication in order to load. The <strong>ResourceLoadingCallback</strong> can be used to pass the needed credentials</td></tr><tr><td><strong><em>DocumentBuilder.InsertHtml</em></strong></td><td>This method parses an HTML snippet into the document at the current cursor. As with <strong>DocumentBuilder.InsertImage</strong> this snippet can contain links to external resources.</td></tr><tr><td><strong><em>ImageData.SetImage</em></strong></td><td>Use a <strong>ResourceLoadingCallback</strong> to allow inserting images from a Base64 string source.</td></tr><tr><td><strong><em>ImageData.ToStream</em></strong></td><td>If the user requests a linked image to be converted to stream then it is downloaded from the external source and returned to the user. Add a callback here to control how this download occurs.</td></tr><tr><td><strong><em>Export to fixed paged formats (PDF, image etc)</em></strong></td><td>If an image is linked and not stored in the document, it is retrieved during conversion so it can be present in the rendered output. In some situations you may wish to skip this happening in order to speed up conversion times.</td></tr><tr><td><strong><em>Update of INCLUDEPICTURE fields</em></strong></td><td>When this field is preserved in the document object model by using the <strong>LoadOptions.PreserveIncludePictureField** property, this field can be linked to an external path and updating fields could cause loading of external data.</td></tr></tbody></table></figure>

Below are code examples of how to achieve the two most common use cases.

### Insert an Image that requires Authentication```
Document doc = new Document();
DocumentBuilder builder = new DocumentBuilder(doc);

// Create the resource loading handler which downloads images that require authentication.
doc.ResourceLoadingCallback = new InsertImageWithCredentialsHandler();

// It is expected that the images reference in this HTML snippet requires authorization.
// Note that supplied address here is just an example and does not actually exist.
builder.InsertHtml(@"<p style='margin:0pt'><span style='font-family:Calibri; font-size:11pt'>Test Html document.</span>
<p style='margin:0pt'><img src='https://www.aspose.com/download/auto.jpg' alt='Test.png' />");


public class InsertImageWithCredentialsHandler : IResourceLoadingCallback
{
   public InsertImageWithCredentialsHandler()
   {
      mWebClient = new WebClient();
   }

   public ResourceLoadingAction ResourceLoading(ResourceLoadingArgs args)
   {
      if (args.ResourceType == ResourceType.Image)
      {
          Uri uri = new Uri(args.Uri);

          // For NetworkCredentials to work it's assumed that the website implements a basic 401 authorization request.
          // You may wish to implement further logic here.
          if (uri.Host == "www.aspose.com")
              mWebClient.Credentials = new NetworkCredential("User1", "akjdlsfkjs");
          else
               mWebClient.Credentials = new NetworkCredential("SomeOtherUserID", "wiurlnlvs");

          // Supply the bytes from the location referenced by the URI.
          byte[] imageBytes = mWebClient.DownloadData(args.Uri);
          args.SetData(imageBytes);
          return ResourceLoadingAction.UserProvided;
      }
      else
      {
      return ResourceLoadingAction.Default;
      }
   }

   private WebClient mWebClient;
}
```

### Prevent Network Access with External Links```
LoadOptions loadOptions = new LoadOptions();
loadOptions.PreserveIncludePictureField = true;
loadOptions.ResourceLoadingCallback = new BanNetworkAccessHandler();

Document doc = new Document("DocumentWithIncludePicture.doc", loadOptions);
// Updating fields causes the IncludePicture link to attempt to download external data.
// The loading callback handler will prevent any external data from being downloaded.
doc.UpdateFields();


public class BanNetworkAccessHandler : IResourceLoadingCallback
{
   public ResourceLoadingAction ResourceLoading(ResourceLoadingArgs args)
   {
      // Skip any external resource from being downloaded.
      if (args.ResourceType == ResourceType.Image)
         return ResourceLoadingAction.Skip;

      return ResourceLoadingAction.Default;
   }
}
```

## Full Right-To-Left Language Support on Field Update

In previous versions of Aspose.Words there was no support for right-to-left languages during field update or mail merge which caused problems to customers who used right to left languages such as Arabic or Hebrew during mail merge.

Beginning in this release we have fully implemented right-to-left language support during field update and mail merge. We achieved this by analyzing more than 200 test cases of this behavior in Microsoft Word and implementing the same behavior in Aspose.Words in great detail.

Since there are extra steps involved in the process to properly merge right-to-left text we wanted to make sure backward compatibility and performance is maintained for those who do not use this feature. Therefore an option was implemented to toggle this functionality on or off.

To enable proper handling of right-to-left text during field update and mail merge you should set **Document.FieldOptions.IsBidiTextSupportedOnUpdate** to true in your code before performing field update or mail merge.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: https://blog.aspose.com/
[4]: http://blog.aspose.com
[5]: http://docs.aspose.com/display/wordsproductfamily
[6]: https://docs.aspose.com/display/wordsproductfamily/Home




