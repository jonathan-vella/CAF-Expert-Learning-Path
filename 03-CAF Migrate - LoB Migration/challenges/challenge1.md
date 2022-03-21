# CAF Hackathon

Adopt: **Migrate**

![CAF Hackathon Header](/media/caf-hackathon-header.png)

In this challenge we want to talk about the landing zone and the first two CAF modules.

## Challenge 1

Your challenge is to begin the initial planning for the migration of Contoso Land Surveying applications and existing infrastructure to Azure. Remember that while your initial focus is on a subset of servers and applications within the current datacenter, you are tasked with validating that the process you use throughout this journey can be used for future migrations. Do not forget to review and adapt your plan as you encounter new aspects and considerations with each subsequent challenge. During this stage, you will determine the process, tools, and technologies you will use to execute your migration to Azure. Based on your knowledge of the current infrastructure and the target platform, your team must work through the customer requirements to choose how you will migrate your applications, how you will determine the cost of the new environment, and how you will minimize downtime for the users of the applications as migrations occur. This time should be used to familiarize yourself with the general phases of migration to Azure. Answering the following questions can help you come to a consensus:

- How will you establish your migration priorities?
- How will you involve your stakeholders throughout the project?
- How will you create an inventory of your existing servers and determine dependencies?

As you design your plan, remember that the IT leadership team at Contoso Mortgage has worked closely with business partners to define the business drivers for this migration effort, which include:

- Limiting risk. While the applications selected for this migration effort are representative of Contoso Land Surveying on-premises estate, the are also production systems.
- Extend in a stable way. Without access to the source code, the applications cannot be easily modified and are considered stable today. Stability during and after the migration is critical.

These drivers have led to the following technical migration goals:

- Validate the migration of workloads hosted on legacy Windows operating systems including Windows Server 2008 R2, and Windows Server 2012 R2, as well as systems hosted on Microsoft SQL Server 2008 R2, to take advantage of the additional time offered for vendor support.
- Modernize systems to improve availability and resiliency where possible within the timelines needed for rapid migration. While the overarching goal is to rehost existing systems, where meaningful improvements can be made, they should be.
- Investigate the potential modernization of application components by evaluating and eventually transitioning to platform services where possible after issues around vendor support have been addressed.
- Educate the business and Contoso Land Surveying management on the processes and tooling that can be used to eventually move the remaining servers to Microsoft Azure, drastically reducing their on-premises presence.

## Customer requirements

Contoso Mortgage has the following requirements which you should take into consideration:

- Any assessment of the existing environment must provide a clear line of sight into server dependencies. While the Infrastructure and Application Support teams feel they understand their operating environment today, they would like verification before migrating to demonstrate to IT leadership.
- Before a migration occurs, IT needs to know the estimated monthly cost to host their servers in Azure to perform chargebacks to business owners. Under Contoso Land Surveying current Enterprise Agreement, they have negotiated a discount with Microsoft and may have existing Windows Server licenses that can be reused. They would like to understand their cost under both models - one where they reuse their existing licensing and one where they procure new licenses from Microsoft for their Windows Servers hosted in Microsoft Azure.
- In the current Azure subscription, cloud identities are used to secure Azure resources. The Security team would like to leverage their existing on-premises identities in the cloud if possible, to control access to Azure resources using role-based access control.
- The Security and Operations teams have determined that any domain-joined servers in Azure must be able to authenticate to Contoso Land Surveying domain even if connectivity between on-premises and Azure is lost. Any solution must account for a lack of network connectivity between Contoso's on-premises environment and Azure-hosted resources after the initial migration is complete.
- The existing applications have well-known URLs for Contoso Land Surveying users. IT leadership and business owners recognize that transitioning to the cloud may require a new URL to access each of the applications but want to minimize change and would like to have no more than one URL change for each application.
- The migrated applications must maintain their segmentation at the network layer. For example, the customer-accessible web front-end for the Contoso Mortgage application can only communicate with the application server, and the application server can only communicate with the database server.
- While the current migration effort is focused on a subset of applications, Contoso Land Surveying on-premise environment consists of over 180 servers. Any processes, tools, or technologies that are selected to support the migration of a workload must scale to the entire datacenter and not just these initial applications.

## Success Criteria

Present to your peer group your general migration plan, including how you will structure your team and how you will interact with your stakeholders throughout the project. Also, present a high-level architecture which shows:

- The tools and technologies you will use to migrate the existing servers to Microsoft Azure.
- The tools and technologies you will use to migrate any existing on-premises identities (users and groups) to Microsoft Azure.
- The target topology for any migrated servers in Azure, including resource groups, virtual networks and subnets, and any other Azure resources required to execute the migration.

Your architecture should be presented as one or more diagrams. As a component of your architecture, present to your peer group a naming standard for Azure resources that you will use as you progress through your migration. Be ready to answer the following questions:

- What tools or technologies will be used to show server dependencies to Contoso?
- Before migrating any servers to Azure, a cost estimate must be performed. This estimation must be presented under Contoso Land Surveying current pricing offer and their negotiated price with Microsoft. How will you perform this calculation?
- What tools or technologies will be used to allow servers to be domain-joined in Azure and logged on to with existing identities that will persist should hybrid connectivity not be available between Contoso Land Surveying on-premises datacenter and Azure?
- How will Contoso Mortgage host its public DNS in Azure and manage DNS records for its migrated web applications?

Discuss with your peer group...
