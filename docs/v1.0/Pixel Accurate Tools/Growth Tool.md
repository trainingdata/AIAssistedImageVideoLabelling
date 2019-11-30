# 2D Growth Tool for DICOM
2D growth tool ONLY works for DICOM (radiology) files
2D growth tool grows region based on HU value and pixel-distance

## Configuration

Configure: **Growth range in HU**
Configure: **Distance in Pixel**
If you enter -30 to 30 HU with 10 pixel radius, when you click on a pixel, growth tool will select all pixels within 10 pixel radius, that have HU value in -30 to +30 range with relative to HU value of selected pixel. If HU value of selected pixel is 450, all pixels within 10 pixel radius in 420 - 480 HU values, will be selected.

## Video



<!-- [![2DGrowthExample](https://i.ytimg.com/vi/-LV3co2EFtM/hqdefault.jpg)](https://www.youtube.com/watch?v=-LV3co2EFtM&feature=youtu.be) -->

<div class="video-wrapper">
  <iframe width="1280" height="480" src="https://www.youtube.com/embed/-LV3co2EFtM" frameborder="0" allowfullscreen></iframe>
</div>


## Accuracy



![Accuracy of 3D Growth compared to Desktop Tools](/assets/images/7194b7c-HighAccuracyRadiology.gif)



![Comparison](/assets/images/baa1179-HighPrecision.png)
