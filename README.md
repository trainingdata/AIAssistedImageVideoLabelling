# TrainingData.io: AI Assisted Image & Video Training Data Labeling @ Scale

# Table Of Contents

+ [Overview](#overview)
  + [Complete Feature Set](#complete-feature-set)
  + [Quality Management](#quality-management)
  + [Security and Privacy](#security-and-privacy)
  + [FAQ](#faq)
+ [Quality Management Workflow](#quality-management-workflow)
  + [Annotator Performance Management](#annotator-performance-management)
  + [Roles: Admin](#roles--admin)
  + [Roles: Annotator](#roles--annotator)
  + [Roles: Reviewer](#roles--reviewer)
+ [On Premises Infrastructure](#on-premises-infrastructure)
  + [Docker and VPN for Secure Training Data](#docker-and-vpn-for-secure-training-data)
  + [Ubuntu: Troubleshooting Docker](#ubuntu--troubleshooting-docker)
  + [Windows: Troubleshooting Docker](#windows--troubleshooting-docker)
  + [On-Prem Datasets](#on-prem-datasets)
  + [Cloud Hosted Datasets](#cloud-hosted-datasets)
+ [Pixel Accurate Tools](#pixel-accurate-tools)
  + [Segmentation with Brush & Eraser](#segmentation-with-brush--eraser)
  + [Freehand with Sculpter](#freehand-with-sculpter)
  + [Polygon Tool](#polygon-tool)
  + [Magnify](#magnify)
  + [2D Growth Tool for DICOM](#2d-growth-tool-for-dicom)
+ [Labeling Instructions](#labeling-instructions)
  + [KeyBoard Shortcuts: Productivity](#keyboard-shortcuts--productivity)
  + [Labeling Instruction Builder](#labeling-instruction-builder)
+ [AI Assisted Annotation](#ai-assisted-annotation)
  + [Segmentation of Liver](#segmentation-of-liver)
  + [Segmentation of Spleen](#segmentation-of-spleen)
+ [DataSet](#dataset)
  + [Create a Dataset](#create-a-dataset)
  + [Delete a Dataset](#delete-a-dataset)
+ [Projects](#projects)
  + [Add New Project](#add-new-project)
  + [Start Annotation](#start-annotation)
+ [Collaborators](#collaborators)
  + [Add Collaborators to a Specific Project](#add-collaborators-to-a-specific-project)
  + [Add a Collaborator](#add-a-collaborator)
  + [Collaborators](#collaborators)
+ [Workspace](#workspace)
  + [Active Viewport Image](#active-viewport-image-middle)
  + [Folder Navigation](#folder-navigation-left)
  + [Label Data](#label-data-right)
  + [ToolBar](#toolbar-top)
+ [Terms and Conditions](#terms-and-conditions)
  + [Privacy Policy](#privacy-policy)
  + [Terms of Use](#terms-of-use)


# Overview
TrainingData.io application provides high precision training data labeling for Visual AI. Our SaaS solution uses AI assisted features to give machine learning engineers speed up of several orders of magnitude. Our goal is to "empower data scientists to control quality of training data"

## Key Benefits

1. High precision labeling tool with Superpixel segmentation, AI-assisted labeling, and active-learning.
2. Custom labeling instructions for every task - delivers productivity enhancing user-experience for annotators.
3. Data security and privacy protection using On-premises, In-cloud or hybrid hosting. (using Docker and VPN)
4. Collaboration with multiple annotator's on same task.
5. Annotator performance and quality management workflow.
6. AI-Assisted annotation using existing ML models.
7. Out of the box support for medical imaging (DICOM).


![Key Benefits of TrainingData.io](https://files.readme.io/2020847-NewWorkflow.png)



![Old Workflow](https://files.readme.io/39f6721-CurrentWorkflow.png)



## 

#[Click Here For Complete Feature Set](#complete-feature-set)


# Complete Feature Set
At TrainingData.io, we believe quality of the machine learning model is dependent on the quality of labelling. We empower data-scientists to control the quality of data labelling in the following ways:

## Segmentation and Classification

TD.io's application supports following types of annotation work:
1. Segmentation only
2. Classification only
3. Segmentation with Classification.

## Pixel Accurate Tools

We use advanced image processing to provide pixel accurate tools like
1. [Superpixel-segmentation](#segmentation-with-brush--eraser) with brush and eraser,
2. [Polygon](#polygon-tool) with advanced editing, bounding box, 
3. [Freehand-draw with sculpter](#freehand-with-sculpter), and
4. Region of Interest (ROI) growth tool.


## AI Assisted Annotation

1. AI Assisted Annotation using Data-scientist's ML model
2. AI Assisted Annotation using NVIDIA Clara


## Data Security and Privacy Controls

On-premises hosting of datasets and annotation tools using Docker and VPN.

## Collaboration: Annotator's Performance Management

1. Measure, record and analyze annotator's performance on every individual task, asset and label.
2. Compare performance of multiple annotators on same task.
3. Distribute labeling work among multiple labelers and observe consensus among their work.
4. Seed annotation tasks with golden data set. Report performance of annotator on golden data set.

## Labeling Instruction Builder

[Labeling instruction builder](#labeling-instruction-builder-2) empowers data scientist to define user experience of annotators in fine-detail:
1. Labeling classes and ontology can be defined in fine-detail.
2. WYSIWYG instruction builder enables  data-scientist to view how labeling interface appears to the annotator.

We believe the quality of work performed by annotators depends on the quality of user experience in annotation tools. We build intuitive user experience for annotators.

## WorkForce: Humans-in-the-Loop

We partner with highest quality workforce from around the world.

# Security and Privacy
At TrainingData.io we take data security and privacy very seriously. 

We allow you to log in to TrainingData.io application using the same identity provider that you use for other services.

## Data Security
We allow data owners to control who accesses their data. Each annotator's (internal or external) activity is recorded and they are not allowed to download training data. We allow data owners to see complete access log of every collaborator's activity. 

## Single Sign-On
TrainingData.io supports single sign-on (SSO), which allows you to log in to TrainingData.io application using the same identity provider that you use for other services.

## On Premises Solution
We  provide our labeling software as Docker image, it can run as hosted solution in your network. Hosted version of annotation tool can access images that are hosted on local machine, images hosted on local web-server or images hosted in cloud. All training data and resulting labels are saved on local infrastructure. Only project definition sits in cloud.


![On-Prem Solution using Docker Container and VPN](https://files.readme.io/819bde1-Docker.png)

## Cloud Hosted Solution
You can upload your assets (images and videos) to our cloud. Our cloud is secure with equivalent of HIPAA compliance. (We sign BAA agreement if needed).

## Hybrid Solution
We offer hybrid solution where annotation tool is installed on local infrastructure as Docker instance. Training data is hosted in cloud.

# Quality Management
At TrainingData.io, we believe, quality of the machine learning model is entirely dependent on the quality of labeling for training data. We help you control quality of data labeling in following ways:

## Annotator's Performance Management

1. Measure, record and analyze annotator's performance on every individual task, asset and label.
2. Compare performance of multiple annotators on same task.
3. Distribute labeling work among multiple labelers and observe consensus among their work.
4. Seed annotation tasks with golden data set. Report performance of annotator on golden data set.

## Pixel Accurate tools

1. We use advanced image processing to build pixel accurate tools like segmentation, freehand, growth tools.
2. Build high quality user experience for annotators that allows then to do high quality work at fast pace.
3. Enable smooth collaboration between annotators and data-scientists.

## State of the art User Experience (UX)

1. TD.io believes quality of work performed by annotators depends on quality of user experience in annotation tools
2. We build intuitive user experience for annotators.

## Labeling Instruction Builder

1. Empowering data scientist to take control user experience of annotators.
2. Labeling classes and ontology needs to be defined in detail.
3. Data scientist needs precise view of how labeling interface appears to the annotator.

# FAQ
#General Questions
**What is TrainingData.io?**
TrainingData.io application is a AI training-data management platform. Our goal is to  empower data science team to control the training data management workflow.

**What is Data annotation?**
In order to train machines to make decisions on behalf of humans, they must learn to make those decisions. In order to learn about the world around us, machines take input in form of images and text that is labeled for representative features. A label in an image is clearly marked bounding region that represents a real world entity or object. Managing data labeling at very large scale is time consuming and requires special software.

**What can I annotate with TrainingData.io application?**
With our labeling solution you can label any visual dataset including images and videos. We support medical imaging format - DICOM. 

**What kind of data formats are supported by TrainingData.io? **
Our annotation tools support JPEG, PNG, DICOM, mov, avi, mp4, zip, tar, gz

**How Trainingdata.io application will help my data science team deploy Machine Learning/Artificial Intelligence?**
Trainingdata.io is a place where you can start small and scale-up your data management operations with time. We help you manage early-stage AI projects with internal stakeholders. Once your are ready to scale operations we connect you with human-labelers outside your organization. We help you control quality of work produced by third-party human labelers. This helps you improve quality of your machine learning models at fast pace and at fraction of cost. 

****

**How is Trainingdata.io different from managed labeling services?**
Managed Labeling services produce error rates as high as 65%. This is due to low quality and inconsistency of labeling tools. Quality of labels produced by workforce depends on quality of user experience for the human labelers. We empower data science team to control user-experience of human labelers. 

What sets us apart is our focus on:
1. Pixel accurate annotation tools
2. Customizable labeling interface for every task
3. Quality and performance management
4. Data security and privacy protection with on-premises solution.

Compare the two workflows in image below:

**Old (current) Work Flow**

![Old Work Flow](https://files.readme.io/4108b7a-CurrentWorkflow.png)

**New Work Flow**

![New Work Flow](https://files.readme.io/2bbda76-NewWorkflow.png)

**How do I get started with Trainingdata.io application?**
You can sign up at [login page](https://app.trainingdata.io/v1/td/login).

**Does Trainingdata.io provide support?**
Trainingdata.io provides support to all users. 

**Does TrainingData.io have a discount for academic users?**
Yes, we do

**I have my data annotated by a service. Why would I use TrainingData.io?**
With TrainingData.io you can still outsource your annotating projects as well as leverage your internal team on those same projects. The big differentiator is that with TrainingData.io you can manage the quality and performance of your entire annotating team whether they are outsourced or internal, all in one place.

TrainingData.io does not provide in-house annotating services but we do work with several annotating companies (BPO Firms) that we have vetted and currently work with many of our customers in TrainingData.io. We simply recommend them as a third party to help our customers so you are always free to choose any annotating services company that meets your requirements.

**My company built an internal labeling tool that seems to work okay. Why would I use TrainingData.io?**
It's quick and easy to start annotating data using locally installed tools. For most simple annotation tasks being performed by a single annotator, this solution architecture annotates well. As data annotation needs scale, data management and quality control processes are needed to produce accurate and consistent training data. A common cause of under performing AI systems is low accuracy training data.

**When building data labeling infrastructure, consider the following:**

  * Total Cost of Ownership
Homegrown tools are built to exist and serve a particular function, but with new business, demands come to the cost of upgrades. There is a high cost of ongoing maintenance, both in time and money. Technical debt accrues over time due to engineer turn-over, product neglect, and evolving product demands.

  * Unknown and Evolving Scope
Developing an internal product requires planning, resource allocation, and preparing for the unknown. Because feature flagging platforms are relatively new, it can be difficult to accurately define the scope and construct a solution for needs across engineering and product groups.

  * Minimum Viable Functionality
Internal tools are generally not built for usability, scalability, or cross-team support. They are built to solve an immediate pain point or provide minimum viable functionality as quickly as possible.

  * Data Labeling is Cross Functional
Turning raw data into accurate and consistent training data is a team effort. Engineers, domain experts (annotators), and managers must work together while playing different roles. Data annotation infrastructure must facilitate this by providing information and interfaces unique to these roles.

  * Enterprise Readiness
Productizing AI systems takes fast, reliable, and scaled infrastructure across raw data collection, data labeling, and compute.

**Will TrainingData.io improve the quality and consistency of my labeled data?**
This is one of our core competencies and one of the main reasons we decided to build TrainingData.io application. We saw that all the available options for annotating made it extremely difficult to ensure our training data was high enough in quality for a production-ready machine learning model and it cost us valuable time and money in the end. We developed a world-class quality and performance management interface within our platform to address this.

**Annotation Questions**
**How do I setup a project?**
You can set up a project in three steps:
1. Click “Add Project” and give the project a name.
2. Attach your data set to the project.
3. Customize your labeling interface.
4. Start Labeling!

**Does TrainingData.io work with Cloud buckets data such as Amazon S3 or Google Cloud Storage?**
Check out our guide for Connecting Cloud Data.

**How do I revisit skipped or submitted labels?**
You can do this by Re-Enqueuing them from the Activity Tab. For a guide on Re-Enqueuing labels click here

**Does TrainingData.io work with on-premises data?**
TrainingData.io works with source data hosted on-premises or on a private cloud. The source data is accessed directly from the client computer and never shared (or accessible) by TrainingData.io. Check out our guide here.

**Does TrainingData.io work on mobile devices?**
We do not currently support mobile devices, although we are working on adding this in the future.

**Can I annotate on an iPad?**
Yes .

**Does Trainingdata.io work in all countries?**
Yes, unless your network has a restrictive firewall, or you have internet connectivity issues. We currently only support the English language on our platform.

**Does Trainingdata.io application work without an internet connection?**
No, you must have an internet connection to use trainingdata.io application.

**What browser do you recommend for trainingdata.io application?**
We recommend Chrome. We do not recommend Internet Explorer or Safari due to compatibility issues.

**What formats can I export my annotated data?**
Your annotated data can be exported in JSON, Mask and PNG which should allow  you to import it into any machine learning framework.

**How does Auto Consensus work?**
Auto Consensus ensures consistency and accuracy of the labeled data. When turned on, some or all of the images are labeled by more than one labeler so that a consensus among labelers for each labeled datum can be calculated and ultimately managed. You can configure the percentage of your dataset in a project that will be randomly selected to be labeled more than once by distinct collaborators. You can also configure the number of times this percentage of labels will be labeled. Check out our docs here for more detail.

**Will other labelers see the same data that I'm labeling?**
If Auto Consensus is turned on and configured then yes, otherwise no.

**Does TrainingData.io have an API?**
Yes, we have a fully featured API. Everything you can do with our interface, you can do programmatically through our API. The API is available on our Enterprise tier. You may contact sales at https://trainingdata.io/contact.

If you are a paid user you may request an API key from our support team via the Chat icon (preferred method) or by sending an email to info@trainingdata.io, and title it "API Request".*

**I already have training data. Can I import it into Trainingdata.io application?**
Yes, it can be imported. Simply send us the annotated data and we will reformat it and upload it for you.

**How do I delete a project?**
Open your project then go to settings > Other, and click on the delete button.*

# Quality Management Workflow

## Annotator Performance Management

Analyze performance of every annotator for every image or video-frame. Following statistics are available:
1. Number of labels created by an annotator.
2. Time spent per label (average) in seconds.
3. Total time spent on the project in seconds.
4. Last activity by every annotator.
5. Reviewers can accept or reject annotations of every annotator. Reviewer acceptance rate is a percentage that is calculated by aggregating reviewer's acceptance count.  
6. Reviewers can optionally give a score for every image. Reviewer's average score (between 0 and 10) is calculated 
7. Consensus using IOU


![Annotator Performance](https://files.readme.io/da2f882-AfterReview1.png)



## Review Mode: How to review a task performed by Annotators

In Review mode performance of an annotator can be reviewed for every image or video-frame. As seen in video below reviewers can
1. "Accept" "Reject" an annotation: Mandatory 
2. Give a score between 0 and 10, (optional).
3. Leave a comment for the annotator (optional).

[![How To Review Annotations created by an Annotator TrainingData](https://i.ytimg.com/vi/UEjkveN3hFg/hqdefault.jpg)](https://www.youtube.com/embed/UEjkveN3hFg)



![Graphical User Interface for Reviews](https://files.readme.io/8ec6485-Review.png)



## Annotation Mode: How to create annotations

From project settings page select button "Start Annotating". 
1. Select classes on right panel
2. When a class is selected, corresponding tool is activated.
3. Draw annotation with respective tool
4. Enter questionnaire related to the annotations
5. Press Button:"Save" to save annotation
6. Press Button:"Delete" to delete an annotation.
7. Press left button or right button to move left and right.

[![Role: Annotator - How to create annotations](https://i.ytimg.com/vi/bHrd55nISzY/hqdefault.jpg)](https://www.youtube.com/embed/bHrd55nISzY)

# Roles- Admin

## What is Admin's Role?

1. Admin can create annotations. 
2. Admin can review annotations.

Image below shows admin's view of a task with ability to annotate and review-annotations.


![Admin's view to project settings](https://files.readme.io/2ecdb5f-Admin.png)



## Admin Mode: How to create annotations



[![Role: Annotator - How to create annotations](https://i.ytimg.com/vi/bHrd55nISzY/hqdefault.jpg)](https://www.youtube.com/embed/bHrd55nISzY)



## Admin Mode: How to review annotations



[![How To Review Annotations created by an Annotator TrainingData'](https://i.ytimg.com/vi/UEjkveN3hFg/hqdefault.jpg)](https://www.youtube.com/embed/UEjkveN3hFg)

# Roles- Annotator

## What is Annotator's Role?

Every project can have multiple collaborators. A collaborator can be an admin, annotator or reviewer. An admin can annotate and review. An annotator can only annotate, not review. A reviewer is usually a subject matter expert, they can review annotations (and add modifications to annotations)

Annotator can only add or modify annotations. They will also see reviews from reviewers.

Image below shows annotator seeing reviews by a reviewer.

![Review Comments Visible to Annotator](https://files.readme.io/25655db-AnnotatorReviewComments.png)



## Annotation Mode: How to create annotations



[![Role: Annotator - How to create annotations](https://i.ytimg.com/vi/bHrd55nISzY/hqdefault.jpg)](https://www.youtube.com/embed/bHrd55nISzY)

# Roles- Reviewer

## What is Reviewer's Role?

Every project can have multiple collaborators. A collaborator can be an admin, annotator or reviewer. An admin can annotate and review. An annotator can only annotate, not review. A reviewer is usually a subject matter expert, they can review annotations (and add modifications to annotations)

In Review mode performance of an annotator can be reviewed for every image or video-frame. Review mode gives reviewer to:
1. "Accept" or "Reject" an annotation. 
2. Enter a score between 0 and 10.
3. Leave a comment for the annotator.

[![How To Review Annotations created by an Annotator TrainingData](https://i.ytimg.com/vi/UEjkveN3hFg/hqdefault.jpg)](https://www.youtube.com/embed/UEjkveN3hFg)

# On Premises Infrastructure



## Docker and VPN for Secure Training Data

## Private On-Premises Annotation Tool Using Docker

Download Docker image that runs annotation tool. Both data and annotations remain private with-in local network.

(Latest release of docker image is v1.7.4)

1. Use shell on Unix or Mac OS X (or PowerShell on Windows)

2. Create a directory on your disk to store TD.io database. For example "C:\db"


3. (Optional) Create a directory to place images and videos (dataset assets). For example: "C:\images"

4. Run Docker image providing mount point for database and mount point for images folder.

5. Login to https://app.trainingdata.io
6. Create a local dataset as described [here](#on-prem-datasets).
5. Create a labeling interface with classes and attributes
6. Create a project with the dataset in (4) and the labeling-interface in (5).
7. Start labeling your local hosted project.

## Mac OS X: On-Premises Docker Image

Annotation tool is served using a web server on port 8090. 
Image server is served on port 8000.

[![On Premises Docker Mac OS X](https://i.ytimg.com/vi/X3QOo_lJrjE/hqdefault.jpg)](https://www.youtube.com/watch?v=X3QOo_lJrjE&feature=youtu.be)



## Ubuntu: On-Premises Docker Image

Annotation tool is served using a web server on port 8090. 
Image server is served on port 8000.

[![Ubuntu](https://i.ytimg.com/vi/ESAtt73cBLw/hqdefault.jpg)](https://www.youtube.com/watch?v=ESAtt73cBLw&feature=youtu.be)



## Project Management on Cloud

Project management, project meta-data, Dataset management, Dataset meta-data, collaborator management happens on cloud. *All your imaging data sets and annotations stay in your private network.* 

[![May 23, 2019 1:25 PM](https://i.ytimg.com/vi/45nKiW8inFM/hqdefault.jpg)](https://www.youtube.com/watch?v=45nKiW8inFM&feature=youtu.be)



## Private On-Premises DataSets

Host datasets on any of your favorite web-servers or media servers or PACs for radiology.

For quick testing use node's built in webserver with directory images stored in ./imageserver:
 

##### 
```shell
 docker pull trainingdataio/tdviewer:v1.7.4

```

##### 
```shell
mkdir -p  c:\db
```

##### 
```shell
mkdir -p c:\Images
```

##### 
```shell
docker run --mount src=c:\db,target=/home/user/trainingdataio/tdviewer/db,type=bind --mount src=c:\Images,target=/home/user/trainingdataio/tdviewer/images,type=bind -p 127.0.0.1:8090:8090 trainingdataio/tdviewer:v1.7.4
```

##### Command Line
```shell
npx http-server --cors -p 8000 ./imageserver
```

# Ubuntu- Troubleshooting Docker

## [Error: EACCES: permission denied, open 'db/trainingdata.db']

Or

## Mounted host volume is not writable from container

Your account's uid on host `id -u` is not the same as the uid of the user who is running the docker container. Try this:  

Now run docker image again. If you still get the same error try this:

Now run docker image again.
##### 
```shell
sudo groupadd docker
sudo usermod -aG docker $USER
```

##### 
```shell
chmod a+rwx -R db/


```

# Windows- Troubleshooting Docker

## Run PowerShell in Admin Mode

In Start-Menu search for 'powershell'. To run PowerShell as administrator, right-click (or tap and hold, if you use a touchscreen) on the Windows PowerShell search result, and then click or tap "Run as administrator." (as shown in screenshot below)

## Windows 10



![Windows 10: Run PowerShell as Admin](https://files.readme.io/e1bdd0c-Powershell.png)



## Windows 7



![Windows 7: Run PowerShell as Admin](https://files.readme.io/c3dcf8b-PowerShell-Windows7.png)



## Restart Docker in PowerShell

Type following six commands in same order as given below:



## Error Code: open //./pipe/docker_engine: System cannot find file

error during connect: Get http://%2F%2F.%2Fpipe%2Fdocker_engine/v1.29/version: open //./pipe/docker_engine: The system cannot find the file specified. In the default daemon configuration on Windows, the docker client must be run elevated to connect . This error may also indicate that the docker daemon is not running.



## Stuck in: "Waiting for an IP..." "Creating SSH Keys..."

Docker on Windows has a slew of problems. Here are few things you can try:


For more details refer to this article: https://github.com/docker/toolbox/issues/457
##### 
```shell
net stop docker
net stop com.docker.service
taskkill /IM "dockerd.exe" /F
taskkill /IM "Docker for Windows.exe" /F
net start docker
net start com.docker.service
```

##### 
```shell
docker-machine create default --virtualbox-no-vtx-check
docker-machine restart default



```

##### 
```shell
First Disable AntiVirus
Next Disable FireWall
Next Run these commands
docker-machine rm default
docker-machine create --driver virtualbox --virtualbox-no-vtx-check default
```

# Cloud Hosted Datasets

## Whose Cloud?

TrainingData.io supports any cloud storage that has configurable CORS policy. 

You can use your own cloud storage or upload data to TD.io's cloud storage.

Our cloud storage comes with HIPAA compliance.

## Self Hosted Cloud Datasets

Data scientists can use self-hosted datasets as shown in CSV file. Prepare a CSV file with a list of URLs as shown below: 
1. login to your TrainingData.io account. 
2. Select "Data" tab. 
3. Select "Add New Dataset".
4. Enter name for new Dataset
5. Select "Remote"
6. Upload a csv file that arranges URLs like this
7. Select "Submit"
8. Inspect new dataset
https://docs.google.com/spreadsheets/d/e/2PACX-1vRkA6t3G5QC45Kt7f14ntmhvhptID70YQfjoUZWcHIYYVbBCm96oJmXpjpsJd6cZ56eglJzX1T0P7-Z/pubhtml?gid=1329669182&amp;single=true&amp;widget=true"


[![Self Hosted Cloud Dataset](https://i.ytimg.com/vi/p8wubMrjpKw/hqdefault.jpg)](https://www.youtube.com/embed/p8wubMrjpKw)



## TD.io Hosted Cloud Dataset

Alternatively, you can upload individual files and Folders to TD.io's Cloud. TD.io's cloud hosting is HIPAA compliant.
1. Add new dataset
2. Select "Remote"
3. Enter a name for the dataset
4. Click "Upload Files"
5. Select "Upload Files" and select individual files 
6. Select "Upload Folder" and select individual folder
7. Inspect individual files
8. Select "Submit"
Individual image files will be uploaded to TD.io's cloud storage. (Folder structure will be preserved exactly as that of selected folder)

[![TD.io's Cloud Hosted Dataset - Edited](https://i.ytimg.com/vi/LT1hnxT_kD0/hqdefault.jpg)](https://www.youtube.com/watch?v=LT1hnxT_kD0&feature=youtu.be)

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

[![Local - Edited](https://i.ytimg.com/vi/dPe4nCOB9Y4/hqdefault.jpg)](https://www.youtube.com/embed/dPe4nCOB9Y4)

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

[![CSV Upload for Local Dataset](https://i.ytimg.com/vi/4rKX_mBwUjM/hqdefault.jpg)](https://www.youtube.com/embed/4rKX_mBwUjM)



## What is recommended directory structure?

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

# Pixel Accurate Tools

# Segmentation with Brush & Eraser
Segmentation tool works for JPEG, PNG and DICOM images

## How to use Segmentation Tool

**Configure Segmentation Tool**

* Paint mode will turn mouse-pointer into a painting tool.
* Erase mode will turn mouse-pointer into an eraser.


* Segmentation mode will enable Superpixel segmentation. Each superpixel can be filled (or erased) with a single click.
* Brush mode will turn mouse-pointer into a brush (or eraser)

Brush Settings:
1. Shape of brush can be round or square.
2. Radius of brush tool can be configured.


![Segmentation Config Controls](https://files.readme.io/c2fb0e7-SegmentationConfig.png)

**Actions**
1. Mouse Click -- add (or erase) a region to annotation.
2. Mouse Drag right -- add (or erase) segments traced by mouse drag in current annotation.


[![Segmentation with Brush & Eraser](https://i.ytimg.com/vi/xtrJhqoRjhg/hqdefault.jpg)](https://www.youtube.com/embed/xtrJhqoRjhg)



![Accuracy of Segmentation Tool](https://files.readme.io/4a708b3-Ptch2.gif)


# Freehand with Sculpter
Freehand Draw tool can be used with mouse to draw accurate freehand contour. 

## Add Freehand Annotation

* Click and drag mouse to start drawing.
* Drag the mouse to draw the shape.
* End the shape by releasing mouse. 

## Edit using Sculpter: Region-Of-Interest

* Select "Enable Sculpter" to begin editing.
* The closer to the contour the mouse is, the smaller the tool will be.
* The tool can push from either the inside or the outside.
* With the mouse held down, drag the tool to push the Region-of-Interest.
* New points will be created and deleted as needed.
* Release the mouse to complete the edit.
* You may find you wish to make rough edits with a large tool, before making fine adjustments with a finer tool.

[![Freehand: Sculpt Accurate Shape](https://i.ytimg.com/vi/sllO1nw_LpI/hqdefault.jpg)](https://www.youtube.com/embed/sllO1nw_LpI)



![Freehand Annotation](https://files.readme.io/5a79857-Freehand.png)


# Polygon Tool
Polygon Tool is most versatile tool for adding new labels and editing existing labels. 

## Add a Polygon

* Click to draw a point.
* Keep clicking to draw a shape.
* End the shape by connecting it to the origin node without crossing any lines.

[![Polygon: Add New Polygon](https://i.ytimg.com/vi/5VgMAKn7DFs/hqdefault.jpg)](https://www.youtube.com/embed/5VgMAKn7DFs)



## Edit a Polygon



## Delete a Vertex

* *Ctrl-Click* on a handle to delete it.


## Add New Vertex

* *Ctrl-click* on a line to insert a new handle.

## Move a Vertex

* Release Ctrl and drag a handle to move it.

[![Polygon: Edit](https://i.ytimg.com/vi/2W7Sg8yxnH8/hqdefault.jpg)](https://www.youtube.com/embed/2W7Sg8yxnH8)



![Polygon  Annotation](https://files.readme.io/9c94020-PolygonTool.png)

# Magnify
While performing any annotation task, users may want to see a Region-Of-Interest on the image at a high magnification level. Magnify tool enables users to see ROI at a very high magnification level.

## How to use Magnification Tool

To use the magnification tool, select "Magnify" Button in the top toolbar.

![Magnify Button](https://files.readme.io/1d8a12d-Magnify.png)



## Left-Mouse-Button

Hold down left-mouse-button at the Region-of-interest (ROI).

![How To Magnify?](https://files.readme.io/3bc0bc4-HowToMagnify_-_Edited.gif)

# 2D Growth Tool for DICOM
2D growth tool ONLY works for DICOM (radiology) files
2D growth tool grows region based on HU value and pixel-distance

## Configuration

Configure: **Growth range in HU**
Configure: **Distance in Pixel**
If you enter -30 to 30 HU with 10 pixel radius, when you click on a pixel, growth tool will select all pixels within 10 pixel radius, that have HU value in -30 to +30 range with relative to HU value of selected pixel. If HU value of selected pixel is 450, all pixels within 10 pixel radius in 420 - 480 HU values, will be selected.

## Video



[![2DGrowthExample](https://i.ytimg.com/vi/-LV3co2EFtM/hqdefault.jpg)](https://www.youtube.com/watch?v=-LV3co2EFtM&feature=youtu.be)



## Accuracy



![Accuracy of 3D Growth compared to Desktop Tools](https://files.readme.io/7194b7c-HighAccuracyRadiology.gif)



![Comparison](https://files.readme.io/baa1179-HighPrecision.png)

# Labeling Instructions


# KeyBoard Shortcuts- Productivity

## Why do you need shortcuts?

Keyboard shortcuts can enhance productivity of annotators very significantly. Annotation tasks are very repetitive in nature, requiring same actions to be performed again and again. Keyboard shortcuts help human-labelers reach actions to be performed very fast.

## How to add Keyboard Shortcuts?

Here is how you add keyboard shortcuts:
1. Select "Label Configuration"
2. Create new or Edit a Labeling Interface
3. Click on Text entry "Assign Keyboard shortcut"
4. Enter keyboard shortcut on you keyboard (for example SHIFT+N)

![How to Add Keyboard Shortcuts](https://files.readme.io/a33ce0c-KeyBoardShortcuts.gif)



## For Annotators: How to View Keyboard Shortcuts?

Click "Information" icon on top right corner of the screen (as shown in image below).

![How to view keyboard ShortCuts.](https://files.readme.io/28c108d-KeyboardShortcuts.png)


# Labeling Instruction Builder

## What is a Labeling Instruction?

In order to give labeling task to freelance annotators, data science team needs to define specifications of a labeling task. Those specifications need to be converted to a user-experience. In TrainingData.io application specification builder is called labeling instruction. Labeling instruction is a list of objects that a data-scientist wants human-labelers to find in an image. Objects can have properties like color, size, shape etc. Data-scientist wants to present these properties in question-and-answer HTML form to the annotator.

Labeling instruction has two parts to it. Left panel and right panel. The left panel shows list of classes, their attributes and image-attributes. The right-panel shows how annotation-user-experience appear to the annotator (exactly). 

![Sample Labeling Instruction](https://files.readme.io/4413682-LabelingInstruction1.png)



## How to create a new Labeling Instruction?

As you add a class or an attribute on left panel, you will observe same class and attributes will show up on the right panel in real time. 

[![LabelingInterface Example](https://i.ytimg.com/vi/Z1ZYpmFLaRc/hqdefault.jpg)](https://www.youtube.com/watch?v=Z1ZYpmFLaRc&feature=youtu.be)



## Step 1: Creating First Class-Type

Classes are abstract-representation of real world objects that machine learning model learns about. Each class can have a:
1. Name: Associated real world object-class (like a car)
2. Color
3. Tool to be used to draw each object-instance belonging to that class
4. Sub-attributes are the properties of that class type

![New Class-type](https://files.readme.io/bea51e7-CarPolygon.png)



[![Create First Class](https://i.ytimg.com/vi/wc6oD7ZWCVo/hqdefault.jpg)](https://www.youtube.com/embed/wc6oD7ZWCVo)



## Step 2: Adding Attributes to Class-Type

Attributes define properties of real world objects. A simple example is color of car is a property of that car. Data scientists would want to know these properties, so that they can use it to train machines that make decision.  

An attribute is a question that you ask an annotator. There are four different data-types of an attribute:
1. Text: alphanumeric data entry
2. Multi-select Checkbox: a list of check boxes with multi-select functionality
3. Single-select Drop down list: with single select functionality
4. Single-select Radio button: with single selection functionality

[![Add Class Attribute](https://i.ytimg.com/vi/3glJI8KxZng/hqdefault.jpg)](https://www.youtube.com/embed/3glJI8KxZng)



## Step 3: Final Labeling Interface

After adding all classes and attributes to a labelling interface, a complete labelling interface will look like this:

![New Attribute](https://files.readme.io/de94b8b-LabelingInterface.png)

# AI Assisted Annotation


# Segmentation of Liver

## Segmentation of Liver using NVIDIA Clara Backend



[![AI Assisted Liver Segmentation](https://i.ytimg.com/vi/t3rXegVVTE4/hqdefault.jpg)](https://www.youtube.com/watch?v=t3rXegVVTE4&feature=youtu.be)

# Segmentation of Spleen

## Segmentation of Spleen using NVIDIA Clara



[![AI Assisted Spleen Segmentation](https://i.ytimg.com/vi/giFBUSsmJyE/hqdefault.jpg)](https://www.youtube.com/watch?v=giFBUSsmJyE&feature=youtu.be)


## 

# DataSet


# Create a Dataset
Datasets can be hosted in multiple locations. Location of datasets can be following:
1. A dataset can be local to your intranet (accessible to outside world over a VPN connection) 
2. A dataset can be hosted on your cloud, or your AWS S3, your Google Firebase storage, your Azure account.
3. A dataset can be uploaded to TrainingData.io's cloud storage. We use AWS S3.

## 1. Add New On-Prem Dataset with CSV File Upload

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


[![Local Dataset using CSV File Upload - Edited](https://i.ytimg.com/vi/rJK58Ed3kAg/hqdefault.jpg)](https://www.youtube.com/watch?v=rJK58Ed3kAg&feature=youtu.be)



## 2. Add New On-Prem Dataset with Folder Upload

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

[![Create Local Dataset using "Upload Folder" Local - Edited](https://i.ytimg.com/vi/dPe4nCOB9Y4/hqdefault.jpg)](https://www.youtube.com/watch?v=dPe4nCOB9Y4&feature=youtu.be)



## 3. Upload Archive: zip or tar to TD.io's Cloud Storage

Alternatively, you can upload an archive:
1. Add new dataset
2. Select "Remote"
3. Enter a name for the dataset
4. Click "Upload Files"
5. Select an archive of files and folders (recursive folder structure preserved with image files)
6. Select "Submit"
Individual image files will be uploaded to TD.io's cloud storage. Folder structure will be preserved exactly as given in archive.

[![Archive (zip) Dataset - Edited](https://i.ytimg.com/vi/WbTMiDM2b2M/hqdefault.jpg)](https://www.youtube.com/watch?v=WbTMiDM2b2M&feature=youtu.be)



## 4. Upload Individual Files and Folders to TD.io's Cloud

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

## 5. Upload Video Files to TD.io's Cloud

Alternatively, you can upload video files to TD.io's Cloud:
1. Add new dataset
2. Select "Remote"
3. Enter a name for the dataset
4. Click "Upload Files"
5. Select "Upload Files" and select individual video files (mov, avi) 
6. Inspect video files to be uploaded
8. Select "Submit"
Video files will be broken down into individual frames by TD.io's cloud system

[![Video File Upload](https://i.ytimg.com/vi/Dvd2DtY1j9s/hqdefault.jpg)](https://www.youtube.com/watch?v=Dvd2DtY1j9s&feature=youtu.be)



## 6. Upload CSV File with Self Hosted-Cloud URLs

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


[![Self Hosted Cloud Dataset](https://i.ytimg.com/vi/p8wubMrjpKw/hqdefault.jpg)](https://www.youtube.com/watch?v=p8wubMrjpKw&feature=youtu.be)



## Supported File Formats

TrainingData.io application standard image annotating interface supports the following image file formats.
PNG
JPEG
BMP
DCM
TAR
ZIP
GZ
# Delete a Dataset
Click on the three dots at right end of the Dataset and you will get delete option. Click on same to delete dataset

![Delete DataSet](https://files.readme.io/ef68532-DeleteDataset.png)





# Projects


# Add New Project

## What is a Project, and how is it different from Dataset?

A project is a collection of dataset and collaborators working on the project as annotators or reviewers. 
1. Login to your account
2. Select "Add Project"
3. Enter a name for the new project
4. Click "Next"
5. Attach a dataset to the project (only one dataset is allowed)
6. Click "Next"
7. Attach a labelling interface to the project
8. Click "Complete Setup"

[![Add New Project with Cloud Hosted Dataset](https://i.ytimg.com/vi/i6lhM3HGWTU/hqdefault.jpg)](https://www.youtube.com/watch?v=i6lhM3HGWTU&feature=youtu.be)



![Add Project Name](https://files.readme.io/e287b82-Project1.png)



![Project - Attach a Dataset](https://files.readme.io/365fb02-Project2.png)


![Project - Attach a Labeling Instruction](https://files.readme.io/0cbe3d5-Project3.png)

# Start Annotation
To start annotating click on any project entry. You will be taken to the workplace where you can create new annotations.

![Start Labeling](https://files.readme.io/4c5eeb2-StartLabeling.gif)

# Collaborators


# Add Collaborators to a Specific Project
Select a project from the Projects tab. This will open project settings. Under "Collaborators" sub tab, click "Add a Collaborator". Enter email address of new collaborator, enter role of new collaborator. Role of a collaborator can be "Admin", "Annotator", or "Reviewer".

Click "Add" to finish.

[![Add Collaborator](https://i.ytimg.com/vi/2ZUXOUe30n0/hqdefault.jpg)](https://www.youtube.com/embed/2ZUXOUe30n0)

# Add a Collaborator
A Collaborator is an individual who works on your labeling task. Collaborators can be your teammates at work, or people in other teams like data-science team, product team, devops team, legal team. Collaborators can also be individuals outside your organization like freelance annotators who would do annotation-work requiring skills not available in your organization.

## How do I Add a New Collaborator to My Organization?

Login to your account

Select "Collaborator" tab

Select "Add Collaborator"

Enter email address of new collaborator

Select Roles as "Project Based"

List of all your projects will populate

Now set role of this new collaborator for each individual project

[![New Collaborator Project Based](https://i.ytimg.com/vi/IfDn_GWWQ1w/hqdefault.jpg)](https://www.youtube.com/embed/IfDn_GWWQ1w)



## How do I Add Collaborator With Same Role for All Projects?

Login to your account

Select "Collaborator" tab

Select "Add Collaborator"

Enter email address of new collaborator

Select Role as "Admin" or "Annotator" or "Reviewer"

This new user will have same role for all projects.

## How to Remove a Collaborator?

Login to your account

Select "Collaborator" tab

For the collaborator to be removed, set role to "Select Role"

This collaborator will no more have access to your projects.
# Collaborators

## Why do you need collaborators?

Deep learning requires millions of images as input. Task of labeling millions of images requires many individuals. These individuals might be freelancers, and they might be located in distant locations. A data-science team needs to engage freelance workforce to complete their tasks.

The Collaborator feature allows data-science team to invite individuals to help with a labeling project. If multiple users are collaborating on an annotating project, TrainingData.io application distributes all of the data attached to a project to the collaborators with access. Collaborators will only get unique data, meaning there will not be multiple annotators annotating the same data.

## Roles

**Annotator**
The Annotator role can annotate queued data and view their own work from the Activity Table. An annotator cannot view annotators performance or view/modify any aspect of the project configuration or data sources.

**Reviewer**
The Reviewer role extends the annotator role by being able to see and review all annotated data in the project.

**Admin**
The Admin role can add and edit projects, data and Annotators. By default, the user that signs up for an account has the role of Admin.

**Project Based Roles**
 When a user is given a project based role, they don't have access to projects by default. However, the user is granted access to each project with a specific role and the role of each project can be changed. The benefit of this is that you can limit the access and the role of a user depending on the project at your discretion.

# Workspace


# Active Viewport Image (middle)
Active Viewport shows the current image on which a user is creating annotations.

![Viewport](https://files.readme.io/38146cd-Viewport.png)

# Folder Navigation (left)
TrainingData.io workspace allows you to partition your dataset into folders for easy navigation. We advice you to have two levels of folders for easy navigation. As shown in image below, first image in the folder will be used for Thumbnail.

![](https://files.readme.io/94a0873-Folders.png)

# Label Data (right)
Label settings include step-by-step walk through of questionnaire that annotator needs to answer for each label created.

## Navigation

Navigation includes left arrow and right arrow. Left arrow will change image in viewport to previous image in the selected folder. Right arrow will change image in view port  to the next image in the folder. 

Counter shows current index of the image in folder.

![Right Panel with Form](https://files.readme.io/221db3c-RightPanel.png)



## Class Names and Count of Labels

Each class name is represented by a box and a count of number of labels for that particular class.

## Form Data for Classes and Their Attributes

Each class has associated form-data that needs to be populated by the annotator.

Some parts of form-data might be "required", i.e. they are mandatory.

If annotator tries to save an annotation without entering "required" data entry, an error will be flashed as shown in image below:

![Error Prompt when trying to save annotation with incomplete form data.](https://files.readme.io/119f6c3-Error.png)

# ToolBar (top)
Toolbar on the top has four sections.

**Section One and Two: Image Placement**
Following features allow easy accessibility of different sections of the image: Zoom in, Zoom out, Pan
Following features allow you to pixel level detail of the image. In case of PNG or Jpeg you can see RGB values at each pixel, in case of DICOM image format you can see HU value.


**Section Three: Annotation Tools**
Draw tool allows free hand drawing as shown in image below

![Draw Tool](https://files.readme.io/19a0433-DrawTool.gif)

Rectangle tool can be used to create **bounding box** annotations.

## Freehand Drawing Tool

**Freehand Tool** can be used to create freehand annotations as shown in figure below

![Freehand Tool](https://files.readme.io/03563da-FreeHand_Tool.gif)



## Segmentation Tool

 
**Pixel Level Accuracy**
**PNG and JPEG**: Segmentation tool provides superpixel segmentation based on color. Segmentation tool works for JPG and PNG image formats.
https://youtu.be/l8XL_b4SIyk

[![Segmentation Tool](https://i.ytimg.com/vi/l8XL_b4SIyk/hqdefault.jpg)](https://www.youtube.com/embed/l8XL_b4SIyk)




## 3D Growth Tool

For **DICOM** format: 2D growth and 3D growth works based on HU value (Hounsfield Unit). It grows the region based on HU value within a specified pixel-radius. Video below shows how to create pixel-accurate annotations at very fast pace.
https://youtu.be/EkKbQQctLfA

[![3D Growth Tool Using HU Value](https://i.ytimg.com/vi/EkKbQQctLfA/hqdefault.jpg)](https://www.youtube.com/embed/EkKbQQctLfA)

**Section Four: Window Level**
Contrast: Set contrast of image
Brightness: Set brightness in the image
Window level: Select one of the following presets: Abdominal soft tissue, Bone, Brain, Brain Marrow, Liver, Lung, Subdural Brain

**Section Five: Layouts**
TrianingData.io workspace allows upto 4 folders to be viewed at the same time. In "Layout" menu options user can select 1x2, 2x1 or 2x2 mode to view upto 4 folders in same viewport. This allows for easy comparison of images.

**Stack Scroll**
For DICOM image format if more than one folder is in viewport, stack scroll will be automatically enabled as shown in image below 

![Stack Scroll](https://files.readme.io/8e61c3a-StackScroll.png)
# Terms and Conditions


# Privacy Policy
Privacy Policy

Effective date: January 1, 2019

We at TrainingData know you care about how your personal information is used and shared, and we take your privacy seriously. Please read the following to learn more about our Privacy Policy. By using or accessing the Services in any manner, you acknowledge that you accept the practices and policies outlined in this Privacy Policy, and you hereby consent that we will collect, use, and share your information in the following ways. Remember that your use of TrainingData’s Services is at all times subject to the Terms of Use, which incorporates this Privacy Policy. Any terms we use in this Policy without defining them have the definitions given to them in the Terms of Use.

What does this Privacy Policy cover?

This Privacy Policy covers our treatment of personally identifiable information ("Personal Information") that we gather when you are accessing or using our Services, but not to the practices of companies we don’t own or control, or people that we don’t manage. We gather various types of Personal Information from our users, as explained in more detail below, and we use this Personal Information internally in connection with our Services, including to personalize, provide, and improve our services, to allow you to set up a user account and profile, to contact you and allow other users to contact you, to fulfill your requests for certain products and services, and to analyze how you use the Services. In certain cases, we may also share some Personal Information with third parties, but only as described below. As noted in the Terms of Use, we do not knowingly collect or solicit personal information from anyone under the age of 13. If you are under 13, please do not attempt to register for the Services or send any personal information about yourself to us. If we learn that we have collected personal information from a child under age 13, we will delete that information as quickly as possible. If you believe that a child under 13 may have provided us personal information, please contact us at support@TrainingData.io

Will TrainingData ever change this Privacy Policy?

We’re constantly trying to improve our Services, so we may need to change this Privacy Policy from time to time as well, but we will alert you to changes by placing a notice on the Services, by sending you an email, and/or by some other means. Please note that if you’ve opted not to receive legal notice emails from us (or you haven’t provided us with your email address), those legal notices will still govern your use of the Services, and you are still responsible for reading and understanding them. If you use the Services after any changes to the Privacy Policy have been posted, that means you agree to all of the changes.

What Information does TrainingData Collect?

Information You Provide to Us:

We receive and store any information you knowingly provide to us. For example, through the registration process and/or through your account settings, we may collect Personal Information such as your name, email address, phone number, and third-party account credentials (for example,

your log-in credentials for Facebook or other third party sites). If you provide your third-party account credentials to us or otherwise sign in to the Services through a third party site or service, you understand some content and/or information in those accounts (“Third Party Account Information”) may be transmitted into your account with us if you authorize such transmissions], and that Third Party Account Information transmitted to our Services is covered by this Privacy Policy; for example, your public profile information from Facebook. Certain information may be required to register with us or to take advantage of some of our features.

We may communicate with you if you’ve provided us the means to do so. For example, if you’ve given us your email address, we may send you promotional email offers on behalf of other businesses, or email you about your use of the Services. Also, we may receive a confirmation when you open an email from us. This confirmation helps us make our communications with you more interesting and improve our services. If you do not want to receive communications from us, please indicate your preference by emailing us at support@TrainingData.io.

Information Collected Automatically

Whenever you interact with our Services, we automatically receive and record information on our server logs from your browser or device, which may include your IP address, geolocation data, device identification, “cookie” information, the type of browser and/or device you’re using to access our Services, and the page or feature you requested. “Cookies” are identifiers we transfer to your browser or device that allow us to recognize your browser or device and tell us how and when pages and features in our Services are visited and by how many people. You may be able to change the preferences on your browser or device to prevent or limit your device’s acceptance of cookies, but this may prevent you from taking advantage of some of our features. Our advertising partners may also transmit cookies to your browser or device, when you click on ads that appear on the Services. Also, if you click on a link to a third party website or service, such third party may also transmit cookies to you. Again, this Privacy Policy does not cover the use of cookies by any third parties, and we aren’t responsible for their privacy policies and practices. Please be aware that cookies placed by third parties may continue to track your activities online even after you have left our Services, and those third parties may not honor “Do Not Track” requests you have set using your browser or device.

We may use this data to customize content for you that we think you might like, based on your usage patterns. We may also use it to improve the Services - for example, this data can tell us how often users use a particular feature of the Services, and we can use that knowledge to make the Services interesting to as many users as possible.

Information Collected From Other Websites and Do Not Track Policy

Through cookies we place on your browser or device, we may collect information about your online activity after you leave our Services. Just like any other usage information we collect, this information allows us to improve the Services and customize your online experience, and otherwise as described in this Privacy Policy. Your browser may offer you a “Do Not Track” option, which allows you to signal to operators of websites and web applications and services (including behavioral advertising services) that you do not wish such operators to track certain of your online activities over time and across different websites. Our Services do not support Do Not Track requests at this time, which means that we collect information about your online activity both while you are using the Services and after you leave our Services.

Will TrainingData Share Any of the Personal Information it Receives?

We may share your Personal Information with third parties as described in this below:

Information that’s been de-identified. We may de-identify your Personal Information so that you are not identified as an individual, and provide that information to our partners. We may also provide aggregate usage information to our partners (or allow partners to collect that information from you), who may use such information to understand how often and in what ways people use our Services, so that they, too, can provide you with an optimal online experience. However, we never disclose aggregate usage or de-identified information to a partner (or allow a partner to collect such information) in a manner that would identify you as an individual.

Analytics: We may use third party analytics services, such as Google Analytics, to grow our business, to improve and develop our Services, to monitor and analyze use of our Services, to aid our technical administration, to increase the functionality and user-friendliness of our Services, and to verify that users have the authorization needed for us to process their requests. These services may collect and retain some information about you. Google Analytics collects the IP address assigned to you on the date you use the Services, but not your name or other personally identifying information. We do not combine the information generated through the use of Google Analytics with your Personal Information. Although Google Analytics plants a persistent cookie on your web browser to identify you as a unique user the next time you use the Services, the cookie cannot be used by anyone but Google. Google’s ability to use and share information collected by Google Analytics about your use of the Services is restricted by the Google Analytics Terms of Use and the Google Privacy Policy. You may find additional information about Google Analytics at www.google.com/policies/privacy/partners/. Finally, you can opt out of Google Analytics by visiting https://tools.google.com/dlpage/gaoptout/.

Advertisers: We allow advertisers and/or merchant partners (“Advertisers”) to choose the demographic information of users who will see their advertisements and/or promotional offers and you agree that we may provide any of the information we have collected from you in non-personally identifiable form to an Advertiser, in order for that Advertiser to select the appropriate audience for those advertisements and/or offers. For example, we might use the fact you are located in San Francisco to show you ads or offers for San Francisco businesses, but we will not tell such businesses who you are. Or, we might allow Advertisers to display their ads to users with similar usage patterns to yours, but we will not disclose usage information to Advertisers except in aggregate form, and not in a manner that would identify you personally. Note that if an advertiser asks us to show an ad to a certain audience or audience segment and you respond to that ad, the advertiser may conclude that you fit the description of the audience they were trying to reach.

We may deliver a file to you through the Services (known as a “web beacon”) from an ad network. Web beacons allow ad networks to provide anonymized, aggregated auditing, research and reporting for us and for advertisers. Web beacons also enable ad networks to serve targeted advertisements to you when you visit other websites. Because your web browser must request these advertisements and web beacons from the ad network’s servers, these companies can view, edit, or set their own cookies, just as if you had requested a web page from their site. You may be able to opt-out of web beacon tracking conducted by third parties through our Services by adjusting the Do Not Track settings on your browser; please note that we don’t control whether or how these third parties comply with Do Not Track requests.

Affiliated Businesses: In certain situations, businesses or third party websites we’re affiliated with may sell or provide products or services to you through or in connection with the Services (either

alone or jointly with us). You can recognize when an affiliated business is associated with such a transaction or service, and we will share your Personal Information with that affiliated business only to the extent that it is related to such transaction or service. One such service may include the ability for you to automatically transmit Third Party Account Information to your Services profile or to automatically transmit information in your Services profile to your third party account; for example, transmitting your public profile information from Facebook. We have no control over the policies and practices of third party websites or businesses as to privacy or anything else, so if you choose to take part in any transaction or service relating to an affiliated website or business, please review all such business’ or websites’ policies.

Our Agents: We employ other companies and people to perform tasks on our behalf and need to share your information with them to provide products or services to you; for example, we may use a payment processing company to receive and process your credit card transactions for us. Unless we tell you differently, our agents do not have any right to use the Personal Information we share with them beyond what is necessary to assist us. Note that an “agent” may also be considered a “partner” in certain circumstances, and may be subject to the terms of the “Information that’s been de-identified” section above in that regard.

User Profiles and Submissions: Certain user profile information, including your name, location, and any video or image content that such user has uploaded to the Services, may be displayed to other users to facilitate user interaction within the Services or address your request for our services. Your account privacy settings may allow you to limit the other users who can see the Personal Information in your user profile and/or what information in your user profile is visible to others.] Please remember that any content you upload to your public user profile, along with any Personal Information or content that you voluntarily disclose online in a manner other users can view (on discussion boards, in messages and chat areas, etc.) becomes publicly available, and can be collected and used by anyone. Your user name may also be displayed to other users if and when you send messages or comments or upload images or videos through the Services and other users can contact you through messages and comments.

Business Transfers: We may choose to buy or sell assets, and may share and/or transfer customer information in connection with the evaluation of and entry into such transactions. Also, if we (or our assets) are acquired, or if we go out of business, enter bankruptcy, or go through some other change of control, Personal Information could be one of the assets transferred to or acquired by a third party.

Protection of TrainingData and Others: We reserve the right to access, read, preserve, and disclose any information that we believe is necessary to comply with law or court order; enforce or apply our Terms of Use and other agreements; or protect the rights, property, or safety of TrainingData, our employees, our users, or others.

Is Personal Information about me secure?

Your account is protected by a password for your privacy and security. If you access your account via a third party site or service, you may have additional or different sign-on protections via that third party site or service. You must prevent unauthorized access to your account and Personal Information by selecting and protecting your password and/or other sign-on mechanism appropriately and limiting access to your computer or device and browser by signing off after you have finished accessing your account.

We endeavor to protect the privacy of your account and other Personal Information we hold in our records, but unfortunately, we cannot guarantee complete security. Unauthorized entry or use, hardware or software failure, and other factors, may compromise the security of user information at any time.

TrainingData is based in the United States and the information we collect is governed by U.S. law. By accessing or using the TrainingData Services or otherwise providing information to us, you consent to the processing and transfer of information in and to the U.S. and other countries.

What Personal Information can I access?

Through your account settings, you may access, and, in some cases, edit or delete the following information you’ve provided to us:

· name and password

· email address

· location

· phone number

· user profile information, including images and videos you have uploaded to the site.

The information you can view, update, and delete may change as the Services change. If you have any questions about viewing or updating information we have on file about you, please contact us at support@TrainingData.io.

Under California Civil Code Sections 1798.83-1798.84, California residents are entitled to contact us to prevent disclosure of Personal Information to third parties for such third parties’ direct marketing purposes; in order to submit such a request, please contact us at support@TrainingData.io.

What choices do I have?

You can always opt not to disclose information to us, but keep in mind some information may be needed to register with us or to take advantage of some of our features.

You may be able to add, update, or delete information as explained above. When you update information, however, we may maintain a copy of the unrevised information in our records. You may request deletion of your account by contacting us at support@TrainingData.io. Some information may remain in our records after your deletion of such information from your account. We may use any aggregated data derived from or incorporating your Personal Information after you update or delete it, but not in a manner that would identify you personally.

What if I have questions about this policy?

If you have any questions or concerns regarding our privacy policies, please send us a detailed message to support@TrainingData.io and we will try to resolve your concerns.
# Terms of Use
PLEASE NOTE THAT YOUR USE OF AND ACCESS TO OUR SERVICES (DEFINED BELOW) ARE SUBJECT TO THE FOLLOWING TERMS; IF YOU DO NOT AGREE TO ALL OF THE FOLLOWING, YOU MAY NOT USE OR ACCESS THE SERVICES IN ANY MANNER.

Terms of Use

Effective date: January 1, 2019

Welcome to www.TrainingData.io. Please read on to learn the rules and restrictions that govern your use of our website(s), products, services and applications (the “Services”). If you have any questions, comments, or concerns regarding these terms or the Services, please contact us at support@TrainingData.io.

These Terms of Use (the “Terms”) are a binding contract between you and TrainingData, Inc.. (“TrainingData,” “we” and “us”). You must agree to and accept all of the Terms, or you don’t have the right to use the Services. Your using the Services in any way means that you agree to all of these Terms, and these Terms will remain in effect while you use the Services. These Terms include the provisions in this document, as well as those in the Privacy Policy and Copyright Dispute Policy.

NOTICE: Please read these Terms carefully. They cover important information about Services provided to you and any charges, taxes, and fees we bill you. These Terms include information about future changes to these Terms, automatic renewals , limitations of liability, a class action waiver, and resolution of disputes by arbitration instead of in court.

Will these Terms ever change?

We are constantly trying to improve our Services, so these Terms may need to change along with the Services. We reserve the right to change the Terms at any time, but if we do, we will bring it to your attention by placing a notice on the www.TrainingData.io website, by sending you an email, and/or by some other means.

If you don’t agree with the new Terms, you are free to reject them; unfortunately, that means you will no longer be able to use the Services. If you use the Services in any way after a change to the Terms is effective, that means you agree to all of the changes.

Except for changes by us as described here, no other amendment or modification of these Terms will be effective unless in writing and signed by both you and us.

What about my privacy?

TrainingData takes the privacy of its users very seriously. For the current TrainingData Privacy Policy, please click here

The Children’s Online Privacy Protection Act (“COPPA”) requires that online service providers obtain parental consent before they knowingly collect personally identifiable information online from children who are under 13. We do not knowingly collect or solicit personally identifiable information from children under 13; if you are a child under 13, please do not attempt to register for the Services or send any personal information about yourself to us. If we learn we have collected personal information from a child under 13, we will delete that information as quickly as possible. If you believe that a child under 13 may have provided us personal information, please contact us at support@TrainingData.io.

What are the basics of using www.TrainingData.io?

You may be required to sign up for an account, and select a password and user name (“TrainingData User ID”). You promise to provide us with accurate, complete, and updated registration information about yourself. You may not select as your TrainingData User ID a name that you don’t have the right to use, or another person’s name with the intent to impersonate that person. You may not transfer your account to anyone else without our prior written permission.

You represent and warrant that you are of legal age to form a binding contract (or if not, you’ve received your parent’s or guardian’s permission to use the Services and gotten your parent or guardian to agree to these Terms on your behalf). If you’re agreeing to these Terms on behalf of an organization or entity, you represent and warrant that you are authorized to agree to these Terms on that organization or entity’s behalf and bind them to these Terms (in which case, the references to “you” and “your” in these Terms, except for in this sentence, refer to that organization or entity).

You will only use the Services for your own internal, personal, non-commercial use, and not on behalf of or for the benefit of any third party, and only in a manner that complies with all laws that apply to you. If your use of the Services is prohibited by applicable laws, then you aren’t authorized to use the Services. We can’t and won’t be responsible for your using the Services in a way that breaks the law.

You will not share your account or password with anyone, and you must protect the security of your account and your password. You’re responsible for any activity associated with your account.

Your use of the Services is subject to the following additional restrictions:

You represent, warrant, and agree that you will not contribute any Content or User Submission (each of those terms is defined below) or otherwise use the Services or interact with the Services in a manner that:

(a) Infringes or violates the intellectual property rights or any other rights of anyone else (including TrainingData);

(b) Violates any law or regulation, including, without limitation, any applicable export control laws;

(c) Is harmful, fraudulent, deceptive, threatening, harassing, defamatory, obscene, or otherwise objectionable;

(d) Jeopardizes the security of your TrainingData account or anyone else’s (such as allowing someone else to log in to the Services as you);

(e) Attempts, in any manner, to obtain the password, account, or other security information from any other user;

(f) Violates the security of any computer network, or cracks any passwords or security encryption codes;

(g) Runs Maillist, Listserv, any form of auto-responder or “spam” on the Services, or any processes that run or are activated while you are not logged into the Services, or that otherwise interfere with the proper working of the Services (including by placing an unreasonable load on the Services’ infrastructure);

(h) “Crawls,” “scrapes,” or “spiders” any page, data, or portion of or relating to the Services or Content (through use of manual or automated means);

(i) Copies or stores any significant portion of the Content;

(j) Decompiles, reverse engineers, or otherwise attempts to obtain the source code or underlying ideas or information of or relating to the Services.

A violation of any of the foregoing is grounds for termination of your right to use or access the Services.

What are my rights in the Services?

The materials displayed or performed or available on or through the Services, including, but not limited to, text, graphics, data, articles, photos, images, illustrations, User Submissions, and so forth (all of the foregoing, the “Content”) are protected by copyright and/or other intellectual property laws. You promise to abide by all copyright notices, trademark rules, information, and restrictions contained in any Content you access through the Services, and you won’t use, copy, reproduce, modify, translate, publish, broadcast, transmit, distribute, perform, upload, display, license, sell, commercialize or otherwise exploit for any purpose any Content not owned by you, (i) without the prior consent of the owner of that Content or (ii) in a way that violates someone else’s (including TrainingData’s) rights.

You understand that TrainingData owns the Services. You won’t modify, publish, transmit, participate in the transfer or sale of, reproduce (except as expressly provided in this Section), create derivative works based on, or otherwise exploit any of the Services.

The Services may allow you to copy or download certain Content; please remember that just because this functionality exists, doesn’t mean that all the restrictions above don’t apply – they do!

Do I have to grant any licenses to TrainingData or to other users?

Anything you post, upload, share, store, or otherwise provide through the Services is your “User Submission.” Some User Submissions may be viewable by other users. In order to display your User Submissions on the Services, and to allow other users to enjoy them (where applicable), you grant us certain rights in those User Submissions. Please note that all of the following licenses are subject to our Privacy Policy to the extent they relate to User Submissions that are also your personally-identifiable information.

For all User Submissions, you hereby grant TrainingData a license to translate, modify (for technical purposes, for example making sure your content is viewable on an iPhone as well as a computer) and reproduce and otherwise act with respect to such User Submissions, in each case to enable us to operate the Services, as described in more detail below. This is a license only – your ownership in User Submissions is not affected.

If you store a User Submission in your own personal TrainingData account, in a manner that is not viewable by any other user except you (a “Personal User Submission”), you grant TrainingData the license above, as well as a license to display, perform, and distribute your Personal User Submission for the sole purpose of making that Personal User Submission accessible to you and providing the Services necessary to do so.

If you share a User Submission only in a manner that only certain specified users can view (for example, a private message to one or more other users)(a “Limited Audience User Submission”), then you grant TrainingData the licenses above, as well as a license to display, perform, and distribute your Limited Audience User Submission for the sole purpose of making that Limited Audience User Submission accessible to such other specified users, and providing the Services necessary to do so. Also, you grant such other specified users a license to access that Limited Audience User Submission, and to use and exercise all rights in it, as permitted by the functionality of the Services.

If you share a User Submission publicly on the Services and/or in a manner that more than just you or certain specified users can view[, or if you provide us (in a direct email or otherwise) with any feedback, suggestions, improvements, enhancements, and/or feature requests relating to the Services] (each of the foregoing, a “Public User Submission”), then you grant TrainingData the licenses above, as well as a license to display, perform, and distribute your Public User Submission for the purpose of making that Public User Submission accessible to all TrainingData users and providing the Services necessary to do so, as well as all other rights necessary to use and exercise all rights in that Public User Submission in connection with the Services and/or otherwise in connection with TrainingData’s business for any purpose, provided that

TrainingData will try to notify you if it uses your Public User Submission for any reason other than displaying it on the Services]. Also, you grant all other users of the Services a license to access that Public User Submission, and to use and exercise all rights in it, as permitted by the functionality of the Services.

You agree that the licenses you grant are royalty-free, perpetual, sublicenseable, irrevocable, and worldwide, provided that when you delete your TrainingData account, we will stop displaying your User Submissions (other than Public User Submissions, which may remain fully available)] to other users (if applicable), but you understand and agree that it may not be possible to completely delete that content from TrainingData’s records, and that your User Submissions may remain viewable elsewhere to the extent that they were copied or stored by other users.

Finally, you understand and agree that TrainingData, in performing the required technical steps to provide the Services to our users (including you), may need to make changes to your User Submissions to conform and adapt those User Submissions to the technical requirements of connection networks, devices, services, or media, and the foregoing licenses include the rights to do so.

What if I see something on the Services that infringes my copyright?

You may have heard of the Digital Millennium Copyright Act (the “DMCA”), as it relates to online service providers, like TrainingData, being asked to remove material that allegedly violates someone’s copyright. We respect others’ intellectual property rights, and we reserve the right to delete or disable Content alleged to be infringing, and to terminate the accounts of repeat alleged infringers; to review our complete Copyright Dispute Policy and learn how to report potentially infringing content,. To learn more about the DMCA, click here.

Who is responsible for what I see and do on the Services?

Any information or content publicly posted or privately transmitted through the Services is the sole responsibility of the person from whom such content originated, and you access all such information and content at your own risk, and we aren’t liable for any errors or omissions in that information or content or for any damages or loss you might suffer in connection with it. We cannot control and have no duty to take any action regarding how you may interpret and use the Content or what actions you may take as a result of having been exposed to the Content, and you hereby release us from all liability for you having acquired or not acquired Content through the Services. We can’t guarantee the identity of any users with whom you interact in using the Services and are not responsible for which users gain access to the Services.

You are responsible for all Content you contribute, in any manner, to the Services, and you represent and warrant you have all rights necessary to do so, in the manner in which you contribute it. You will keep all your registration information accurate and current. You are responsible for all your activity in connection with the Services.

The Services may contain links or connections to third party websites or services that are not owned or controlled by TrainingData. When you access third party websites or use third party services, you accept that there are risks in doing so, and that TrainingData is not responsible for such risks. We encourage you to be aware when you leave the Services and to read the terms and conditions and privacy policy of each third party website or service that you visit or utilize.

TrainingData has no control over, and assumes no responsibility for, the content, accuracy, privacy policies, or practices of or opinions expressed in any third party websites or by any third party that you interact with through the Services. In addition, TrainingData will not and cannot monitor, verify, censor or edit the content of any third party site or service. By using the Services, you release and hold us harmless from any and all liability arising from your use of any third party website or service.

Your interactions with organizations and/or individuals found on or through the Services, including payment and delivery of goods or services, and any other terms, conditions, warranties or representations associated with such dealings, are solely between you and such organizations and/or individuals. You should make whatever investigation you feel necessary or appropriate before proceeding with any online or offline transaction with any of these third parties. You agree that TrainingData shall not be responsible or liable for any loss or damage of any sort incurred as the result of any such dealings.

If there is a dispute between participants on this site, or between users and any third party, you agree that TrainingData is under no obligation to become involved. In the event that you have a dispute with one or more other users, you release TrainingData, its officers, employees, agents, and successors from claims, demands, and damages of every kind or nature, known or unknown, suspected or unsuspected, disclosed or undisclosed, arising out of or in any way related to such disputes and/or our Services. If you are a California resident, you shall and hereby do waive California Civil Code Section 1542, which says: "A general release does not extend to claims which the creditor does not know or suspect to exist in his favor at the time of executing the release, which, if known by him must have materially affected his settlement with the debtor."

Will TrainingData ever change the Services?

We’re always trying to improve the Services, so they may change over time. We may suspend or discontinue any part of the Services, or we may introduce new features or impose limits on certain features or restrict access to parts or all of the Services. We reserve the right to remove any Content from the Services at any time, for any reason (including, but not limited to, if someone alleges you contributed that Content in violation of these Terms), in our sole discretion, and without notice.

Do the Services cost anything?

The Services are currently free, but we reserve the right to charge for certain or all Services in the future. We will notify you before any Services you are then using begin carrying a fee, and if you wish to continue using such Services, you must pay all applicable fees for such Services.

What if I want to stop using the Services? You’re free to do that at any time, by contacting us at support@TrainingData.io; please refer to our Privacy Policy, as well as the licenses above, to understand how we treat information you provide to us after you have stopped using our Services.

TrainingData is also free to terminate (or suspend access to) your use of the Services or your account, for any reason in our discretion, including your breach of these Terms. TrainingData has the sole right to decide whether you are in violation of any of the restrictions set forth in these Terms.

Account termination may result in destruction of any Content associated with your account, so keep that in mind before you decide to terminate your account.

Provisions that, by their nature, should survive termination of these Terms shall survive termination. By way of example, all of the following will survive termination: any obligation you have to pay us or indemnify us, any limitations on our liability, any terms regarding ownership or intellectual property rights, and terms regarding disputes between us, including without limitation the arbitration agreement.

What else do I need to know?

Warranty Disclaimer. Neither TrainingData nor its licensors or suppliers make any representations or warranties concerning any content contained in or accessed through the Services, and we will not be

responsible or liable for the accuracy, copyright compliance, legality, or decency of material contained in or accessed through the Services. We (and our licensors and suppliers) make no representations or warranties regarding suggestions or recommendations of services or products offered or purchased through the Services. Products and services purchased or offered (whether or not following such recommendations and suggestions) through the Services are provided “AS IS” and without any warranty of any kind from TrainingData or others (unless, with respect to such others only, provided expressly and unambiguously in writing by a designated third party for a specific product). THE SERVICES AND CONTENT ARE PROVIDED BY TrainingData (AND ITS LICENSORS AND SUPPLIERS) ON AN “AS-IS” BASIS, WITHOUT WARRANTIES OR ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT, OR THAT USE OF THE SERVICES WILL BE UNINTERRUPTED OR ERROR-FREE. SOME STATES DO NOT ALLOW LIMITATIONS ON HOW LONG AN IMPLIED WARRANTY LASTS, SO THE ABOVE LIMITATIONS MAY NOT APPLY TO YOU.

Limitation of Liability. TO THE FULLEST EXTENT ALLOWED BY APPLICABLE LAW, UNDER NO CIRCUMSTANCES AND UNDER NO LEGAL THEORY (INCLUDING, WITHOUT LIMITATION, TORT, CONTRACT, STRICT LIABILITY, OR OTHERWISE) SHALL TrainingData (OR ITS LICENSORS OR SUPPLIERS) BE LIABLE TO YOU OR TO ANY OTHER PERSON FOR (A) ANY INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES OF ANY KIND, INCLUDING DAMAGES FOR LOST PROFITS, LOSS OF GOODWILL, WORK STOPPAGE, ACCURACY OF RESULTS, OR COMPUTER FAILURE OR MALFUNCTION, OR (B) ANY AMOUNT, IN THE AGGREGATE, IN EXCESS OF THE GREATER OF (I) $100 OR (II) THE AMOUNTS PAID BY YOU TO TrainingData IN CONNECTION WITH THE SERVICES IN THE TWELVE (12) MONTH PERIOD PRECEDING THIS APPLICABLE CLAIM, OR (C) ANY MATTER BEYOND OUR REASONABLE CONTROL. SOME STATES DO NOT ALLOW THE EXCLUSION OR LIMITATION OF CERTAIN DAMAGES, SO THE ABOVE LIMITATION AND EXCLUSIONS MAY NOT APPLY TO YOU.

Indemnity. To the fullest extent allowed by applicable law,] You agree to indemnify and hold TrainingData, its affiliates, officers, agents, employees, and partners harmless from and against any and all claims, liabilities, damages (actual and consequential), losses and expenses (including attorneys’ fees) arising from or in any way related to any third party claims relating to (a) your use of the Services (including any actions taken by a third party using your account), and (b) your violation of these Terms. In the event of such a claim, suit, or action (“Claim”), we will attempt to provide notice of the Claim to the contact information we have for your account (provided that failure to deliver such notice shall not eliminate or reduce your indemnification obligations hereunder).

Assignment. You may not assign, delegate or transfer these Terms or your rights or obligations hereunder, or your Services account, in any way (by operation of law or otherwise) without TrainingData’s prior written consent. We may transfer, assign, or delegate these Terms and our rights and obligations without consent.

Choice of Law. These Terms are governed by and will be construed under the Federal Arbitration Act, applicable federal law, and the laws of the State of California, without regard to the conflicts of laws provisions thereof.

Arbitration Agreement. PLEASE READ THE FOLLOWING ARBITRATION AGREEMENT CAREFULLY BECAUSE IT REQUIRES YOU TO ARBITRATE CERTAIN DISPUTES AND CLAIMS WITH TrainingData AND LIMITS THE MANNER IN WHICH YOU CAN SEEK RELIEF FROM US. Both you and TrainingData acknowledge and agree that for the purposes of any dispute arising out of or relating to the subject matter of these Terms, TrainingData’s officers, directors, employees and independent contractors (“Personnel”) are third party beneficiaries of these Terms, and that upon your acceptance of

these Terms, Personnel will have the right (and will be deemed to have accepted the right) to enforce these Terms against you as the third party beneficiary hereof.

(a) Arbitration Rules; Applicability of Arbitration Agreement. Any dispute arising out of or relating to the subject matter of these Terms shall be finally settled by binding arbitration in San Francisco County, California. The arbitration will proceed in the English language, in accordance with the Streamlined Arbitration Rules and Procedures of Judicial Arbitration and Mediation Services, Inc. ("JAMS") then in effect, by one commercial arbitrator with substantial experience in resolving intellectual property and commercial contract disputes, who shall be selected from the appropriate list of JAMS arbitrators in accordance with such Rules. Judgment upon the award rendered by such arbitrator may be entered in any court of competent jurisdiction. Notwithstanding the foregoing obligation to arbitrate disputes, each party shall have the right to pursue injunctive or other equitable relief at any time, from any court of competent jurisdiction.

(b) Costs of Arbitration. The JAMS rules will govern payment of all arbitration fees. TrainingData will pay all arbitration fees for claims less than $75,000. TrainingData will not seek its attorneys’ fees and costs in arbitration unless the arbitrator determines that your claim is frivolous.

(c) Small Claims Court. Furthermore, either you or TrainingData may assert claims, if they qualify, in small claims court in San Francisco County, California or any United States county where you live or work.

(d) Waiver of Jury Trial. YOU AND TrainingData WAIVE ANY CONSTITUTIONAL AND STATUTORY RIGHTS TO GO TO COURT AND HAVE A TRIAL IN FORNT OF A JUDGE OR JURY. You and TrainingData are instead choosing to have claims and disputes resolved by arbitration. Arbitration procedures are typically more limited, more efficient, and less costly than rules applicable in court and are subject to very limited review by a court. In any litigation between you and TrainingData over whether to vacate or enforce an arbitration award, YOU AND TrainingData WAIVE ALL RIGHTS TO A JURY TRIAL, and elect instead to have the dispute be resolved by a judge.

(e) Waiver of Class or Consolidated Actions. ALL CLAIMS AND DISPUTES WITHIN THE SCOPE OF THIS ARBITRATION AGREEMENT MUST BE ARBITRATED OR LITGATED ON AN INDIVIDUAL BASIS AND NOT ON A CLASS BASIS. CLAIMS OF MORE THAN ONE CUSTOMER OR USER CANNOT BE ARBITRATED OR LITGATED JOINTLY OR CONSOLIDATED WITH THOSE OF ANY OTHER CUSTOMER OR USER. If however, this waiver of class or consolidated actions is deemed invalid or unenforceable, neither you nor we are entitled to arbitration; instead all claims and disputes will be resolved in a court as set forth in (g) below.

(f) Opt-out. You have the right to opt out of the provisions of this Section by sending written notice of your decision to opt out to the following address: 170 Capp Street, Suite A, SF, CA 94110 postmarked within 30 days of first accepting these Terms. You must include (1) your name and residence address; (2) the email address and/or telephone number associated with your account; and (3) a clear statement that you want to opt out of these Terms’ arbitration agreement.

(g) Exclusive Venue. If you send the opt-out notice in (f), and/or in any circumstances where the foregoing arbitration agreement permits either you or TrainingData to litigate any dispute arising out of or relating to the subject matter of these Terms in court, then the foregoing arbitration agreement will not apply to either party and both you and TrainingData agree that any judicial proceeding (other than small claims actions) will be brought in the state or federal courts located in, respectively, San Francisco County, California, or the Northern District of California.

Miscellaneous. You will be responsible for paying, withholding, filing, and reporting all taxes, duties, and other governmental assessments associated with your activity in connection with the Services, provided

that the TrainingData may, in its sole discretion, do any of the foregoing on your behalf or for itself as it sees fit. The failure of either you or us to exercise, in any way, any right herein shall not be deemed a waiver of any further rights hereunder. If any provision of these Terms is found to be unenforceable or invalid, that provision will be limited or eliminated, to the minimum extent necessary, so that these Terms shall otherwise remain in full force and effect and enforceable. You and TrainingData agree that these Terms are the complete and exclusive statement of the mutual understanding between you and TrainingData, and that these Terms supersede and cancel all previous written and oral agreements, communications and other understandings relating to the subject matter of these Terms,. You hereby acknowledge and agree that you are not an employee, agent, partner, or joint venture of TrainingData, and you do not have any authority of any kind to bind TrainingData in any respect whatsoever.

You and TrainingData agree there are no third party beneficiaries intended under these Terms.
