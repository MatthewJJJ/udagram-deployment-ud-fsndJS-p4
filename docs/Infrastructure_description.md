### Udagram Infrastructure

Udagram is an AWS native application that can also be configured to run locally. Here are the different pieces of infrastructure that Udagram runs off of.

1. Database - AWS RDS Postgres
   - This database stores all of udagrams data in a structured format
2. Backend Hosting - AWS Elasticbeanstalk
   - AWS Elasticbeanstalk manages the deployment of the backend code which resides on virtual machines (EC2 instances) and other AWS infrastructure (security groups, etc.). Elasticbeanstalk manages all of this for us.
3. Frontend Hosting - AWS S3
   - S3 is AWS's simple storage service and hosts and serves all of the static frontend files for the angular app.

**Note: Udagram also utilizes a GitHub repo which stores the source code and tiggers a CircleCI pipeline that deploys the code to the different AWS resources**
