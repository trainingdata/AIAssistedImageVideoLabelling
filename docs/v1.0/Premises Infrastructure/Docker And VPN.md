# On Premises Infrastructure
We provide a Docker image that you can run in your own network. Host your data within your own network or on your own private cloud. Your training data will be unreachable to TrainingData.io. Only annotations (labels) will be saved on TrainingData.io's cloud.

## Pre-requisite: Install Docker
Pre-requisite: Install Docker on Windows Pro, Ubuntu 16.04 or 16.05, Mac Os X.

## How to Install On-Premises Annotation Tool Using Docker?

To download and run Docker image follow these steps:

(Latest release of docker image is v1.7.8)

1. Use shell on Unix or Mac OS X (or PowerShell on Windows)

        docker pull trainingdataio/tdviewer:v1.7.8

2. Create a directory on your disk to store TD.io database. For example "C:\db"
   
        windows: $ mkdir -p  c:\db
        unix/Mac: $ mkdir -p /path/to/directory/db

3. (Optional) Create a directory to place images and videos (dataset assets). For example: "C:\images"

        windows: $ mkdir -p c:\Images
        unix: $ mkdir -p /path/to/directory/images

4. Run Docker image providing mount point for database and mount point for images folder.

        docker run --mount src=c:\db,target=/home/user/trainingdataio/tdviewer/db,type=bind --mount src=c:\Images,target=/home/user/trainingdataio/tdviewer/images,type=bind -p 8090:8090 trainingdataio/tdviewer:v1.7.8

5. Login to https://app.trainingdata.io
6. Create a on-premises dataset as described [here](/v1.0/Premises Infrastructure/Prem Datasets).
5. Create a labeling instruction with classes and attributes
6. Create a labeling job with a dataset and a labeling-instruction.
7. Start labeling your local-hosted project.

## Video for Mac OS X: On-Premises Docker Image

Annotation tool is served using a web server on port 8090.
Images are served from the same port 8090, in sub-directory http://localhost:8090/images/.

<!-- [![On Premises Docker Mac OS X](https://i.ytimg.com/vi/X3QOo_lJrjE/hqdefault.jpg)](https://www.youtube.com/watch?v=X3QOo_lJrjE&feature=youtu.be) -->

<div class="video-wrapper">
  <iframe width="1280" height="480" src="https://www.youtube.com/embed/X3QOo_lJrjE" frameborder="0" allowfullscreen></iframe>
</div>

## Video for Ubuntu: On-Premises Docker Image

Annotation tool is served using a web server on port 8090.
Image server is served on port 8090, in sub-directory http://localhost:8090/images/.

<!-- [![Ubuntu](https://i.ytimg.com/vi/ESAtt73cBLw/hqdefault.jpg)](https://www.youtube.com/watch?v=ESAtt73cBLw&feature=youtu.be) -->

<div class="video-wrapper">
  <iframe width="1280" height="480" src="https://www.youtube.com/embed/ESAtt73cBLw" frameborder="0" allowfullscreen></iframe>
</div>


## Video: Project Management on Cloud

Project management, project meta-data, Dataset management, Dataset meta-data, collaborator management happens on cloud. *All your imaging data sets and annotations stay in your private network.*

<!-- [![May 23, 2019 1:25 PM](https://i.ytimg.com/vi/45nKiW8inFM/hqdefault.jpg)](https://www.youtube.com/watch?v=45nKiW8inFM&feature=youtu.be) -->

<div class="video-wrapper">
  <iframe width="1280" height="480" src="https://www.youtube.com/embed/45nKiW8inFM" frameborder="0" allowfullscreen></iframe>
</div>


## Hosting Private On-Premises DataSets

Host datasets on any of your favorite web-servers or media servers or PACs for radiology.

For quick testing use NodeJS's built in webserver with directory images stored in ./imageserver:

##### Command Line
```shell
npx http-server --cors -p 8000 ./imageserver
```

## [How to manage On-Premises DataSets in TD.io?](https://docs.trainingdata.io/v1.0/DataSet/Create%20Cloud%20Hosted%20Dataset/)
