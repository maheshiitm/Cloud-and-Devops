#Lambda Function to stop start ec2 instances

import boto3
region = 'us-west-1'
instances = ['i-12345cb6de4f78g9h', 'i-08ce9b2d7eccf6d26']
ec2 = boto3.client('ec2', region_name=region)

def lambda_handler(event, context):
    ec2.start_instances(InstanceIds=instances)
    print('started your instances: ' + str(instances))
	
	
	
construct the cron expression
https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-cron-expressions.html

Exercise 2 : 1. Deploy a sample java application in elastic beanstalk and test the url

Exercise 3: https://catalog.us-east-1.prod.workshops.aws/workshops/f3a3e2bd-e1d5-49de-b8e6-dac361842e76/en-US/basic-modules/40-monitoring/monitoring/1-monitoring

Exercise 4: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/quickref-s3.html#scenario-s3-bucket-website

