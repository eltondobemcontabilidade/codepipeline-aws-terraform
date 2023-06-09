## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | ~> 1.4.2 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | ~> 4.37.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | ~> 4.37.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_cloudwatch_log_group.group](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_log_group) | resource |
| [aws_cloudwatch_log_stream.stream](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_log_stream) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_aws_region"></a> [aws\_region](#input\_aws\_region) | AWS infrastructure regio | `string` | `null` | no |
| <a name="input_cw_name"></a> [cw\_name](#input\_cw\_name) | CW name | `string` | `null` | no |
| <a name="input_retention_in_days"></a> [retention\_in\_days](#input\_retention\_in\_days) | CW retention\_in\_days | `number` | `30` | no |
| <a name="input_tags"></a> [tags](#input\_tags) | Tag map for the resource | `map(string)` | `{}` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_aws_cloudwatch_log_group_id"></a> [aws\_cloudwatch\_log\_group\_id](#output\_aws\_cloudwatch\_log\_group\_id) | cw group arn |
| <a name="output_aws_cloudwatch_log_stream"></a> [aws\_cloudwatch\_log\_stream](#output\_aws\_cloudwatch\_log\_stream) | cw stream arn |
