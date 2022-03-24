# CAF Hackathon - Adopt: Migrate

In this challenge we will build the Landing Zone for the migration.

## Challenge 3

The Director of IT wants to validate that the migration strategy is sound, and the migrated applications will not only be operational but also secure and compliant. Building this trust with the business is a key component of the migration to Azure. By validating not only your architecture but also your approach, you can make sure that the business is a partner in the move to the cloud. This will require testing in isolation so that the existing on-premises environment is not impacted. This will allow the relevant teams at Contoso to perform automated testing, offer application owners the opportunity to provide meaningful feedback, and allow for the migration to be performed as many times as it is needed to get it right.

In addition to maintaining their current segmentation, IT leadership would also like to introduce infrastructure to better position their applications for growth in the future. Moving to Azure will allow IaaS hosted applications to be more resilient by adopting features of the Azure platform that are only available in the cloud. To position themselves for better resiliency for theri web applications, the Network Operations team would like to incorporate a load balancer into their architecture to allow for greater flexibility, security and elasticity in the front-end layer of their applications.

## Notes
Azure Migrate will only create the VMs, their network interfaces, and their disks; all other resources must be staged in advance - so prepare an environment to migrate the servers to Azure.
The target virtual Network should have a IP Range 192.168.0.0/24 and build up a segmentation of the Network to deploy the different tiers of the application in these subnets.

## Customer Requirements

Contoso has the following requirements which you should take into consideration:

- The migrated applications must maintain their segmentation at the network layer. For example, the application server can only communicate with the database server.
- Due to security requirements, server administrators will not be able to use Remote Desktop over the public internet and no public IPs can be associated with Azure-hosted servers.
- Members of a security group called "CIT Server Admins" should be granted rights to use any RDP or remote connectivity solution.

## Success Criteria

- The target environment is deployed in a different resource group
- Network segmentation is in place and limits lateral movement between application layers, including non-application communication such as RDP access.
- Server administrators in the CIT Server Admins security group can access all of the migrated servers in a secure manner which does not require opening RDP access to the public internet for any migrated servers.
- For any migrated servers, native Azure functionality such as the Run Command should be available as if the server was provisioned from the Azure Marketplace.

Let's build up everything in Azure so that the VMs could be migrated to your Landing Zone (use a resource group rg-landingzone for this). And describe how you will address the success criteria.
