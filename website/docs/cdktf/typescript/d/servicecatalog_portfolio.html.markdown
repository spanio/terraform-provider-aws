---
subcategory: "Service Catalog"
layout: "aws"
page_title: "AWS: aws_servicecatalog_portfolio"
description: |-
  Provides information for a Service Catalog Portfolio.
---


<!-- Please do not edit this file, it is generated. -->
# Data Source: aws_servicecatalog_portfolio

Provides information for a Service Catalog Portfolio.

## Example Usage

```typescript
// DO NOT EDIT. Code generated by 'cdktf convert' - Please report bugs at https://cdk.tf/bug
import { Construct } from "constructs";
import { TerraformStack } from "cdktf";
/*
 * Provider bindings are generated by running `cdktf get`.
 * See https://cdk.tf/provider-generation for more details.
 */
import { DataAwsServicecatalogPortfolio } from "./.gen/providers/aws/data-aws-servicecatalog-portfolio";
class MyConvertedCode extends TerraformStack {
  constructor(scope: Construct, name: string) {
    super(scope, name);
    new DataAwsServicecatalogPortfolio(this, "portfolio", {
      id: "port-07052002",
    });
  }
}

```

## Argument Reference

The following arguments are required:

* `id` - (Required) Portfolio identifier.

The following arguments are optional:

* `acceptLanguage` - (Optional) Language code. Valid values: `en` (English), `jp` (Japanese), `zh` (Chinese). Default value is `en`.

## Attribute Reference

This data source exports the following attributes in addition to the arguments above:

* `arn` - Portfolio ARN.
* `createdTime` - Time the portfolio was created.
* `description` - Description of the portfolio
* `name` - Portfolio name.
* `providerName` - Name of the person or organization who owns the portfolio.
* `tags` - Tags applied to the portfolio.

<!-- cache-key: cdktf-0.20.0 input-84da50c0619f8efedfa9915aaeed7934ec932b8663c9afe0bb857f54d0d60299 -->