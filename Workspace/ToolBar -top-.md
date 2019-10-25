---
title: "ToolBar (top)"
excerpt: ""
---
Toolbar on the top has four sections.

**Section One and Two: Image Placement**
Following features allow easy accessibility of different sections of the image: Zoom in, Zoom out, Pan
Following features allow you to pixel level detail of the image. In case of PNG or Jpeg you can see RGB values at each pixel, in case of DICOM image format you can see HU value.


**Section Three: Annotation Tools**
Draw tool allows free hand drawing as shown in image below
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/19a0433-DrawTool.gif",
        "DrawTool.gif",
        639,
        370,
        "#8b8e8b"
      ],
      "caption": "Draw Tool"
    }
  ]
}
[/block]
Rectangle tool can be used to create **bounding box** annotations.
[block:api-header]
{
  "title": "Freehand Drawing Tool"
}
[/block]
**Freehand Tool** can be used to create freehand annotations as shown in figure below
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/03563da-FreeHand_Tool.gif",
        "FreeHand Tool.gif",
        943,
        537,
        "#a3a6a5"
      ],
      "caption": "Freehand Tool"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Segmentation Tool"
}
[/block]
 
**Pixel Level Accuracy**
**PNG and JPEG**: Segmentation tool provides superpixel segmentation based on color. Segmentation tool works for JPG and PNG image formats.
https://youtu.be/l8XL_b4SIyk
[block:html]
{
  "html": "<iframe width=\"560\" height=\"315\" src=\"https://www.youtube.com/embed/l8XL_b4SIyk\" frameborder=\"0\" allow=\"accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture\" allowfullscreen></iframe>"
}
[/block]

[block:embed]
{}
[/block]

[block:api-header]
{
  "title": "3D Growth Tool"
}
[/block]
For **DICOM** format: 2D growth and 3D growth works based on HU value (Hounsfield Unit). It grows the region based on HU value within a specified pixel-radius. Video below shows how to create pixel-accurate annotations at very fast pace.
https://youtu.be/EkKbQQctLfA
[block:html]
{
  "html": "<iframe width=\"560\" height=\"315\" src=\"https://www.youtube.com/embed/EkKbQQctLfA\" frameborder=\"0\" allow=\"accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture\" allowfullscreen></iframe>"
}
[/block]
**Section Four: Window Level**
Contrast: Set contrast of image
Brightness: Set brightness in the image
Window level: Select one of the following presets: Abdominal soft tissue, Bone, Brain, Brain Marrow, Liver, Lung, Subdural Brain

**Section Five: Layouts**
TrianingData.io workspace allows upto 4 folders to be viewed at the same time. In "Layout" menu options user can select 1x2, 2x1 or 2x2 mode to view upto 4 folders in same viewport. This allows for easy comparison of images.

**Stack Scroll**
For DICOM image format if more than one folder is in viewport, stack scroll will be automatically enabled as shown in image below 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/8e61c3a-StackScroll.png",
        "StackScroll.png",
        1364,
        937,
        "#5d5e5e"
      ],
      "caption": "Stack Scroll"
    }
  ]
}
[/block]