---
title: "On-Prem Datasets"
excerpt: ""
---
[block:api-header]
{
  "title": "What is a On-Prem dataset?"
}
[/block]
Local dataset is hosted in an internal network (intranet). It cannot be accessed anywhere on internet. It can be hosted using NAS (network  storage), or SAN (storage area network) 
[block:api-header]
{
  "title": "Supported Address Space for URLs"
}
[/block]
TrainingData.io application ONLY support following URL schemes:
1. HTTP: http://
2. HTTPS: https://
3. DICOM: dicomweb://

**NOT** supported:
1. FILE: file:///
[block:api-header]
{
  "title": "Do you support NAS or SAN?"
}
[/block]
TrainingData.io application supports both NAS (network attached storage) and SAN (storage area network).
[block:api-header]
{
  "title": "Do you prefer NAS over SAN?"
}
[/block]
TrainingData.io does NOT prefer one storage scheme over another. As long as the local storage is addressable by HTTP(S) URL scheme, our application can support any storage that supports HTTP(S) URL scheme.
[block:api-header]
{
  "title": "How can I host a local dataset?"
}
[/block]
This can be achieved in many different ways:
1. You can host a local dataset using any commercial grade NAS device.
2. You can use any of the open source media servers like Plex with [REST API interface](https://docs.google.com/document/d/19bTQr99oKn2pOpHcVtqidokbq9zup-K-mFy8JmII6uQ/edit?usp=sharing).

A comprehensive guide to hosting image files and video files can be found [here](https://www.theguardian.com/technology/askjack/2014/jul/31/how-do-i-set-up-a-media-server-to-share-photos-with-phones-and-tablets).

[block:api-header]
{
  "title": "How to manage local datasets in TrainingData.io application?"
}
[/block]
Local datasets can be created in two ways:
###1. Method One: Provide location to a folder containing image files:
While creating a new dataset select option "Local"
Enter a name for the new dataset. 
Select "Upload Folder" and select the folder that contains images. 
IMPORTANT: image paths will be processed recursively and images will *not* be uploaded to cloud.
[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FdPe4nCOB9Y4%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DdPe4nCOB9Y4&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2FdPe4nCOB9Y4%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"854\" height=\"480\" scrolling=\"no\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=dPe4nCOB9Y4&feature=youtu.be",
  "title": "Local - Edited",
  "favicon": "https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico",
  "image": "https://i.ytimg.com/vi/dPe4nCOB9Y4/hqdefault.jpg"
}
[/block]
###2. Method two: Upload a CSV file containing list of local urls:
Let's assume our name of our dataset is TCGA-CA-G4H2. This dataset has three folders: 
     1. Folder name "Drive" with jpeg files
     2. Folder name "PNG" with png files
     3. Folder name "DICOM" with Dicom files
Arrange folder names and file URLs in following format csv format:
[block:html]
{
  "html": "<iframe width='100%' height='250'  src=\"https://docs.google.com/spreadsheets/d/e/2PACX-1vS0sq3VtQGLMokOyrEuh6sDEnVAkZJeBzFvzsriNSqWZByjFJOgHFp0luJfWEPGqjQYhwOVPhEGo8vk/pubhtml?gid=14120895&amp;single=true&amp;widget=true&amp;headers=false\"></iframe>"
}
[/block]
Upload this csv file while creating a new data set as shown in video below:
[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3D4rKX_mBwUjM&src=https%3A%2F%2Fwww.youtube.com%2Fembed%2F4rKX_mBwUjM%3Ffeature%3Doembed&type=text%2Fhtml&key=f2aa6fc3595946d0afc3d76cbbd25dc3&schema=youtube\" width=\"640\" height=\"480\" scrolling=\"no\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=4rKX_mBwUjM&feature=youtu.be",
  "title": "CSV Upload for Local Dataset",
  "favicon": "https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico"
}
[/block]

[block:api-header]
{
  "title": "What is recommended directory structure?"
}
[/block]
It is recommended that only one folder is uploaded in a dataset. TrainingData.io application supports multiple recursive folders under a select folder. 

Web Server's root directory MUST BE parent directory of selected folder.

### Sample directory structure:
imageserver/
├── radiology
│   └── TCGA-CA-G4H2
│       ├── DICOM
│       │   ├── 000045.dcm
│       │   ├── 000046.dcm
│       │   ├── 000047.dcm
│       │   ├── 000048.dcm
│       │   ├── 000049.dcm
│       │   └── 000050.dcm
│       ├── Drive
│       │   ├── av001.jpg
│       │   ├── av002.jpg
│       │   ├── av003.jpg
│       │   ├── av004.jpg
│       │   └── av005.jpg
│       └── test
│           └── test1
│               ├── av001.jpg
│               ├── av002.jpg
│               └── PNG
│                   ├── 00012.jpg
│                   ├── 00013.jpg
│                   ├── 00014.jpg
│                   ├── 00015.jpg
│                   └── 00016.jpg

7 directories, 19 files