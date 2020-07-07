# General

aws configure
assign keys, default region, and default output format

# S3

aws s3 ls
list all objects in s3 bucket

aws s3 mb s3://{bucket_name}
makes a bucket of given name

aws s3 cp {filepath} {bucket_name}
uploads file to s3