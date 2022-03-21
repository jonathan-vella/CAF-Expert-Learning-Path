# CAF Hackathon

Adopt: **Migrate**

![CAF Hackathon Header](/media/caf-hackathon-header.png)

In this challenge we want to get our first hands on Azure Migrate.

## Challenge 2

In this challenge, you will assess Contoso Land Surveying existing operating environment for the applications Contoso Mortgage and Contoso Mortgage Admin and continue mapping them to Azure resources. Your assessment will include determining how existing servers and workloads are connected and how they will perform in Azure. Remember that while your initial focus is on a subset of servers and applications within the current datacenter, you are tasked with developing a process for assessment that can scale beyond just a handful of servers. Assessments should not just be limited to using tooling to discover information about your environment, you should schedule in time to speak to business owners, end-users, other members within the IT department, etc. in order to get a full picture of what is happening within the environment and understand things tooling cannot tell you. The business owners at Contoso Mortgage currently pay for the servers that host their applications and are cost-conscious. The IT leadership team at Contoso Mortgage wants to make sure that before any migrations begin, that a cost assessment is performed for each application to demonstrate the cost to the business owners who will continue to bear the cost of the servers, even in Azure. The IT leadership team is also concerned about dependent services for migrated applications based on the feedback they have received from the Infrastructure and Application Support teams. IT leadership does not feel they understand their environment today based on previous outages in the on-premises environment and are concerned that they do not have access to the source code for these applications to make updates if dependencies cannot be mapped before migration. As a reminder, the current application server architecture is as follows:

[Application architecture](./../media/application_architecture.png)

## Customer requirements

Contoso Mortgage has the following requirements which you should take into consideration:

- While the Infrastructure and Application Support teams feel they understand their operating environment today, they would like verification before migrating and have a way to report the current state to IT leadership.
- Before migration, the business owners of each application need to know the estimated monthly cost to host their servers in Azure under the current EA pricing agreement.
- In the existing environment, applications are segmented and secured through subnets and local OS firewalls. They would like to know what their network topology in Azure will look like and how they can be as secure in Azure as in their current on-premises environment, if not more so, after the migration.

## Success Criteria

- Dependencies between servers in the on-premises environment can be visualized before migration and visualizations include server-to-server connections as well as ports and protocols.
- The network design limits communication between application tiers to only the required ports and protocols while limiting lateral movement within the network.
- The servers targeted for migration are sized appropriately and the compute needs of each server can be adjusted to meet application owner requirements before migration.
- The estimated cost for each application can be viewed independently and demonstrates the lowest acceptable cost with equivalent performance to the existing on-premises servers.

Let's discuss the findings with your peer group
