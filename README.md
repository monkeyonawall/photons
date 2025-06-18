# Photons

__Author:__ Stunt Muncher

__Last Updated:__ June 17, 2025

## Introduction
Welcome to Photons! A low cost solution to backup your photos on Google Cloud. Photons integrates directly with Google Cloud without any intermediator. You get complete control and transparency of your data.

## Why?
As of June 17, 2025, “Google One” charges $19.99/year for 100 GB [[1](https://one.google.com/about/plans)] and “Google Cloud” charges $0.01/month per 1 GB in Oregon for “Nearline storage” [[2](https://cloud.google.com/storage/pricing)]. This means storing the same 100 GB on “Google Cloud” will cost $12/year. A potential savings of $7.99/year. 

In contrast, “Google One” charges $99.99/year for 2 TB [[1](https://one.google.com/about/plans)]. The same 2 TB on “Google Cloud” in Oregon for “Nearline storage” will cost $240/year. I recommend switching to “Google One” if you fall into this category.

“Google Cloud” will charge additional fees outside of storage costs like read/write operations. Photons relies on a configuration that is stored in your Cloud Bucket to keep track of metadata of your photos and provide the user interface experience in the app that will incur additional costs outside of your photos. Cost and prices will vary based on configuration, experience, and Google Cloud’s policies. Please defer to Google’s public documentation for the latest on their pricing structure. 

## How to Set Up?

Follow the steps below to set up Photons:

1. Create a Google Cloud Account: https://cloud.google.com/docs/get-started. 
1. Create a Cloud Project: https://developers.google.com/workspace/guides/create-project 
1. Create a Cloud Bucket: https://cloud.google.com/storage/docs/creating-buckets#console 
1. Create a Service Account: https://cloud.google.com/iam/docs/service-accounts-create#creating 
1. Create a Service Account key and download the JSON file: https://cloud.google.com/iam/docs/keys-create-delete#creating. Avoid sharing the JSON files with others unless you want them to access your Cloud Bucket.
1. Add the Service Account as Storage Admin to your Cloud Bucket: https://cloud.google.com/storage/docs/access-control/using-iam-permissions
1. Send the JSON to your phone such that you can upload it in Photons.
1. Open Photons, input the name of your Cloud Bucket, and click “Upload API” and select the JSON file of the Service Account key. 
1. You're set!
