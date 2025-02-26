---
subcategory: "Audit Manager"
layout: "aws"
page_title: "AWS: aws_auditmanager_framework_share"
description: |-
  Terraform resource for managing an AWS Audit Manager Framework Share.
---


<!-- Please do not edit this file, it is generated. -->
# Resource: aws_auditmanager_framework_share

Terraform resource for managing an AWS Audit Manager Framework Share.

## Example Usage

### Basic Usage

```typescript
// DO NOT EDIT. Code generated by 'cdktf convert' - Please report bugs at https://cdk.tf/bug
import { Construct } from "constructs";
import { Token, TerraformStack } from "cdktf";
/*
 * Provider bindings are generated by running `cdktf get`.
 * See https://cdk.tf/provider-generation for more details.
 */
import { AuditmanagerFrameworkShare } from "./.gen/providers/aws/auditmanager-framework-share";
class MyConvertedCode extends TerraformStack {
  constructor(scope: Construct, name: string) {
    super(scope, name);
    new AuditmanagerFrameworkShare(this, "example", {
      destinationAccount: "012345678901",
      destinationRegion: "us-east-1",
      frameworkId: Token.asString(awsAuditmanagerFrameworkExample.id),
    });
  }
}

```

## Argument Reference

The following arguments are required:

* `destinationAccount` - (Required) Amazon Web Services account of the recipient.
* `destinationRegion` - (Required) Amazon Web Services region of the recipient.
* `frameworkId` - (Required) Unique identifier for the shared custom framework.

The following arguments are optional:

* `comment` - (Optional) Comment from the sender about the share request.

## Attribute Reference

This resource exports the following attributes in addition to the arguments above:

* `id` - Unique identifier for the share request.
* `status` -  Status of the share request.

## Import

In Terraform v1.5.0 and later, use an [`import` block](https://developer.hashicorp.com/terraform/language/import) to import Audit Manager Framework Share using the `id`. For example:

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

Using `terraform import`, import Audit Manager Framework Share using the `id`. For example:

```console
% terraform import aws_auditmanager_framework_share.example abcdef-123456
```

<!-- cache-key: cdktf-0.20.0 input-14d7a2ed97dee3206ec0e19704aeaa2d131932ec24b406ef4fff013eeb7c1aba -->