# ECR Scan Saver

This cloudformation template creates ECR Repository, EventBridge, Lambda function and S3 bucket to save ECR image scan results to S3 Bucket.
- ECR repository which on-push scan is enabled, you can name your repository using the **RepositoryName** parameter.
- EventBridge will connect your repository and lambda function to trigger lambda function when image scanning is completed.
- Lambda function will retrieve the latest scan result and store that on a private S3 bucket that you will name using **BucketName** parameter.

For more information regarding ECR container image scanning and this setup, you can check https://www.sufle.io/blog/xxxxxxa
