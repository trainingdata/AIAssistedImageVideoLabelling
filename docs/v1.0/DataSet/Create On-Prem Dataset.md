# Create an On-Prem Dataset
On-Premises datasets provide security and privacy protection for data.

## 1. Add New On-Prem Dataset with CSV File Upload

Prepare a CSV file with a list of URLs as shown below:

1. login to your TrainingData.io account.
2. Select "DataSet" tab.
3. Select "Add New Dataset".
4. Enter name for new Dataset
5. Select "Local-Hosted Images"
6. Upload a csv file that arranges URLs like this

<iframe width='100%' height='250'  src="https://docs.google.com/spreadsheets/d/e/2PACX-1vS0sq3VtQGLMokOyrEuh6sDEnVAkZJeBzFvzsriNSqWZByjFJOgHFp0luJfWEPGqjQYhwOVPhEGo8vk/pubhtml?gid=14120895&amp;single=true&amp;widget=true&amp;headers=false"></iframe>


<!-- [![Local Dataset using CSV File Upload - Edited](https://i.ytimg.com/vi/rJK58Ed3kAg/hqdefault.jpg)](https://www.youtube.com/watch?v=rJK58Ed3kAg&feature=youtu.be) -->

<div class="video-wrapper">
  <iframe width="1280" height="480" src="https://www.youtube.com/embed/rJK58Ed3kAg" frameborder="0" allowfullscreen></iframe>
</div>

## 2. Add New On-Prem Dataset by Providing Location to a Folder containing Image Files

A dataset can be created using "Upload Folder" if the folder is:

a) mounted as a disk (local disk or network storage),
AND
b) root of webserver serving dataset is same as the uploaded folder

1. Add new dataset
2. Select "Local"
3. Enter a name for the dataset
4. Click "Upload Folder"
5. Select a folder that is root of webserver
6. In video below root of webserver is folder name "imageserver"
7. Enter "File System Path" as base URL: example http://localhost:8000/
8. Select "Submit"  

<!-- [![Create Local Dataset using "Upload Folder" Local - Edited](https://i.ytimg.com/vi/dPe4nCOB9Y4/hqdefault.jpg)](https://www.youtube.com/watch?v=dPe4nCOB9Y4&feature=youtu.be) -->

<div class="video-wrapper">
  <iframe width="1280" height="480" src="https://www.youtube.com/embed/dPe4nCOB9Y4" frameborder="0" allowfullscreen></iframe>
</div>

## What is recommended directory structure?

It is recommended that only one folder is uploaded in a dataset. TrainingData.io application supports multiple recursive folders under a selected folder.

Web Server's root directory MUST BE parent directory of selected folder.

### Sample directory structure:

```
imageserver/
├── radiology
│   └── TCGA-CA-G4H2
│       ├── DICOM
│       │   ├── 000045.dcm
│       │   ├── 000046.dcm
│       │   ├── 000047.dcm
│       │   ├── 000048.dcm
│       │   ├── 000049.dcm
│       │   └── 000050.dcm
│       ├── Drive
│       │   ├── av001.jpg
│       │   ├── av002.jpg
│       │   ├── av003.jpg
│       │   ├── av004.jpg
│       │   └── av005.jpg
│       └── test
│           └── test1
│               ├── av001.jpg
│               ├── av002.jpg
│               └── PNG
│                   ├── 00012.jpg
│                   ├── 00013.jpg
│                   ├── 00014.jpg
│                   ├── 00015.jpg
│                   └── 00016.jpg
7 directories, 19 files
```
