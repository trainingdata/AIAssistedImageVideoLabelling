---
title: "2D Growth Tool for DICOM"
excerpt: ""
---
2D growth tool ONLY works for DICOM (radiology) files
2D growth tool grows region based on HU value and pixel-distance
[block:api-header]
{
  "title": "Configuration"
}
[/block]
Configure: **Growth range in HU**
Configure: **Distance in Pixel**
If you enter -30 to 30 HU with 10 pixel radius, when you click on a pixel, growth tool will select all pixels within 10 pixel radius, that have HU value in -30 to +30 range with relative to HU value of selected pixel. If HU value of selected pixel is 450, all pixels within 10 pixel radius in 420 - 480 HU values, will be selected.
[block:api-header]
{
  "title": "Video"
}
[/block]

[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3D-LV3co2EFtM&src=https%3A%2F%2Fwww.youtube.com%2Fembed%2F-LV3co2EFtM%3Ffeature%3Doembed&type=text%2Fhtml&key=f2aa6fc3595946d0afc3d76cbbd25dc3&schema=youtube\" width=\"640\" height=\"480\" scrolling=\"no\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=-LV3co2EFtM&feature=youtu.be",
  "title": "2DGrowthExample",
  "favicon": "https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico"
}
[/block]

[block:api-header]
{
  "title": "Accuracy"
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/7194b7c-HighAccuracyRadiology.gif",
        "HighAccuracyRadiology.gif",
        664,
        338,
        "#808382"
      ],
      "caption": "Accuracy of 3D Growth compared to Desktop Tools"
    }
  ]
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/baa1179-HighPrecision.png",
        "HighPrecision.png",
        1552,
        784,
        "#8c8c8d"
      ],
      "caption": "Comparison"
    }
  ]
}
[/block]