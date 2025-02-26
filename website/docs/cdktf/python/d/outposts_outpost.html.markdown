---
subcategory: "Outposts"
layout: "aws"
page_title: "AWS: aws_outposts_outpost"
description: |-
  Provides details about an Outposts Outpost
---


<!-- Please do not edit this file, it is generated. -->
# Data Source: aws_outposts_outpost

Provides details about an Outposts Outpost.

## Example Usage

```python
# DO NOT EDIT. Code generated by 'cdktf convert' - Please report bugs at https://cdk.tf/bug
from constructs import Construct
from cdktf import TerraformStack
#
# Provider bindings are generated by running `cdktf get`.
# See https://cdk.tf/provider-generation for more details.
#
from imports.aws.data_aws_outposts_outpost import DataAwsOutpostsOutpost
class MyConvertedCode(TerraformStack):
    def __init__(self, scope, name):
        super().__init__(scope, name)
        DataAwsOutpostsOutpost(self, "example",
            name="example"
        )
```

## Argument Reference

This data source supports the following arguments:

* `id` - (Optional) Identifier of the Outpost.
* `name` - (Optional) Name of the Outpost.
* `arn` - (Optional) ARN.
* `owner_id` - (Optional) AWS Account identifier of the Outpost owner.

## Attribute Reference

This data source exports the following attributes in addition to the arguments above:

* `availability_zone` - Availability Zone name.
* `availability_zone_id` - Availability Zone identifier.
* `description` - The description of the Outpost.
* `lifecycle_status` - The life cycle status.
* `site_arn` - The Amazon Resource Name (ARN) of the site.
* `site_id` - The ID of the site.
* `supported_hardware_type` - The hardware type.
* `tags` - The Outpost tags.

<!-- cache-key: cdktf-0.20.0 input-35f3fde745d0b61be013964ef1d616fef90704512a6afea84fcf8f9bf3c2acd5 -->