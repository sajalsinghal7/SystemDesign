## ### Problem Statement

Design architecture for an app described below using services from any cloud platform. This
architecture should follow 12 factor app guidelines. It should have data analytics capabilities and
monitoring of services as well.
The App is for sharing text, video and image based content, the content can be searched and is also
personalised and recommended by a machine learning service.


## ### Design

[![](https://github.com/sajalsinghal7/SystemDesign/blob/master/ImageSharing/ImageSharing.png)](https://github.com/sajalsinghal7/SystemDesign/blob/master/ImageSharing/ImageSharing.png)

## ### Architecture Explanation

##### Cloud platform
- AWS (Aussming this for our architecture)
- Azure

##### Data analytics capabilities 
- Cloud Watch Logs

##### Monitoring of services 
- Cloud Watch Logs
- ELK Stack

##### Sharing text, video and image based content
- Upload/Downloading/Deletion handled by File Service

##### Searching
- All user searches stored in Database for future search history
- Search history sent to recommendation system, so to identify user search behavior and update the exisiting keyword and models for user

##### Personalised and recommended data by a machine learning service
- On the basis of user searches, his data set is already updated so sending user its recommended data via recommendation service