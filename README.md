repository:
  name: aws-resource-inventory
  description: "A shell scripting project that automates the process of listing all active resources in an AWS account using AWS CLI."
  author: "Aditya "
  files:
    README.md: |
      # AWS Resource Inventory Script

      A shell scripting project that automates the process of listing all active resources in an AWS account.  
      This is a simple yet powerful tool for **DevOps engineers** and **cloud administrators** to quickly discover resources across different AWS services.  

      ---

      ## 🎯 Project Overview
      This project is my **first shell scripting project** focused on **automation in DevOps**.  
      The script connects to AWS via the AWS CLI and lists resources for supported services in a given region.  

      🔹 Why this is useful:
      - Helps in **cost optimization** by discovering unused or forgotten resources.
      - Can be scheduled as a **cron job** for periodic monitoring.
      - Output can be redirected for **reporting or alerting** (e.g., email reports).

      ---

      ## 🚀 Features
      - Lists resources from multiple AWS services including:
        - EC2
        - RDS
        - S3
        - CloudFront
        - VPC
        - IAM
        - Route53
        - CloudWatch
        - CloudFormation
        - Lambda
        - SNS
        - SQS
        - DynamoDB
        - EBS
      - Uses only **AWS CLI** (no extra dependencies).
      - Clean error handling: checks for AWS CLI installation & configuration before running.
      - Easy-to-use command line interface.

      ---

      ## 📋 Prerequisites
      Before running the script, make sure you have:

      1. **unzip** installed  
         ```bash
         sudo apt-get install unzip -y
         ```

      2. **AWS CLI** installed  
         [Download AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)  

      3. **AWS CLI configured** with credentials  
         - Go to AWS Console → Click on your name → Security Credentials  
         - Create an **Access Key** (Access Key ID + Secret Access Key).  
         - Run:
           ```bash
           aws configure
           ```
         - Provide Access Key, Secret Key, Region, and Output format.

      ---

      ## ⚡ Usage
      ```bash
      ./aws_resource_list.sh <aws_region> <aws_service>
      ```

      ### Example:
      ```bash
      ./aws_resource_list.sh us-east-1 ec2
      ```
      This will list all EC2 instances in the `us-east-1` region.  
      You can replace the region and service as needed.

      ---

      ## 🛠️ Supported Services
      | Service       | Command Example                                |
      |---------------|-----------------------------------------------|
      | EC2           | `./aws_resource_list.sh us-east-1 ec2`        |
      | RDS           | `./aws_resource_list.sh us-east-1 rds`        |
      | S3            | `./aws_resource_list.sh us-east-1 s3`         |
      | CloudFront    | `./aws_resource_list.sh us-east-1 cloudfront` |
      | VPC           | `./aws_resource_list.sh us-east-1 vpc`        |
      | IAM           | `./aws_resource_list.sh us-east-1 iam`        |
      | Route53       | `./aws_resource_list.sh us-east-1 route53`    |
      | CloudWatch    | `./aws_resource_list.sh us-east-1 cloudwatch` |
      | CloudFormation| `./aws_resource_list.sh us-east-1 cloudformation` |
      | Lambda        | `./aws_resource_list.sh us-east-1 lambda`     |
      | SNS           | `./aws_resource_list.sh us-east-1 sns`        |
      | SQS           | `./aws_resource_list.sh us-east-1 sqs`        |
      | DynamoDB      | `./aws_resource_list.sh us-east-1 dynamodb`   |
      | EBS           | `./aws_resource_list.sh us-east-1 ebs`        |

      ---

      ## 📌 Notes
      - Some services like **S3** and **Route53** are **global services**, so the region flag may not apply.
      - You will find service-specific commands in the [AWS CLI Documentation](https://docs.aws.amazon.com/cli/).
      - Script can be extended to support **more AWS services**.

      ---

      ## 🔧 Future Enhancements
      - Add support for more AWS services.
      - Export results in **CSV/JSON format**.
      - Automate with **cron jobs** and send **email reports**.
      - Add **filtering options** (e.g., list only running EC2 instances).

      ---

      ## 🤝 Contributing
      Contributions are welcome!  
      Fork this repo and add support for additional AWS services or improve error handling.  

      ---

      ## 📜 License
      This project is licensed under the [MIT License](LICENSE).

      ---

      ## 👨‍💻 Author
      **Aditya (**  
      A passionate DevOps engineer in the making 🚀, exploring automation, cloud, and infrastructure tools.

    
