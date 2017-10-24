# AWS Utilities CLI

## Amazon Web Services (AWS) Identity and Access Management (IAM)

### Introduction

This script adds predefined roles, groups and associated access policies to a stated AWS account. The script uses predefined arguments to build the relationship between a named policy user and a static policy file in order to state any relevant access rules.

Each [policy file](src/iam/roles/policy.json) needs a specific AWS Account ID before it can be used to create identities. The account ID must be added directly to policy files prior to running the script.

The script is work in progress.

### Key

Key of commonly used terms used in the script.

- `{policy_user}`: assigned to identify each group or role.
- `{policy_preset}`: policy preset assigned to the `policy_user`.
- `{policy_name}`: used to identify the `policy_file` created.
- `{policy_file}`: assigned to each `policy_user` identity.

### Run

```bash
$ chmod +x ./bin/iam/add-roles-groups
$ sh ./bin/iam/add-roles-groups
```

## Author

Author: [dataday](http://github.com/dataday)
