# Deploy your CloudFormation Master Stack using the AWS Management Console

Using a master template simplifies the process by creating all resources in a single step.

## Step 1: Prepare the Master Template

Ensure your master-template.yaml is set up correctly with the appropriate S3 URLs and parameter references.

## Step 2: Deploy the Master Template
- Go to the CloudFormation service in the AWS Management Console.
- Click on "Create stack" and then select "With new resources (standard)".
- Select "Template is ready" and then "Amazon S3 URL".
- Enter the S3 URL of your master-template.yaml template (e.g., https://s3.amazonaws.com/your-bucket-name/master-template.yaml).
- Click "Next".
- Specify a stack name, e.g., MasterStack.
- Under Parameters, enter:
    - InstanceType: t2.medium (or your desired instance type)
    - KeyName: your-key-name
- Click "Next", configure any additional options as needed, and click "Next" again.
- Review your settings and click "Create stack".

By using the master template, you can deploy all the required resources in one go, simplifying the process and ensuring all dependencies are correctly managed.