---
# required metadata

title: Video player module
description: This topic covers video player modules and describes how to add them to site pages in Microsoft Dynamics 365 Commerce.
author: anupamar-ms
ms.date: 09/15/2020
ms.topic: article
ms.prod: 
ms.technology: 

# optional metadata

# ms.search.form: 
audience: Application user
# ms.devlang: 
ms.reviewer: v-chgri
# ms.tgt_pltfrm: 
ms.custom: 
ms.assetid: 
ms.search.region: Global
# ms.search.industry: 
ms.author: anupamar
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: Release 10.0.5

---

# Video player module

[!include [banner](includes/banner.md)]

This topic covers video player modules and describes how to add them to site pages in Microsoft Dynamics 365 Commerce.

The video player module is used to support video playback. It can be added to any page, provided that video content is uploaded to and available in the content management system (CMS). The video player module supports the .mp4 media type.

## Video player module

The video player module can be used to showcase videos on an e-Commerce site. It supports all playback capabilities, such as play, pause, full-size mode, audio descriptions, and closed captions. The video player module also supports customization of closed captions to meet Microsoft accessibility standards. For example, you can customize the font size and background color.

The video player module also supports secondary audio tracks. When a video is uploaded to the CMS, a secondary audio track can also be uploaded. The video player module can then play the secondary audio track if a user selects it.

### Examples of video player modules in e-Commerce

- Instructional videos on product details pages or marketing pages
- Promotional videos or videos about policies on any marketing page
- Marketing videos that highlight product features on product details pages or marketing pages

The following image shows an example of a video player module on a home page.

![Example of a video player module](./media/ecommerce-videoplayer.PNG)

### Video player module properties

| Property name         | Value                               | Description |
|-----------------------|-------------------------------------|-------------|
| Auto play             | **True** or **False**               | When the value is set to **True**, the video is automatically played. |
| Mute                  | **True** or **False**               | When the value is set to **True**, the audio is muted. For this player, the default value is **False**. In the Chrome browser, autoplay videos are muted by default, and the audio is played only if the user manually plays the video. |
| Loop                  | **True** or **False**               | When the value is set to **True**, the video is repeated in a loop. |
| Media                 | Video file path and name | The video file that is played in the video player. |
| Play fullscreen       | **True** or **False**               | When the value is set to **True**, the video is played in full-screen mode. |
| Play pause trigger    | **True** or **False**               | When the value is set to **True**, a play/pause button is shown on the video. |
| Video player controls | **True** or **False**               | When the value is set to **True**, all video player controls are shown. These controls include play and pause buttons, a progress indicator, and closed caption options. |
| Hide poster image     | **True** or **False**               | A video can have a poster frame. When the value of this property is set to **True**, the poster frame is hidden. |
| Mask level            | A number from **0** through **100** | The mask that is applied to the video for styling. |

## Add a video player module to a page

> [!NOTE] 
> Before you create a video player module, you must first upload a video to the Media Library.

To add a video player module to a new page and set the required properties, follow these steps.

1. Go to **Templates**, and select **New** to create a new template.
1. In the **New Template** dialog box, under **Template name**, enter **Video player template**, and then select **OK**.
1. In the **Body** slot, select the ellipsis (**...**), and then select **Add Module**.
1. In the **Add Module** dialog box, select the **Default Page** module, and then select **OK**.
1. In the **Main** slot of the **Default Page** module, select the ellipsis (**...**), and then select **Add Module**.
1. In the **Add Module** dialog box, select the **Container** module, and then select **OK**.
1. In the **Container** slot, select the ellipsis (**...**), and then select **Add Module**.
1. In the **Add Module** dialog box, select the **Video player** module, and then select **OK**.
1. Select **Save**, select **Finish editing** to check in the template, and then select **Publish** to publish it. 
1. Go to **Pages**, and select **New** to create a new page.
1. In the **Choose a template** dialog box, select the video player template that you created. Under **Page name**, enter **Video player page**, and then select **OK**.
1. In the **Main** slot of the new page, select the ellipsis (**...**), and then select **Add Module**.
1. In the **Add Module** dialog box, select the **Container** module, and then select **OK**.
1. In the **Container** slot, select the ellipsis (**...**), and then select **Add Module**.
1. In the **Add Module** dialog box, select the **Video player** module, and then select **OK**.
1. In the property pane of the video player module, select **Add a video**.
1. In the **Media Picker** dialog box, select a video, and then select **Upload new media item**.
1. In File Explorer, select a video file, and then select **Open**.
1. In the **Upload Media Item** dialog box, enter a title and other information as needed, and then select **OK**.
1. In the **Media Picker** dialog box, select **Close**.
1. Select **Save**, and then select **Preview** to preview the page. You should see the video module on the page. You can change additional settings to customize the behavior of the module.
1. Select **Finish editing** to check in the page, and then select **Publish** to publish it. 

## Additional resources

[Module library overview](starter-kit-overview.md)

[Promo banner module](add-alert.md)

[Carousel module](add-carousel.md)

[Text block module](add-content-rich-block.md)

[Content block module](add-hero-module.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]