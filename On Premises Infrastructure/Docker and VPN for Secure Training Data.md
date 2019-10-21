---
title: "Docker and VPN for Secure Training Data"
excerpt: ""
---
[block:api-header]
{
  "title": "Private On-Premises Annotation Tool Using Docker"
}
[/block]
Download Docker image that runs annotation tool. Both data and annotations remain private with-in local network.

(Latest release of docker image is v1.7.4)

1. Use shell on Unix or Mac OS X (or PowerShell on Windows)
[block:code]
{
  "codes": [
    {
      "code": " docker pull trainingdataio/tdviewer:v1.7.4\n",
      "language": "shell"
    }
  ]
}
[/block]
2. Create a directory on your disk to store TD.io database. For example "C:\db"

[block:code]
{
  "codes": [
    {
      "code": "mkdir -p  c:\\db",
      "language": "shell"
    }
  ]
}
[/block]
3. (Optional) Create a directory to place images and videos (dataset assets). For example: "C:\images"
[block:code]
{
  "codes": [
    {
      "code": "mkdir -p c:\\Images",
      "language": "shell"
    }
  ]
}
[/block]
4. Run Docker image providing mount point for database and mount point for images folder.
[block:code]
{
  "codes": [
    {
      "code": "docker run --mount src=c:\\db,target=/home/user/trainingdataio/tdviewer/db,type=bind --mount src=c:\\Images,target=/home/user/trainingdataio/tdviewer/images,type=bind -p 127.0.0.1:8090:8090 trainingdataio/tdviewer:v1.7.4",
      "language": "shell"
    }
  ]
}
[/block]
5. Login to https://app.trainingdata.io
6. Create a local dataset as described here: [https://trainingdata.readme.io/docs/local-datasets](https://trainingdata.readme.io/docs/local-datasets).
5. Create a labeling interface with classes and attributes
6. Create a project with the dataset in (4) and the labeling-interface in (5).
7. Start labeling your local hosted project.
[block:api-header]
{
  "title": "Mac OS X: On-Premises Docker Image"
}
[/block]
Annotation tool is served using a web server on port 8090. 
Image server is served on port 8000.
[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FX3QOo_lJrjE%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DX3QOo_lJrjE&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2FX3QOo_lJrjE%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"640\" height=\"480\" scrolling=\"no\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=X3QOo_lJrjE&feature=youtu.be",
  "title": "On Premises Docker Mac OS X",
  "favicon": "https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico",
  "image": "https://i.ytimg.com/vi/X3QOo_lJrjE/hqdefault.jpg"
}
[/block]

[block:api-header]
{
  "title": "Ubuntu: On-Premises Docker Image"
}
[/block]
Annotation tool is served using a web server on port 8090. 
Image server is served on port 8000.
[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FESAtt73cBLw%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DESAtt73cBLw&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2FESAtt73cBLw%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"640\" height=\"480\" scrolling=\"no\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=ESAtt73cBLw&feature=youtu.be",
  "title": "Ubuntu",
  "favicon": "https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico",
  "image": "https://i.ytimg.com/vi/ESAtt73cBLw/hqdefault.jpg"
}
[/block]

[block:api-header]
{
  "title": "Project Management on Cloud"
}
[/block]
Project management, project meta-data, Dataset management, Dataset meta-data, collaborator management happens on cloud. *All your imaging data sets and annotations stay in your private network.* 
[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2F45nKiW8inFM%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3D45nKiW8inFM&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2F45nKiW8inFM%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"854\" height=\"480\" scrolling=\"no\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=45nKiW8inFM&feature=youtu.be",
  "title": "May 23, 2019 1:25 PM",
  "favicon": "https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico",
  "image": "https://i.ytimg.com/vi/45nKiW8inFM/hqdefault.jpg"
}
[/block]

[block:api-header]
{
  "title": "Private On-Premises DataSets"
}
[/block]
Host datasets on any of your favorite web-servers or media servers or PACs for radiology.

For quick testing use node's built in webserver with directory images stored in ./imageserver:
 
[block:code]
{
  "codes": [
    {
      "code": "npx http-server --cors -p 8000 ./imageserver",
      "language": "shell",
      "name": "Command Line"
    }
  ]
}
[/block]