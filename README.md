# terraform-commands
(Hobby) Here are some very common terraform commands 

```
terraform init  # install terraform  
terraform validate  
terraform apply  
terraform destroy  
terraform plan  
```

Here are some backend configs for `terraform init`: 
```
terraform init \
    -backend-config="address=https://gitlab.com/api/v4/xyz" \
    -backend-config="lock_address=https://gitlab.com/api/v4/xyz" \
    -backend-config="unlock_address=https://gitlab.com/api/v4/xyz" \
    -backend-config="username=<YOUR-USERNAME>" \
    -backend-config="password=<YOUR-ACCESS-TOKEN>" \
    -backend-config="lock_method=POST" \
    -backend-config="unlock_method=DELETE" \
    -backend-config="retry_wait_min=5"

```
