This code is:
- a lambda transform function to attach to a firehose

Compared with the default lambda function, his lambda function sets a nice Splunk sourcetype based on the log group name.
For example, if the log group name contains ec2, then the splunk sourcetype will be aws:cloudwatchlogs:ec2
or, if the log group name contains rds then the sourcetype will be aws:cloudwatchlogs:rds

The code should be extended to support further log group types as they are discovered
