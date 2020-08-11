# 

# telco-analytics-glue-crawler

1. Execute telco-analytics.yaml using CloudFormation Console or CLI
2. Acknowledge that IAM Role will be created by the CloudFormation Console
3. Once CloudFormation template executed, go to AWS Glue Console
4. On the Crawler Tab, choose the "cfn-crawler-telco-analytics" and Run the crawler
5. Once the "cfn-crawler-telco-analytics" crawler finished running, the "cfn-database-telco-analytics" database is filled with the tables from rawdata



***Note:*** if you don't have access to the default S3 bucket provided on line **143** of **telco-analytics.yaml**:

```yaml
- Path: "s3://serverless-analytics/telco-data-analytics-blog/"
```

Please download the rawdata.csv from: https://serverless-analytics.s3.amazonaws.com/telco-data-analytics-blog/rawdata.csv, then upload it on your own S3 bucket and update line **143** of **telco-analytics.yaml**:

```yaml
- Path: "s3://your-own-bucket-name/rawdata.csv"
```

Please keep in mind that the S3 bucket and your Amazon Athena/QuickSight must be in the same AWS Region. 



