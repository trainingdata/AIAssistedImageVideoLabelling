# On-Prem Datasets

## What is a On-Prem dataset?

Local dataset is hosted in an internal network (intranet). It cannot be accessed anywhere on internet. It can be hosted using NAS (network  storage), or SAN (storage area network)

## Supported Address Space for URLs

TrainingData.io application ONLY support following URL schemes:

1. HTTP: http://
2. HTTPS: https://
3. DICOM: dicomweb://

**NOT** supported:
1. FILE: file:///

## Do you support NAS or SAN?

TrainingData.io application supports both NAS (network attached storage) and SAN (storage area network).

## Do you prefer NAS over SAN?

TrainingData.io does NOT prefer one storage scheme over another. As long as the local storage is addressable by HTTP(S) URL scheme, our application can support any storage that supports HTTP(S) URL scheme.

## How can I host a local dataset?

This can be achieved in many different ways:

1. You can host a local dataset using any commercial grade NAS device.
2. You can use any of the open source media servers like Plex with [REST API interface](https://docs.google.com/document/d/19bTQr99oKn2pOpHcVtqidokbq9zup-K-mFy8JmII6uQ/edit?usp=sharing).

A comprehensive guide to hosting image files and video files can be found [here](https://www.theguardian.com/technology/askjack/2014/jul/31/how-do-i-set-up-a-media-server-to-share-photos-with-phones-and-tablets).


## How to manage local datasets in TrainingData.io application?

Local datasets can be created in two ways:
###1. Method One: Provide location to a folder containing image files:
While creating a new dataset select option "Local"
Enter a name for the new dataset.
Select "Upload Folder" and select the folder that contains images.
IMPORTANT: image paths will be processed recursively and images will *not* be uploaded to cloud.

<!-- [![Local - Edited](https://i.ytimg.com/vi/dPe4nCOB9Y4/hqdefault.jpg)](https://www.youtube.com/embed/dPe4nCOB9Y4) -->

<div class="video-wrapper">
  <iframe width="1280" height="480" src="https://www.youtube.com/embed/dPe4nCOB9Y4" frameborder="0" allowfullscreen></iframe>
</div>

###2. Method two: Upload a CSV file containing list of local urls:
Let's assume our name of our dataset is TCGA-CA-G4H2. This dataset has three folders:

     1. Folder name "Drive" with jpeg files
     2. Folder name "PNG" with png files
     3. Folder name "DICOM" with Dicom files
Arrange folder names and file URLs in following format csv format:

<iframe width='100%' height='250'  src="https://docs.google.com/spreadsheets/d/e/2PACX-1vS0sq3VtQGLMokOyrEuh6sDEnVAkZJeBzFvzsriNSqWZByjFJOgHFp0luJfWEPGqjQYhwOVPhEGo8vk/pubhtml?gid=14120895&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

Upload this csv file while creating a new data set as shown in video below:

<!-- [![CSV Upload for Local Dataset](https://i.ytimg.com/vi/4rKX_mBwUjM/hqdefault.jpg)](https://www.youtube.com/embed/4rKX_mBwUjM) -->

<div class="video-wrapper">
  <iframe width="1280" height="480" src="https://www.youtube.com/embed/4rKX_mBwUjM" frameborder="0" allowfullscreen></iframe>
</div>


## What is recommended directory structure?

It is recommended that only one folder is uploaded in a dataset. TrainingData.io application supports multiple recursive folders under a select folder.

Web Server's root directory MUST BE parent directory of selected folder.

### Sample directory structure:

```
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
```
