# Required Providers

## Overview

The `required_providers` block in Terraform specifies the providers your configuration requires and their versions.

## Defining Required Providers

Here's how you can define required providers in your configuration:

```hcl
terraform {
  required_providers {
    aws = {
      source  = "hashicorp/aws"
      version = "~> 3.0"
    }
    azurerm = {
      source  = "hashicorp/azurerm"
      version = "~> 2.0"
    }
  }
}
```

## Updating Providers

To update providers, you can run:

```bash
terraform init -upgrade
```

## Conclusion

Specifying required providers ensures that your configuration uses compatible versions and avoids potential issues during deployment.



[Previous: Multiple Regions](03-multiple-regions.md) | [Next: Variables](05-variables.md) | [Back to README](README.md)
