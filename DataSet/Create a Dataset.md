---
title: "Create a Dataset"
excerpt: ""
---
Datasets can be hosted in multiple locations. Location of datasets can be following:
1. A dataset can be local to your intranet (accessible to outside world over a VPN connection) 
2. A dataset can be hosted on your cloud, or your AWS S3, your Google Firebase storage, your Azure account.
3. A dataset can be uploaded to TrainingData.io's cloud storage. We use AWS S3.
[block:api-header]
{
  "title": "1. Add New On-Prem Dataset with CSV File Upload"
}
[/block]
Prepare a CSV file with a list of URLs as shown below: 
1. login to your TrainingData.io account. 
2. Select "Data" tab. 
3. Select "Add New Dataset".
4. Enter name for new Dataset
5. Select "Remote"
6. Upload a csv file that arranges URLs like this
[block:html]
{
  "html": "<iframe width='100%' height='250'  src=\"https://docs.google.com/spreadsheets/d/e/2PACX-1vS0sq3VtQGLMokOyrEuh6sDEnVAkZJeBzFvzsriNSqWZByjFJOgHFp0luJfWEPGqjQYhwOVPhEGo8vk/pubhtml?gid=14120895&amp;single=true&amp;widget=true&amp;headers=false\"></iframe>"
}
[/block]

[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FrJK58Ed3kAg%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DrJK58Ed3kAg&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2FrJK58Ed3kAg%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"854\" height=\"480\" scrolling=\"no\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=rJK58Ed3kAg&feature=youtu.be",
  "title": "Local Dataset using CSV File Upload - Edited",
  "favicon": "https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico",
  "image": "https://i.ytimg.com/vi/rJK58Ed3kAg/hqdefault.jpg"
}
[/block]

[block:api-header]
{
  "title": "2. Add New On-Prem Dataset with Folder Upload"
}
[/block]
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
[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FdPe4nCOB9Y4%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DdPe4nCOB9Y4&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2FdPe4nCOB9Y4%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"854\" height=\"480\" scrolling=\"no\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=dPe4nCOB9Y4&feature=youtu.be",
  "title": "Create Local Dataset using \"Upload Folder\" Local - Edited",
  "favicon": "https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico",
  "image": "https://i.ytimg.com/vi/dPe4nCOB9Y4/hqdefault.jpg"
}
[/block]

[block:api-header]
{
  "title": "3. Upload Archive: zip or tar to TD.io's Cloud Storage"
}
[/block]
Alternatively, you can upload an archive:
1. Add new dataset
2. Select "Remote"
3. Enter a name for the dataset
4. Click "Upload Files"
5. Select an archive of files and folders (recursive folder structure preserved with image files)
6. Select "Submit"
Individual image files will be uploaded to TD.io's cloud storage. Folder structure will be preserved exactly as given in archive.
[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FWbTMiDM2b2M%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DWbTMiDM2b2M&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2FWbTMiDM2b2M%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"640\" height=\"480\" scrolling=\"no\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=WbTMiDM2b2M&feature=youtu.be",
  "title": "Archive (zip) Dataset - Edited",
  "favicon": "https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico",
  "image": "https://i.ytimg.com/vi/WbTMiDM2b2M/hqdefault.jpg"
}
[/block]

[block:api-header]
{
  "title": "4. Upload Individual Files and Folders to TD.io's Cloud"
}
[/block]
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
[block:api-header]
{
  "title": "5. Upload Video Files to TD.io's Cloud"
}
[/block]
Alternatively, you can upload video files to TD.io's Cloud:
1. Add new dataset
2. Select "Remote"
3. Enter a name for the dataset
4. Click "Upload Files"
5. Select "Upload Files" and select individual video files (mov, avi) 
6. Inspect video files to be uploaded
8. Select "Submit"
Video files will be broken down into individual frames by TD.io's cloud system
[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FDvd2DtY1j9s%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DDvd2DtY1j9s&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2FDvd2DtY1j9s%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"854\" height=\"480\" scrolling=\"no\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=Dvd2DtY1j9s&feature=youtu.be",
  "title": "Video File Upload",
  "favicon": "https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico",
  "image": "https://i.ytimg.com/vi/Dvd2DtY1j9s/hqdefault.jpg"
}
[/block]

[block:api-header]
{
  "title": "6. Upload CSV File with Self Hosted-Cloud URLs"
}
[/block]
Prepare a CSV file with a list of URLs as shown below: 
1. login to your TrainingData.io account. 
2. Select "Data" tab. 
3. Select "Add New Dataset".
4. Enter name for new Dataset
5. Select "Remote"
6. Upload a csv file that arranges URLs like this
7. Select "Submit"
8. Inspect new dataset
[block:html]
{
  "html": "<iframe width='100%' height='250'  src=\"https://docs.google.com/spreadsheets/d/e/2PACX-1vRkA6t3G5QC45Kt7f14ntmhvhptID70YQfjoUZWcHIYYVbBCm96oJmXpjpsJd6cZ56eglJzX1T0P7-Z/pubhtml?gid=1329669182&amp;single=true&amp;widget=true&amp;headers=false\"></iframe>"
}
[/block]

[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2Fp8wubMrjpKw%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3Dp8wubMrjpKw&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2Fp8wubMrjpKw%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"854\" height=\"480\" scrolling=\"no\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=p8wubMrjpKw&feature=youtu.be",
  "title": "Self Hosted Cloud Dataset",
  "favicon": "https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico",
  "image": "https://i.ytimg.com/vi/p8wubMrjpKw/hqdefault.jpg"
}
[/block]

[block:api-header]
{
  "title": "Supported File Formats"
}
[/block]
TrainingData.io application standard image annotating interface supports the following image file formats.
PNG
JPEG
BMP
DCM
TAR
ZIP
GZ