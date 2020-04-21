# Create Cloud-Hosted Dataset
Datasets can be hosted in cloud. Location of datasets can be following:
1. A dataset can be hosted on your private cloud, or your AWS S3, your Google Firebase storage, your Azure account.
2. A dataset can be uploaded to TrainingData.io's cloud storage. We use AWS S3.

## 1. Upload Archive: zip or tar to TD.io's Cloud Storage

Alternatively, you can upload an archive:

1. Add new dataset
2. Select "Remote"
3. Enter a name for the dataset
4. Click "Upload Files"
5. Select an archive of files and folders (recursive folder structure preserved with image files)
6. Select "Submit"
Individual image files will be uploaded to TD.io's cloud storage. Folder structure will be preserved exactly as given in archive.

<!-- [![Archive (zip) Dataset - Edited](https://i.ytimg.com/vi/WbTMiDM2b2M/hqdefault.jpg)](https://www.youtube.com/watch?v=WbTMiDM2b2M&feature=youtu.be) -->

<div class="video-wrapper">
  <iframe width="1280" height="480" src="https://www.youtube.com/embed/WbTMiDM2b2M" frameborder="0" allowfullscreen></iframe>
</div>

## 2. Upload Individual Image Files and Folders to TD.io's Cloud Storage

Alternatively, you can upload individual files and Folders to TD.io's Cloud:

1. Add new dataset
2. Select "Remote"
3. Enter a name for the dataset
4. Click "Upload Files"
5. Select "Upload Files" and select individual files
6. Select "Upload Folder" and select individual folder
7. Inspect individual files
8. Select "Submit"
Individual image files will be uploaded to TD.io's cloud storage. (Folder structure will be preserved exactly as that of selected folder)

## 3. Upload Video Files to TD.io's Cloud

Alternatively, you can upload video files to TD.io's Cloud:

1. Add new dataset
2. Select "Remote"
3. Enter a name for the dataset
4. Click "Upload Files"
5. Select "Upload Files" and select individual video files (mov, avi)
6. Inspect video files to be uploaded
8. Select "Submit"
Video files will be broken down into individual frames by TD.io's cloud system

<!-- [![Video File Upload](https://i.ytimg.com/vi/Dvd2DtY1j9s/hqdefault.jpg)](https://www.youtube.com/watch?v=Dvd2DtY1j9s&feature=youtu.be) -->

<div class="video-wrapper">
  <iframe width="1280" height="480" src="https://www.youtube.com/embed/Dvd2DtY1j9s" frameborder="0" allowfullscreen></iframe>
</div>

## 4. Upload CSV File to Self Hosted-Cloud URLs

Prepare a CSV file with a list of URLs as shown below:

1. login to your TrainingData.io account.
2. Select "Data" tab.
3. Select "Add New Dataset".
4. Enter name for new Dataset
5. Select "Remote"
6. Upload a csv file that arranges URLs like this
7. Select "Submit"
8. Inspect new dataset

<iframe width='100%' height='250'  src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRkA6t3G5QC45Kt7f14ntmhvhptID70YQfjoUZWcHIYYVbBCm96oJmXpjpsJd6cZ56eglJzX1T0P7-Z/pubhtml?gid=1329669182&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

<!-- [![Self Hosted Cloud Dataset](https://i.ytimg.com/vi/p8wubMrjpKw/hqdefault.jpg)](https://www.youtube.com/watch?v=p8wubMrjpKw&feature=youtu.be) -->

<div class="video-wrapper">
  <iframe width="1280" height="480" src="https://www.youtube.com/embed/p8wubMrjpKw" frameborder="0" allowfullscreen></iframe>
</div>

## Supported File Formats

TrainingData.io application standard image annotating interface supports the following image file formats.

PNG

JPEG

BMP

DICOM (natively)

NIFTI (natively)

MOV (H.264, H.265, VP8/9 natively)

MP4 (H.264, H.265, VP8/9 natively)

TAR

ZIP

GZ

CSV