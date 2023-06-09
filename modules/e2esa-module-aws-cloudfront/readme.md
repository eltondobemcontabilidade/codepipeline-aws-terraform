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
| [aws_cloudfront_distribution.cf](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudfront_distribution) | resource |
| [aws_cloudfront_origin_access_control.oac](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudfront_origin_access_control) | resource |
| [aws_cloudfront_origin_access_identity.origin_access_identity](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudfront_origin_access_identity) | resource |
| [aws_s3_bucket.selected](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/s3_bucket) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_allowed_methods"></a> [allowed\_methods](#input\_allowed\_methods) | allowed\_methods | `list(string)` | <pre>[<br>  "GET",<br>  "HEAD",<br>  "OPTIONS"<br>]</pre> | no |
| <a name="input_aws_region"></a> [aws\_region](#input\_aws\_region) | AWS infrastructure region | `string` | `"us-east-1"` | no |
| <a name="input_cached_methods"></a> [cached\_methods](#input\_cached\_methods) | cached\_methods | `list(string)` | <pre>[<br>  "GET",<br>  "HEAD",<br>  "OPTIONS"<br>]</pre> | no |
| <a name="input_cf_domain_names"></a> [cf\_domain\_names](#input\_cf\_domain\_names) | cf\_domain\_names | `list(string)` | `null` | no |
| <a name="input_cf_log_s3_bucket"></a> [cf\_log\_s3\_bucket](#input\_cf\_log\_s3\_bucket) | cf\_log\_s3\_bucket | `string` | `null` | no |
| <a name="input_cf_log_s3_bucket_prefix"></a> [cf\_log\_s3\_bucket\_prefix](#input\_cf\_log\_s3\_bucket\_prefix) | cf\_log\_s3\_bucket\_prefix | `string` | `"cf-log"` | no |
| <a name="input_cloudfront_comment"></a> [cloudfront\_comment](#input\_cloudfront\_comment) | cloudfront\_comment | `string` | `"CloudFront Distribution for "` | no |
| <a name="input_cloudfront_default_certificate"></a> [cloudfront\_default\_certificate](#input\_cloudfront\_default\_certificate) | cloudfront\_default\_certificate | `bool` | `true` | no |
| <a name="input_name"></a> [name](#input\_name) | name | `string` | `null` | no |
| <a name="input_prefix"></a> [prefix](#input\_prefix) | Resource name prefix | `string` | `"cf-"` | no |
| <a name="input_price_class"></a> [price\_class](#input\_price\_class) | price\_class | `string` | `"PriceClass_200"` | no |
| <a name="input_restriction_type"></a> [restriction\_type](#input\_restriction\_type) | restriction\_type | `string` | `"whitelist"` | no |
| <a name="input_s3_bucket_regional_domain_name"></a> [s3\_bucket\_regional\_domain\_name](#input\_s3\_bucket\_regional\_domain\_name) | s3\_bucket\_regional\_domain\_name | `string` | `null` | no |
| <a name="input_s3_origin_id"></a> [s3\_origin\_id](#input\_s3\_origin\_id) | s3\_origin\_id | `string` | `null` | no |
| <a name="input_tags"></a> [tags](#input\_tags) | Tag map for the resource | `map(string)` | `{}` | no |
| <a name="input_viewer_protocol_policy"></a> [viewer\_protocol\_policy](#input\_viewer\_protocol\_policy) | viewer\_protocol\_policy | `string` | `"redirect-to-https"` | no |
| <a name="input_whitelist_locations"></a> [whitelist\_locations](#input\_whitelist\_locations) | whitelist\_locations | `list(string)` | <pre>[<br>  "US",<br>  "CA",<br>  "IN"<br>]</pre> | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_arn"></a> [arn](#output\_arn) | n/a |
| <a name="output_domain_name"></a> [domain\_name](#output\_domain\_name) | n/a |
| <a name="output_hosted_zone_id"></a> [hosted\_zone\_id](#output\_hosted\_zone\_id) | n/a |
| <a name="output_id"></a> [id](#output\_id) | n/a |
| <a name="output_status"></a> [status](#output\_status) | n/a |
| <a name="output_tags_all"></a> [tags\_all](#output\_tags\_all) | n/a |
