### Terraform state creation + key vault

This will create a storage account and storage container for you to use in other terraform configurations. 

Followed the [microsoft documentation](https://learn.microsoft.com/en-us/azure/developer/terraform/store-state-in-azure-storage?tabs=terraform)

To use the terraform state in your app look at the section that includes setting up the backend.

Also added in creating a key vault from the [microsoft documentation](https://learn.microsoft.com/en-us/azure/key-vault/keys/quick-create-terraform?tabs=azure-cli)

I believe that this gives the current user the access policies as I did not set up a service principal as specified in the setting up [terraform documentation](https://developer.hashicorp.com/terraform/tutorials/azure-get-started/azure-build)

This would be a best practice to follow for production environments but here for testing I believe it is the current user who is logged into azure who gets the policies.
