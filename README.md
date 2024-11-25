# workflows

Shared workflows for GitHub Actions

## terraform

Static code analysis for Terraform. Performs the following checks:

- terraform fmt -check
- terraform validate
- tflint

Inputs:

- terraform-version -- Version of Terraform to use for `terraform fmt`, `terraform init`, and `terraform validate`. Defaults to latest version.
- directory -- Run checks in this directory, relative to project root. Defaults to project root.
- test-dir -- If specified, `terraform init` and `terraform validate` will run in this directory. Otherwise, they will run in the directory specified by the `directory` input. This is useful for a reusable module that has a test directory containing test or example code that can be used as a root module containing the module to be tested.
