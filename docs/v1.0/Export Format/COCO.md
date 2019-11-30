# COCO Export Format

[COCO data format](http://cocodataset.org/#format-data) uses JSON to store annotations. It has five types of annotations: object detection, keypoint detection, stuff segmentation, panoptic segmentation, and image captioning. Basic higher level data format looks like this:
```
{
  "info" : info, 
  "images" : [image], 
  "annotations" : [annotation], 
  "licenses" : [license],
}

info: {
  "year" : int, 
  "version" : str, 
  "description" : str, 
  "contributor" : str, 
  "url" : str, 
  "date_created" : datetime,
}

image: {
  "id" : int, 
  "width" : int, 
  "height" : int, 
  "file_name" : str, 
  "license" : int, 
  "flickr_url" : str, 
  "coco_url" : str, 
  "date_captured" : datetime,
}

license: {
  "id" : int, 
  "name" : str, 
  "url" : str,
}
```
## Sample COCO Format File
```
{
	"images": [{
		"coco_url": "",
		"date_captured": "",
		"file_name": "000045.dcm",
		"flickr_url": "",
		"id": "dicomweb://localhost:8000/radiology/TCGA-CA-G4H2/DICOM/000045.dcm",
		"license": 0,
		"height": 512,
		"width": 512
	}],
	"categories": [],
	"licenses": [],
	"info": {},
	"attributes": [],
	"annotations": [{
		"segmentation": [175.16666666666669, 174.1684027777778, 151.27777777777783, 200.83506944444446, 185.72222222222226, 215.2795138888889],
		"annotations": [],
		"image_id": "dicomweb://localhost:8000/radiology/TCGA-CA-G4H2/DICOM/000045.dcm",
		"iscrowd": 0,
		"id": "163b7530-acd2-4937-b529-27166f56b305",
		"category_id": "polygon"
	}, {
		"segmentation": [202.18712029161605, 166.5030376670717, 217.11786148238156, 204.45200486026732, 254.4447144592953, 198.23086269744837, 242.00243013365736, 155.92709599027947],
		"annotations": [],
		"image_id": "dicomweb://localhost:8000/radiology/TCGA-CA-G4H2/DICOM/000045.dcm",
		"iscrowd": 0,
		"id": "163b7530-acd2-4937-b529-27166f56b305",
		"category_id": "polygon"
	}, {
		"segmentation": [138.5, 253.140625, 200.5, 253.140625, 200.5, 285.140625, 138.5, 285.140625],
		"annotations": [],
		"image_id": "dicomweb://localhost:8000/radiology/TCGA-CA-G4H2/DICOM/000045.dcm",
		"iscrowd": 0,
		"id": "041b692e-11d6-4266-8bf6-1ae972de3c83",
		"category_id": "Car"
	}, {
		"segmentation": [252.5, 239.140625, 302.5, 239.140625, 302.5, 277.140625, 252.5, 277.140625],
		"annotations": [],
		"image_id": "dicomweb://localhost:8000/radiology/TCGA-CA-G4H2/DICOM/000045.dcm",
		"iscrowd": 0,
		"id": "041b692e-11d6-4266-8bf6-1ae972de3c83",
		"category_id": "Car"
	}, {
		"segmentation": [317.5, 157.140625, 317.5, 156.140625, 313.5, 156.140625, 307.5, 156.140625, 303.5, 156.140625, 297.5, 157.140625, 294.5, 158.140625, 289.5, 161.140625, 287.5, 162.140625, 285.5, 165.140625, 284.5, 167.140625, 283.5, 170.140625, 283.5, 172.140625, 284.5, 176.140625, 285.5, 179.140625, 290.5, 184.140625, 304.5, 192.140625, 312.5, 194.140625, 323.5, 196.140625, 333.5, 196.140625, 342.5, 193.140625],
		"annotations": [],
		"image_id": "dicomweb://localhost:8000/radiology/TCGA-CA-G4H2/DICOM/000045.dcm",
		"iscrowd": 0,
		"id": "041877cb-2371-49e3-b21f-c9960ef4c9af",
		"category_id": "freehan"
	}, {
		"segmentation": [360.5, 159.140625, 359.5, 160.140625, 350.5, 164.140625, 346.5, 169.140625, 345.5, 175.140625, 345.5, 181.140625, 348.5, 187.140625, 354.5, 191.140625, 360.5, 194.140625, 367.5, 196.140625, 374.5, 197.140625, 382.5, 198.140625, 390.5, 197.140625, 399.5, 195.140625, 407.5, 191.140625, 411.5, 189.140625],
		"annotations": [],
		"image_id": "dicomweb://localhost:8000/radiology/TCGA-CA-G4H2/DICOM/000045.dcm",
		"iscrowd": 0,
		"id": "041877cb-2371-49e3-b21f-c9960ef4c9af",
		"category_id": "freehan"
	}, {
		"value": "c1",
		"name": "Image size",
		"image_id": "dicomweb://localhost:8000/radiology/TCGA-CA-G4H2/DICOM/000045.dcm"
	}, {
		"value": "r1",
		"name": "Image color",
		"image_id": "dicomweb://localhost:8000/radiology/TCGA-CA-G4H2/DICOM/000045.dcm"
	}, {
		"value": "o1",
		"name": "opacity",
		"image_id": "dicomweb://localhost:8000/radiology/TCGA-CA-G4H2/DICOM/000045.dcm"
	}, {
		"value": "",
		"name": "clarity",
		"image_id": "dicomweb://localhost:8000/radiology/TCGA-CA-G4H2/DICOM/000045.dcm"
	}]
}
```
[Mask File for COCO File above](..\..\assets\images\000045.png)

```
## Object Detection
```
annotation{
  "id" : int, 
  "image_id" : int, 
  "category_id" : int, 
  "segmentation" : RLE or [polygon], 
  "area" : float, 
  "bbox" : [x,y,width,height], 
  "iscrowd" : 0 or 1,
}

categories[{
  "id" : int, 
  "name" : str, 
  "supercategory" : str,
}]
```
## Keypoint Detection
```
annotation{
  "keypoints" : [x1,y1,v1,...], 
  "num_keypoints" : int, 
  "[cloned]" : ...,
}

categories[{
  "keypoints" : [str], 
  "skeleton" : [edge], 
  "[cloned]" : ...,
}]

"[cloned]": denotes fields copied from object detection annotations defined above.
```
