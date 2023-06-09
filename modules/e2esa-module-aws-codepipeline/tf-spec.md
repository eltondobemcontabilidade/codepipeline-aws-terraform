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
| [aws_codepipeline.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/codepipeline) | resource |
| [aws_iam_policy.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_role.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role_policy_attachment.attachment](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_policy_document.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_approve_comment"></a> [approve\_comment](#input\_approve\_comment) | approval comment | `string` | `"Terraform code updated"` | no |
| <a name="input_approve_sns_arn"></a> [approve\_sns\_arn](#input\_approve\_sns\_arn) | SNS arn | `string` | `"sns"` | no |
| <a name="input_approve_url"></a> [approve\_url](#input\_approve\_url) | approval url | `string` | `"url"` | no |
| <a name="input_artifacts_store_type"></a> [artifacts\_store\_type](#input\_artifacts\_store\_type) | Artifacts store type | `string` | `"S3"` | no |
| <a name="input_aws_region"></a> [aws\_region](#input\_aws\_region) | AWS infrastructure regio | `string` | `null` | no |
| <a name="input_branch_name"></a> [branch\_name](#input\_branch\_name) | branch\_name | `string` | `"main"` | no |
| <a name="input_codestar_connector_credentials"></a> [codestar\_connector\_credentials](#input\_codestar\_connector\_credentials) | codestar\_connector\_credentials | `string` | `""` | no |
| <a name="input_full_repository_id"></a> [full\_repository\_id](#input\_full\_repository\_id) | full\_repository\_id | `string` | `""` | no |
| <a name="input_input_artifacts"></a> [input\_artifacts](#input\_input\_artifacts) | input\_artifacts | `string` | `"tf-code"` | no |
| <a name="input_output_artifact_format"></a> [output\_artifact\_format](#input\_output\_artifact\_format) | OutputArtifactFormat | `string` | `"CODE_ZIP"` | no |
| <a name="input_output_artifacts"></a> [output\_artifacts](#input\_output\_artifacts) | output\_artifacts | `string` | `"tf-code"` | no |
| <a name="input_policy_name"></a> [policy\_name](#input\_policy\_name) | policy\_name | `string` | `"E2EsaTerraformCodePipelinePolicy"` | no |
| <a name="input_project_name"></a> [project\_name](#input\_project\_name) | codebuild project name | `string` | `null` | no |
| <a name="input_role_name"></a> [role\_name](#input\_role\_name) | role\_name | `string` | `"E2EsaTerraformCodePipelineRole"` | no |
| <a name="input_s3_bucket_id"></a> [s3\_bucket\_id](#input\_s3\_bucket\_id) | s3\_bucket\_id | `string` | `""` | no |
| <a name="input_source_provider"></a> [source\_provider](#input\_source\_provider) | source\_provider | `string` | `"CodeStarSourceConnection"` | no |
| <a name="input_tags"></a> [tags](#input\_tags) | Tag map for the resource | `map(string)` | `{}` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_aws_codepipeline_arn"></a> [aws\_codepipeline\_arn](#output\_aws\_codepipeline\_arn) | aws codepipeline project arn |
