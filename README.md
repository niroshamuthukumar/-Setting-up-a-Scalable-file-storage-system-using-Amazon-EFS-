 # SETTING UP A SCALABLE FILE STORAGE SYSTEM USING AMAZON ELASTIC FILE SYSTEM
 NAME: gayathri m
 REG NO:212223220024
  ## AIM
       To  setting up a scalable file storage system using Amazon Elastic File System (EFS) for two EC2 instances in different availability zones. 
## PROBLEM STATEMENT
    Explain about the Experiment.

## ALGORITHM
 ### Steps 1: Create two EC2 instances in different availability zones.
 ### Steps 2: Set up a security group that allows necessary communication between the instances and EFS.
 ### Steps 3: Create an EFS file system and mount it to both EC2 instances.
 ### Steps 4: Ensure that the EC2 instances can access the file system and share data between them.

## COMMANDS
## EC2 Instance 1
```
sudo su
yum install httpd -y
yum install -y amazon-efs-utils
mount -t efs -o tls fs-064645ac116a12816:/ /var/www/html
cd /var/www/html
vi file  # Create a file and add some text
```
## EC2 Instance 2
```
sudo su
yum install httpd -y
yum install -y amazon-efs-utils
mount -t efs -o tls fs-064645ac116a12816:/ /var/www/html
cd /var/www/html
ls
cat file  
```
## OUTPUT
![cc efs](https://github.com/user-attachments/assets/a8dc5954-b5e1-4c22-bd92-38d3f5088ad2)

![Screenshot (20)](https://github.com/user-attachments/assets/630ca823-6b2b-4909-b17b-617ddf596071)

![Screenshot (19)](https://github.com/user-attachments/assets/c239a039-a48f-4be2-b61c-2c70cd2eed76)

![Screenshot (18)](https://github.com/user-attachments/assets/1c7a8044-d7cc-4ce8-991d-3a95743c2eb2)

![Screenshot (17)](https://github.com/user-attachments/assets/eadd4798-ed10-415c-92a9-bd3774156c1e)

 
## RESULT
 Thus, The setting up a scalable file storage system using Amazon Elastic File System (EFS) for two EC2 instances in different availability zones, enabling shared access to data is executed successfully.

  


