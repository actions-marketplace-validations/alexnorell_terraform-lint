# Terraform Lint with Diff

A GitHub action to check for and display any formatting issues found with `terraform fmt`.

## Usage

```yaml
name: terraform-lint

on: [push, pull_request]

jobs:
  lint:
    runs-on: ubuntu-latest
    steps:
    - name: Check out code
      uses: actions/checkout@master
    - name: Lint Terraform
      uses: actionshub/terraform-lint-with-diff@master
```
