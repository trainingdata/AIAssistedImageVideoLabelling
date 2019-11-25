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

## How do I host a local dataset?

This can be achieved in many different ways:

1. You can host a local dataset using any commercial grade NAS device.
2. You can use any of the open source media servers like Plex with [REST API interface](https://docs.google.com/document/d/19bTQr99oKn2pOpHcVtqidokbq9zup-K-mFy8JmII6uQ/edit?usp=sharing).

A comprehensive guide to hosting image files and video files can be found [here](https://www.theguardian.com/technology/askjack/2014/jul/31/how-do-i-set-up-a-media-server-to-share-photos-with-phones-and-tablets).


## [How do I access and manage local datasets in TrainingData.io application](https://docs.trainingdata.io/v1.0/DataSet/Create%20On-Prem%20Dataset/)
