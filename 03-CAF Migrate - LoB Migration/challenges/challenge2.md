# CAF Hackathon - Adopt: Migrate

In this challenge we want to get our first hands on Azure Migrate.

## Challenge 2

In this challenge, you will assess customer's existing operating environment for the applications and map them to Azure resources. Your assessment will determine how existing servers and workloads are connected and how they will perform in Azure.
Remember that while your initial focus is on a subset of servers and applications within the current datacenter, you are tasked with developing a process for assessment that can scale beyond just a handful of servers.
Assessments should not just be limited to using tooling to discover information about your environment, you should schedule time to speak to business owners, end-users, other members within the IT department, etc. in order to get a full picture of what is happening within the environment and understand things tooling cannot tell you. The business owners at currently pay for the servers that host their applications and are cost-conscious.

The IT leadership team wants to make sure that before any migrations begin a cost assessment is performed for each application to demonstrate the cost to the business owners who will continue to bear the cost of the servers, even in Azure.
The IT leadership team is also concerned about dependent services for migrated applications based on the feedback they have received from the Infrastructure and Application Support teams. IT leadership does not feel they understand their environment today based on previous outages in the on-premises environment and are concerned that they do not have access to the source code for these applications to make updates if dependencies cannot be mapped before migration.
As a reminder, the current application server architecture is as follows:

[Application architecture](./../media/application_architecture.png)

## Customer requirements

Customer has the following requirements which you should take into consideration:

- While the Infrastructure and Application Support teams feel they understand their operating environment today, they want to have a verification before migrating and have a way to report the current state to IT leadership.
- Before migration, the business owners of each application need to know the estimated monthly cost to host their servers in Azure under the current EA pricing agreement (assume a 5% discount).
- In the existing environment, applications are segmented and secured through subnets and local OS firewalls. They would like to know what their network topology in Azure will look like and how they can be as secure in Azure as in their current on-premises environment, if not more so, after the migration.

## Success Criteria

- Dependencies between servers in the on-premises environment can be visualized before migration and visualizations include server-to-server connections as well as ports and protocols.
- The network design limits communication between application tiers to only the required ports and protocols while limiting lateral movement within the network.
- The servers targeted for migration are sized appropriately and the compute needs of each server can be adjusted to meet application owner requirements before migration.
- The estimated cost for each application can be viewed independently and demonstrates the lowest acceptable cost with equivalent performance to the existing on-premises servers.

Let's discuss the findings with your peer group.