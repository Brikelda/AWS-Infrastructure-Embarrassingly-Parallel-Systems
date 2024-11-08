# AWS-Infrastructure-Embarrassingly-Parallel-Systems
This group project integrates embarrassingly parallel systems with AWS, where the Master EC2 instance splits the work evenly to 4 Worker EC2 instances.
The Master distributes the work into an S3 bucket, the workers take the tasks from the bucket, compute the work, and return the result into the bucket. 
The Master then polls the results from the bucket and combines them. This approach is very time-efficient and accurate.
