# CLOUD-SPACE-STORAGE

**COMPANY**:  CODETECH IT SOLUTIONS

**NAME**:PRAGATHI P

**INTERN ID**:CT04DG1065

**DOMAIN**:Cloud Computing

**DURATION**: 4 WEEKS

**MENTOR**:Neela Santhosh Kumar

**Task Description: Creating and Configuring Cloud Storage on AWS S3**

The objective of this task was to create and configure a cloud storage solution using Amazon Web Services (AWS) Simple Storage Service (S3). The focus was on creating an S3 bucket named my-aws-viji, uploading example files into it, and setting appropriate access permissions to allow public access where necessary.

**Creating the S3 Bucket**

The process began by logging into the AWS Management Console and navigating to the S3 service. A new S3 bucket was created by selecting “Create bucket,” entering the unique name my-aws-viji, and choosing the appropriate region (in this case, Asia Pacific – Mumbai). During creation, most default settings were retained.
One critical section reviewed during setup was the Block Public Access settings, which AWS enables by default to prevent unintended public exposure of data. Since this task required that certain files be publicly accessible, these settings were adjusted in a later step.

**Uploading Files**

Once the my-aws-viji bucket was created, several files were uploaded as examples. These included images and documents selected from the local computer. The upload process was done using the S3 web interface, which allows drag-and-drop or file browsing options. After upload, the files appeared listed inside the bucket.

**Configuring Permissions**

To make the uploaded files accessible publicly, access permissions were configured both at the bucket level and for individual objects.
First, the Block Public Access settings for the bucket were edited. All four options were unchecked to allow access via policies and ACLs (Access Control Lists). These changes were saved after confirming the action.
Next, a bucket policy was added to allow public read access to all files within my-aws-viji. The policy was written in JSON format and granted anyone ("Principal": "*") the ability to perform the s3:GetObject action on all files within the bucket using the wildcard arn:aws:s3:::my-aws-viji/*.
Additionally, each uploaded file was individually configured through its Permissions tab. In the Access Control List (ACL) section, read permissions were granted to “Everyone,” enabling the file to be publicly viewable using its Object URL.

**Testing Access**

To verify that the setup was successful, the Object URL of one of the files was copied and pasted into a web browser. The file opened directly without requiring authentication, indicating that the public access settings were correctly applied.

**Troubleshooting**

During the process, an “Access Denied” error was encountered when attempting to open a file through its URL. This issue was caused by the default block public access settings conflicting with the bucket policy. After disabling the block settings and reapplying the bucket policy and ACL changes, the error was resolved.

**Conclusion**

This task provided practical experience in working with AWS S3, one of the most widely used cloud storage solutions. It involved creating a new bucket (my-aws-viji), uploading files, adjusting security permissions, and testing public access. Understanding how to manage access control in S3 is crucial for safely sharing or storing files in the cloud. This setup is now ready for further use in application development, file hosting, or integration with other AWS services.


**OUTPUT**

<img width="1440" alt="Image" src="https://github.com/user-attachments/assets/bc829472-e728-4e49-9a9e-ad1206312e8c" />

<img width="1440" alt="Image" src="https://github.com/user-attachments/assets/c1420624-aea4-4005-91a7-645cd84ec901" />

<img width="1439" alt="Image" src="https://github.com/user-attachments/assets/2c5996e2-5138-4289-993f-e967e1b7336f" />

<img width="1439" alt="Image" src="https://github.com/user-attachments/assets/bbc31526-c1d1-4749-b8b9-dbea0d00face" />

<img width="1438" alt="Image" src="https://github.com/user-attachments/assets/221737c2-2bd4-461f-9f81-8e26c74a8be6" />

<img width="1440" alt="Image" src="https://github.com/user-attachments/assets/082ddca0-5a6b-4b8d-817c-8767cc5f5084" />

<img width="1440" alt="Image" src="https://github.com/user-attachments/assets/27a6def4-814f-442a-9f14-af5c388c48f5" />
