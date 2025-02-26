---
subcategory: "CloudWatch Logs"
layout: "aws"
page_title: "AWS: aws_cloudwatch_log_stream"
description: |-
  Provides a CloudWatch Log Stream resource.
---


<!-- Please do not edit this file, it is generated. -->
# Resource: aws_cloudwatch_log_stream

Provides a CloudWatch Log Stream resource.

## Example Usage

```typescript
// DO NOT EDIT. Code generated by 'cdktf convert' - Please report bugs at https://cdk.tf/bug
import { Construct } from "constructs";
import { TerraformStack } from "cdktf";
/*
 * Provider bindings are generated by running `cdktf get`.
 * See https://cdk.tf/provider-generation for more details.
 */
import { CloudwatchLogGroup } from "./.gen/providers/aws/cloudwatch-log-group";
import { CloudwatchLogStream } from "./.gen/providers/aws/cloudwatch-log-stream";
class MyConvertedCode extends TerraformStack {
  constructor(scope: Construct, name: string) {
    super(scope, name);
    const yada = new CloudwatchLogGroup(this, "yada", {
      name: "Yada",
    });
    new CloudwatchLogStream(this, "foo", {
      logGroupName: yada.name,
      name: "SampleLogStream1234",
    });
  }
}

```

## Argument Reference

This resource supports the following arguments:

* `name` - (Required) The name of the log stream. Must not be longer than 512 characters and must not contain `:`
* `logGroupName` - (Required) The name of the log group under which the log stream is to be created.

## Attribute Reference

This resource exports the following attributes in addition to the arguments above:

* `arn` - The Amazon Resource Name (ARN) specifying the log stream.

## Import

In Terraform v1.5.0 and later, use an [`import` block](https://developer.hashicorp.com/terraform/language/import) to import Cloudwatch Log Stream using the stream's `logGroupName` and `name`. For example:

```typescript
// DO NOT EDIT. Code generated by 'cdktf convert' - Please report bugs at https://cdk.tf/bug
import { Construct } from "constructs";
import { TerraformStack } from "cdktf";
class MyConvertedCode extends TerraformStack {
  constructor(scope: Construct, name: string) {
    super(scope, name);
  }
}

```

Using `terraform import`, import Cloudwatch Log Stream using the stream's `logGroupName` and `name`. For example:

```console
% terraform import aws_cloudwatch_log_stream.foo Yada:SampleLogStream1234
```

<!-- cache-key: cdktf-0.20.0 input-4fed32ff75bb830aa4a809d588a8fcccf96c6368ab7e6ad418f7d940ac65117d -->