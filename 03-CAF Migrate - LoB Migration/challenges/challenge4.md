# CAF Hackathon - Adopt: Migrate

In this challenge we will migrate the database and the website server to azure.

## Challenge 4

Our last challenge is the migration of the webserver and the UbuntuWAF as IaaS to Azure as well as migrating the existing Database to Azure Database PaaS.

We don't provide any additional information - we want to first hear your concept and after the concept is discussed, we want your team to migrate to PaaS in Azure. Tasks:

1. Describe your concept of migration with your peers and wait for "GO" from the trainer.
2. Migrate the servers and database to Azure.
3. If there is time left, assess the application using the App Service Migration Assistant.

Have in mind, there are a number of post-migration steps that should be completed before the migrated services is ready for production use.
These include:

- Validation that the Azure VM agent is deployed.
- Enabling backup and disaster recovery at scale
- Encrypting VM disks at scale
- Ensuring the network is properly secured
- Ensuring proper subscription governance is in place, such as role-based access control and Azure Policy
- Reviewing recommendations from Azure Advisor and Security Center
- Cleaning up migration resources

If there is time left, please try to perform some of these steps.
