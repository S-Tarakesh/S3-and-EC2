## CLOUD-STORAGE-CREATION-S3-AND-LAUNCHING-AN-EC2-INSTANCE-IN-AWS-
# Aim
To create an Amazon S3 bucket for cloud storage and launch a virtual machine using Amazon EC2 in the AWS Management Console.
Objectives
After completing this experiment, students will be able to:
•	Understand AWS Cloud Storage (Amazon S3). 
•	Create and manage S3 buckets. 
•	Upload and organize files in cloud storage. 
•	Launch an EC2 virtual server. 
•	Connect to an EC2 instance. 
•	Understand cloud computing infrastructure services. 
Software Requirements
•	Laptop/Desktop 
•	Internet Connection 
•	AWS Academy Learner Account / AWS Free Tier Account 
•	Modern Web Browser (Chrome/Edge) 

# Theory
Amazon S3 (Simple Storage Service)
Amazon S3 is an object storage service provided by AWS that stores unlimited amounts of data with high durability and availability.
Features
•	Unlimited Storage 
•	99.999999999% (11 9's) durability 
•	High Availability 
•	Secure Storage 
•	Versioning 
•	Lifecycle Management 
•	Encryption
 
Part A – Creating an Amazon S3 Bucket
Step 1
Open the AWS console.
URL: https://aws.amazon.com/console/
Step 2
Log in using the following method:
•	Click Sign in using root user email. 
•	Enter the registered email address. 
•	Enter the AWS password. 
•	Complete the verification process. 
# Output

<img width="912" height="918" alt="Exp2 a" src="https://github.com/user-attachments/assets/79a17c88-8be7-4004-987f-a85361bf646e" />





Step 3
Type S3 in the search box.

Step 4
Click Amazon S3.
Step 5
Click Create bucket.

Step 6
Enter the following details.
Parameter	Value
Bucket type	General purpose
Bucket name	student-cloud-storage-001
AWS Region	Asia Pacific (Mumbai)

Step 7
Leave the remaining settings unchanged.
Step 8
Click Create bucket.
Step 9
Click Upload.
Step 10
Upload the following files:
•	PDF file 
•	Word document 
•	Image file 
Example
student-cloud-storage-001
│
├── Cloud.pdf
├── Assignment.docx
├── Image.jpg
└── Notes.pdf

# Part B – Launching an Amazon EC2 Instance
Step 1
Type EC2 in the AWS search bar.
Step 2
Open the EC2 Dashboard.
Step 3
Click Launch instance.
Step 4
Enter the instance name.
CloudLabVM

Step 5
Select the operating system.
•	Amazon Linux 2023 
•	Ubuntu Server 
Step 6
Select the instance type.
t3.micro

Step 7
Create a key pair.
Parameter	Value
Key pair name	CloudLabKey
Key pair type	RSA
File format	.pem

Step 8
Download the CloudLabKey.pem file.

Step 9
Configure the network settings.
Allow SSH traffic (Port 22)
Allow HTTP traffic (Port 80)
Allow HTTPS traffic (Port 443)
Step 10
Set the storage size.
8 GiB

Step 11
Click Launch instance.

Step 12
Wait until the status changes.
Pending
   ↓
Running

# Connecting to the EC2 Instance
Step 1
Open EC2.

Step 2
Select the instance.

Step 3
Click Connect.

Step 4
Select EC2 Instance Connect.

Step 5
Click Connect.

Step 6
Execute the following command:
echo "Hello AWS"

# Output
<img width="913" height="892" alt="Exp2 b" src="https://github.com/user-attachments/assets/147fad32-af34-487a-9c6f-7f7536a69ab2" />
<img width="908" height="963" alt="Exp2 c" src="https://github.com/user-attachments/assets/44dab691-bfee-4ea5-b459-0ab55eaa452f" />
<img width="918" height="971" alt="Exp2 c2" src="https://github.com/user-attachments/assets/27e9e7f1-5dfa-4999-8fc5-e232afb7af8b" />



Hello AWS

Stopping the EC2 Instance
Step 1
Open EC2.

Step 2
Select Instances.

Step 3
Select the running instance.

Step 4
Click Instance state.

Step 5
Click Stop instance.

Status
Running
   ↓
Stopping
   ↓
Stopped

Logging Out of AWS
1.	Click the profile icon in the upper-right corner. 
2.	Select Sign out. 

# Result
The Amazon S3 bucket was created successfully, files were uploaded, an EC2 instance was launched, and the virtual machine was connected successfully.

