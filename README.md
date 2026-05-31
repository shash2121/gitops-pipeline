### Create the OIDC Provider in Your AWS Account

```bash
# List OIDC Providers
aws iam list-open-id-connect-providers

# Create OIDC Provider
aws iam create-open-id-connect-provider \
  --url https://token.actions.githubusercontent.com \
  --client-id-list sts.amazonaws.com 

# List OIDC Providers
aws iam list-open-id-connect-providers
```