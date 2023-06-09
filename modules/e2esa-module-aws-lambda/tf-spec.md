## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | ~> 1.4.2 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | ~> 4.5.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | ~> 4.5.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_cloudwatch_log_group.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_log_group) | resource |
| [aws_iam_role.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_lambda_alias.test_lambda_alias](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_alias) | resource |
| [aws_lambda_function.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_aws_region"></a> [aws\_region](#input\_aws\_region) | AWS infrastructure region | `string` | `null` | no |
| <a name="input_lambda_alias_name"></a> [lambda\_alias\_name](#input\_lambda\_alias\_name) | lambda\_alias\_name | `string` | `""` | no |
| <a name="input_lambda_filename_zip"></a> [lambda\_filename\_zip](#input\_lambda\_filename\_zip) | filename zip name | `string` | `"null"` | no |
| <a name="input_lambda_func_current_version"></a> [lambda\_func\_current\_version](#input\_lambda\_func\_current\_version) | lambda\_func\_current\_version | `string` | `""` | no |
| <a name="input_lambda_func_target_version"></a> [lambda\_func\_target\_version](#input\_lambda\_func\_target\_version) | lambda\_func\_target\_version | `string` | `""` | no |
| <a name="input_lambda_function_name"></a> [lambda\_function\_name](#input\_lambda\_function\_name) | function\_name | `string` | `"null"` | no |
| <a name="input_lambda_handler"></a> [lambda\_handler](#input\_lambda\_handler) | handler name | `string` | `"index.test"` | no |
| <a name="input_lambda_role_arn"></a> [lambda\_role\_arn](#input\_lambda\_role\_arn) | lambda\_role\_arn | `string` | `""` | no |
| <a name="input_lambda_runtime"></a> [lambda\_runtime](#input\_lambda\_runtime) | lambda\_runtime | `string` | `"nodejs16.x"` | no |
| <a name="input_tags"></a> [tags](#input\_tags) | Tag map for the resource | `map(string)` | `{}` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_aws_lambda_arn"></a> [aws\_lambda\_arn](#output\_aws\_lambda\_arn) | aws\_lambda\_function arn |
| <a name="output_aws_lambda_invoke_arn"></a> [aws\_lambda\_invoke\_arn](#output\_aws\_lambda\_invoke\_arn) | to be used in aws\_api\_gateway\_integration for APIGW |
