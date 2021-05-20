## Intro to Amazon S3
- https://docs.aws.amazon.com/AmazonS3/latest/dev/Introduction.html 
- Simple Storage Service
- has a simple web services interface that can be used to store and retrieve any amout of data at any time anywhere 
- focuses on simplicity and robustness
  - Creating buckets – Create and name a bucket that stores data. Buckets are the fundamental containers in Amazon S3 for data storage.
  - Storing data – Store an infinite amount of data in a bucket. Upload as many objects as you like into an Amazon S3 bucket. Each object can contain up to 5 TB of data. Each object is stored and retrieved using a unique developer-assigned key.
  - Downloading data – Download your data or enable others to do so. Download your data anytime you like, or allow others to do the same.
  - Permissions – Grant or deny access to others who want to upload or download data into your Amazon S3 bucket. Grant upload and download permissions to three types of users. Authentication mechanisms can help keep data secure from unauthorized access.
  - Standard interfaces – Use standards-based REST and SOAP interfaces designed to work with any internet-development toolkit.
- Amazon S3 charges you only for what you actually use, with no hidden fees and no overage charges. This gives developers a variable-cost service that can grow with their business while enjoying the cost advantages of the AWS infrastructure.

## S3 with Amplify
- `amplify add storage`
- `amplify push`
- add libraries into the dependencies
- Initialize amplify storage
- upload data to your bucket.
