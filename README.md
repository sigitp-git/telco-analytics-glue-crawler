# telco-analytics-glue-crawler

1. Execute telco-analytics.yaml using CloudFormation Console or CLI
2. Acknowledge that IAM Role will be created by the CloudFormation Console
3. Once CloudFormation template executed, go to AWS Glue Console
4. On the Crawler Tab, choose the "cfn-crawler-telco-analytics" and Run the crawler
5. Once the "cfn-crawler-telco-analytics" crawler finished running, the "cfn-database-telco-analytics" database is filled with the tables from rawdata
