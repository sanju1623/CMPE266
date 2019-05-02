# CMPE266

University Name: http://www.sjsu.edu/

Course: Big Data Engineering and Analytics

Professor Sanjay Garje https://www.linkedin.com/in/sanjaygarje/

Public URL:
Face Analysis - 
https://sanju1623.github.io/CMPE266/

Face Authentication and Verification - 
https://my-static-site-example266code.herokuapp.com/

Team:

Hari Krishna Pariveda https://www.linkedin.com/in/harikrishnapariveda/
Sanjay Karnati https://www.linkedin.com/in/sanjaykarnati/
Sri Harsha Vanga 
Suvid Anand www.linkedin.com/in/suvid-anand
Varun Khatri https://www.linkedin.com/in/varun-khatri-9b8956107/

**Project Introduction**

The application that we are focusing on is a Dynamic advertisement delivery system in combination with a face-based authentication system. The main actuator of the project is a dynamic content deliverer which delivers personalized content to the user based on the facial, demographic and sentiment analysis of the user’s face. Amazon Rekognition API is a chief operator in this process, it performs all the aforementioned analysis on the captured user images and produces a result which can be used to make a decision on which advertisement to display. The decisioning logic decides which advertisement to display based on the results produced by Rekognition API. The data produced by Rekognition API is also stored for analytics purposes and to improve accuracy of future decisions based on the demographic data.

The image data is captured from a video feed, still frames are acquired from this video feed and as mentioned above, the image is analyzed using Amazon Rekognition API to produce results. This project makes use of various Amazon cloud services like S3, DynamoDB, Lambda. 


**Sample Demo Screenshots**

![image](https://user-images.githubusercontent.com/36252473/57069895-bc2f1680-6c8a-11e9-857f-bab6fe0f7249.png)

![image](https://user-images.githubusercontent.com/36252473/57069973-eed90f00-6c8a-11e9-916b-8df36b5be9d4.png)

![image](https://user-images.githubusercontent.com/36252473/57069995-fc8e9480-6c8a-11e9-86d2-a7fdc8fdfe59.png)

![image](https://user-images.githubusercontent.com/36252473/57070018-087a5680-6c8b-11e9-82f3-0cd360dd2554.png)


**Pre-requisites Set Up**

- **AWS S3** Bucket is used to store the images from video that were split into
frames.

- **AWS Lambda** functions are written for image processing which gets triggered
when an image is uploaded to S3 bucket.

- **Amazon Rekognition** service is used to identify objects, faces, celebrities etc
present in the images. This service provides an intelligent image and video
analysis based on deep learning.

- **AWS DynamoDB** is No-sql based database that is used to store the information
obtained from image processing using AWS Rekognition tool.

- **AWS API Gateway** is used to securely maintain and monitor the REST API’s.
These API’s can be used to access data or business logic running in EC2 or
AWS lambda service.

- **Node.js** is a Javascript runtime environment.It is an asynchronous single
threaded programming language that runs on based on an event loop.
