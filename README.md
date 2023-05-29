# it-ae-actions-terraform-pr-apply

A GitHub Composite action for applying terraform state changes when a pull request is merged.

This action requires a pull request to be associated with the run. If a pull request id is not passed as an input, the action will attempt to find the pull request ID with a matching merge commit hash. If not pull request id is found, the action will fail.

The `terraform apply` output will be posted to the pull request as a comment, trimmed to 65535 characters. The full output log will also be uploaded to s3 and a link to the log will be posted to the pull request as a comment.

## Inputs

See [action.yml](action.yml) for the full list of inputs.

## Outputs

See [action.yml](action.yml) for the full list of outputs.

