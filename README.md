# **Backup Service to Google Drive**☁️🔒
## **Overview**
Creating a Backup service that periodically backup the contents of a folder to **Google Drive using Docker and Kubernets**. The service ensures that the files are securely backed up and managed without redundancy.

## **Features**
- **📦 Backup Service**: Automates the backup of files and folders to Google Drive.
- **🔄 Periodic Backups**: Utilizes Kubernetes CronJobs to schedule regular backups.
- **🗃️ Redundancy Elimination**: Maintains a single copy of each file in Google Drive to avoid redundancy.
- **✅ User Notifications**: Provides appropriate messages if a file or folder already exists in Google Drive.
  
## **Tech Stack**
<p align="center">
  <img src="https://img.icons8.com/color/48/000000/docker.png" alt="Docker" width="40" height="40"/>
  <img src="https://img.icons8.com/color/48/000000/kubernetes.png" alt="Kubernetes" width="40" height="40"/>
  <img src="https://img.icons8.com/color/48/000000/google-drive.png" alt="Google Drive API" width="40" height="40"/>
  <img src="https://img.icons8.com/color/48/000000/python.png" alt="Python" width="40" height="40"/>
</p>

- **Docker**: For containerizing the backup application.
- **Kubernetes**: For orchestrating and managing the backup service.
- **Google Drive API**: For interacting with Google Drive.
- **Python Libraries**: For scripting and API interactions.

## **Implementation**
**[Week-1:](https://github.com/gantasrilaitha/Back-Up-Service-using-Docker-and-Kubernetes-CloudComputing/tree/main/week1)**
Contains Dockerfile & backup script that performs google-drive-authentication and fetches top-10 most recently used files from Google Drive.

**[Week-2:](https://github.com/gantasrilaitha/Back-Up-Service-using-Docker-and-Kubernetes-CloudComputing/tree/main/week2)**
Implemented Backup service using Kubernets Cronjob and PVC. A file/folder can be uploaded to drive, maintaining its single copy in drive, thus,eliminating redundancy.
Appropriate message shown to user if file/folder aldready exists in drive.
