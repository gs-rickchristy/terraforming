# Terraforming

Export existing AWS resources to [Terraform](https://terraform.io/) style (tf, tfstate)

## Prerequisites

- [AWS Command Line Interface (awscli)](http://aws.amazon.com/cli/?nc2=h_ls)

## Usage

### ELB

```bash
$ aws elb describe-load-balancers | terraforming-elb [--tfstate]
```

### RDS

```bash
$ aws rds describe-db-instances | terraforming-rds [--tfstate]
```

### S3

```bash
$ aws s3api list-buckets | terraforming-s3 [--tfstate]
```

### Security Group

```bash
$ aws ec2 describe-security-groups | terraforming-sg [--tfstate]
```

### VPC

```bash
$ aws ec2 describe-vpcs | terraforming-vpc [--tfstate]
```