[![Maintained by Scaffoldly](https://img.shields.io/badge/maintained%20by-scaffoldly-blueviolet)](https://github.com/scaffoldly)
![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/scaffoldly/terraform-github-repository)
![Terraform Version](https://img.shields.io/badge/tf-%3E%3D0.15.0-blue.svg)

## Description

Create a GitHub repostiory from a template repository

## Usage

```hcl
module "repository" {
  source = "scaffoldly/github/repository"

  template = var.template
  name     = local.repo_name
}
```

<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 0.15 |
| <a name="requirement_github"></a> [github](#requirement\_github) | 4.9.4 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_github"></a> [github](#provider\_github) | 4.9.4 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [github_repository.repository](https://registry.terraform.io/providers/integrations/github/4.9.4/docs/resources/repository) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_name"></a> [name](#input\_name) | Name of the repo | `string` | n/a | yes |
| <a name="input_template"></a> [template](#input\_template) | Organization and template repo name (e.g. scaffoldly/sls-rest-api-template) | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_name"></a> [name](#output\_name) | Re-output of var.name |
<!-- END_TF_DOCS -->
