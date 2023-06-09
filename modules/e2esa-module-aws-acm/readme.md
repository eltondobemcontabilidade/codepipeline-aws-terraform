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
| [aws_acm_certificate.cert](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate) | resource |
| [aws_acm_certificate_validation.validation](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate_validation) | resource |
| [aws_route53_record.r53](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record) | resource |
| [aws_route53_zone.hz](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/route53_zone) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_aws_region"></a> [aws\_region](#input\_aws\_region) | AWS infrastructure region | `string` | `null` | no |
| <a name="input_bool"></a> [bool](#input\_bool) | bool | `bool` | `false` | no |
| <a name="input_domain_name"></a> [domain\_name](#input\_domain\_name) | domain name | `string` | `null` | no |
| <a name="input_list"></a> [list](#input\_list) | list | `list(string)` | `[]` | no |
| <a name="input_name"></a> [name](#input\_name) | name | `string` | `null` | no |
| <a name="input_number"></a> [number](#input\_number) | number | `number` | `0` | no |
| <a name="input_prefix"></a> [prefix](#input\_prefix) | Resource name prefix | `string` | `null` | no |
| <a name="input_tags"></a> [tags](#input\_tags) | Tag map for the resource | `map(string)` | `{}` | no |
| <a name="input_validation_method"></a> [validation\_method](#input\_validation\_method) | validation\_method | `string` | `"DNS"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_arn"></a> [arn](#output\_arn) | arn |
| <a name="output_domain_name"></a> [domain\_name](#output\_domain\_name) | domain\_name |
| <a name="output_id"></a> [id](#output\_id) | id |
| <a name="output_status"></a> [status](#output\_status) | status |
| <a name="output_tags_all"></a> [tags\_all](#output\_tags\_all) | A map of tags assigned to the resource, including those inherited from the provider default\_tags |
| <a name="output_type"></a> [type](#output\_type) | type |
