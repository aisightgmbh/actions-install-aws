# Install AWS Action

This action can be used to install the AWS CLI.
Afterwards, the `aws` command will be available.
This is only necessary if you're not running a job on the default runners.

## Example

```yaml
jobs:
  example-job:
    runs-on: <YourCustomRunner>
    steps:
      - uses: aisight/actions-install-aws@v1
      - run: aws --version
```
