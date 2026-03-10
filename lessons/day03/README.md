# Task for Day03

- Get yourself familiarized with Terraform documentation
  
`https://registry.terraform.io/providers/hashicorp/azurerm/latest`
- Create the below Azure resources using azurerm Terraform provider
    - Resource Group
    - Storage account

## Commands used in the demo

- Log in to Azure
```
- az login
```

- Create Service Principal 
```
az ad sp create-for-rbac -n az-demo --role="Contributor" --scopes="/subscriptions/$SUBSCRIPTION_ID"
```
Note: Use the values generated here to export the variables in the next step

Set as environment variables

- Set env vars so that the service principal is used for authentication

```
For Linux 
export ARM_CLIENT_ID=""
export ARM_CLIENT_SECRET=""
export ARM_SUBSCRIPTION_ID=""
export ARM_TENANT_ID=""
```
```
For Windows 
$Env:ARM_CLIENT_ID = "<APPID_VALUE>"
$Env:ARM_CLIENT_SECRET = "<PASSWORD_VALUE>"
$Env:ARM_SUBSCRIPTION_ID = "<SUBSCRIPTION_ID>"
$Env:ARM_TENANT_ID = "<TENANT_VALUE>"
```


