# Install AWS Action

[![Tests](https://github.com/aisightgmbh/actions-install-aws/actions/workflows/on_push.yaml/badge.svg)](https://github.com/aisightgmbh/actions-install-aws/actions/workflows/on_push.yaml)

This action can be used to install the AWS CLI.
Afterwards, the `aws` command will be available.
This is only necessary if you're not running a job on the default runners.

## Example

```yaml
jobs:
  example-job:
    runs-on: <YourCustomRunner>
    steps:
      - uses: aisightgmbh/actions-install-aws@v1
      - run: aws --version
```
