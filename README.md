# Terraform S3 Module

## Overview:
This Terraform module creates an S3 bucket as well as an IAM user and key with access to the bucket.

---

#### Required Inputs:
  * name - S3 Bucket name.  This name will also be used create the IAM user.

---

#### Module Outputs:
  * iam_access_key_id - IAM access key
  * iam_access_key_secret - IAM access secret


## Examples:

```bash
module "s3" {
  source = "github.com/mondorobot/terraform-s3"

  name = "S3-bucket-name"
}
```
