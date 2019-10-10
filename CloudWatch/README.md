# Reference
 https://docs.aws.amazon.com/health/latest/ug/cloudwatch-events-health.html
 
You can use Amazon CloudWatch Events to detect and react to changes in the status of AWS Personal Health Dashboard (AWS Health) events. Then, based on the rules that you create, CloudWatch Events invokes one or more target actions when an event matches the values that you specify in a rule. Depending on the type of event, you can send notifications, capture event information, take corrective action, initiate events, or take other actions. You can select the following types of targets when using CloudWatch Events as a part of your AWS Health workflow:

##  AWS Lambda functions
## Kinesis streams
## Amazon SQS queues
## Built-in targets (CloudWatch alarm actions)
## Amazon SNS topics

The following are some use cases:
## Use a Lambda function to pass a notification to a Slack channel when an event occurs.
## Send custom text or SMS notifications with Amazon SNS when an AWS Health event happens by using Lambda and CloudWatch Events. 