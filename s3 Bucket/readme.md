# S3 BUCKET PREP

## Step 1: Upload Templates to S3

- Upload Templates to S3 Bucket
- Go to the AWS Management Console.
- Navigate to the S3 service.
- Create a new bucket or use an existing one.
- Upload your templates (security-group.yaml, jenkins-instance.yaml, sonarqube-instance.yaml, nexus-instance.yaml) to the bucket.

- Add a Bucket Policy
    - Go to the "Permissions" tab.
    - Click on "Bucket Policy" and add the following JSON policy. Replace YOUR_BUCKET_NAME with the name of your S3 bucket.

[S3-BUCKET-POLICY](./bucket-policy.json)

This policy allows the CloudFormation service to read objects from your bucket. Note that this example policy grants read access to all objects within the specified bucket to the CloudFormation service.

