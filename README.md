Availability zones are data centres, there are atleast 2 or 3 in each region. multi AAC availablility zone.There are physical az(availability zones). When working with clients from other locations, you have to deploy to the nearest availability zone for where the app is meant to be. AWS created a GovCloud, only NASA and other government sectors have access to that cloud.

scale out means t2 micro, more servers of of the same type and size.

scale up increasing the size of the server. It is done when when you are working towards a minimum requirement, because you can't scale out before the minimum requirements is met.

What is aws cli??? 

 aws s3 ls lists all s3 buckets available.(Buckets are storage in the cloud)

trello stores images on the aws s3 bucket

s3 bucket has a naming convention(certain character's like '_' and capital letters can't be used)
- `sudo apt-get install python`
- `python --version`
- `sudo apt-get install python-pip -y`
- `sudo apt-get install awscli`
- `aws configure`
- `aws s3 ls`
- `aws s3 mb s3://devops-bootcamp-abdul-bucket` - Makes bucket
- `sudo nano devops_bootcamp_test.text`
- `cat devops_bootcamp_test.text`
- `aws s3 cp test_file.txt s3://devops-bootcamp-abdul-bucket` - sends file to bucket
- `rm devops_bootcamp_test.text`
- `aws s3 sync s3://devops-bootcamp-abdul-bucket/ devops_bootcamp_test.text`
-  `cat devops_bootcamp_test.text/`
- `aws s3 rm s3://devops-bootcamp-abdul-bucket/devops_bootcamp_test.text`
- `aws s3 rb s3://devops-bootcamp-abdul-bucket`



s3 storage class are frequently used non frequently used(s3 glacier) lower charges, have to give 24 hours notice, not immediately available.
