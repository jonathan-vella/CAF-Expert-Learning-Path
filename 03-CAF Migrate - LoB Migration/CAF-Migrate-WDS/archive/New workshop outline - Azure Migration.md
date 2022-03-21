![Microsoft Cloud Workshop](https://github.com/Microsoft/MCW-Template-Cloud-Workshop/raw/master/Media/ms-cloud-workshop.png "Microsoft Cloud Workshops")

<div class="MCWHeader1">
Line of Business Application Migration
</div>

<div class="MCWHeader2">
New workshop outline
</div>

<div class="MCWHeader3">
May 2019
</div>

## Line of Business Application Migration outline

  **Team**                        **Name**                            **Email**
  ------------------------------- ----------------------------------- ------------------------------------
  Program manager                 Insert the program manager's name   Insert the program manager's email
  Project manager                 Insert the project manager's name   Insert the project manager's name
  Tech lead                       Insert tech lead's name             Insert tech lead's email
  Content developer vendor name   Insert vendor's name                Insert vendor's email
  Stakeholder                     Insert stakeholders' name(s)        Insert stakeholders' email
  SME Team                        Insert lead SME name                Insert lead SME email

  **Workshop details**      **Description**
  ------------------------- --------------------------------------------------------------------------------------
  Kickoff date              Insert the project kick-off date
  Release date              Insert the project release date
  Target audience           
  Hero solution             Insert Hero solution
  Technical use case        Insert the technical use case
  Products/Services         Insert the products/services covered in workshop
  Link to source material   Insert the link(s) to any source material used to create the workshop, if applicable

## Abstract 

### Workshop

In this workshop, you will learn how to design a migration strategy for on-premises environments to Azure, including the migration of virtual and physical services as well as databases.

At the end of this workshop you will be better able to rationalize the migration of various workloads to Microsoft Azure as well as understanding how to determine the cost of hosting migrated workloads in Azure. 

### Whiteboard design session *(this will go in the readme and in the WDS document)*

In this whiteboard design session, you will look at how to design an Azure migration for a heterogenous customer environment. The existing infrastructure comprises both Windows and Linux servers running on both VMWare and physical machines, and includes some legacy servers. Throughout the whiteboard design session, you will look at the various options and services available to migrate heterogenous environments to Azure.

At the end of this workshop, you will be better able to design and implement the discovery and assessment of environments to evaluate their readiness for migrating to Azure using services including Azure Migrate, Azure Database Migration Service, and Azure Site Recovery.

## Hands-on lab *(this will go in the readme and in the HOL document)*

In this lab, you will use Azure Migrate to perform an assessment of an on-premises environment with both Windows and Linux operating systems. You will learn how to perform discovery with Azure Migrate, how to group machines and customize assessments to understand dependencies of discovered workloads and how to determine cost.

You will then learn how to migrate servers from an on-premises environment to Azure using Azure Site Recovery. This includes setting up the Azure environment, configuring replication, and performing a test failover.

You will also learn to use the Database Migration Service and the Data Migration Assistant to perform assessments of databases and migrate database schemas and content to Azure.

At the end of this lab, you will be better able to execute migrations to Azure.

## Customer case study summary

Fabrikam Fabrics is a major manufacturer and distributor of clothing and soft furnishing materials. The CTO, James Lynch, was hired 6 months ago with a mandate to address ever-increasing IT costs. He has identified a sprawling IT estate, including a substantial legacy server footprint, including:
- Windows servers including both x32 and x64 hardware running Windows Server 2003 through to 2016
- Linux servers running a mix of RHEL 6.10 and 7 series (7.2 through 7.6) and Ubuntu 16.04
- The above servers comprise both physical machines as well as VMs hosted on VMware infrastructure managed by vCenter 6.5
- Multiple database engines, including Microsoft SQL Server, PostgreSQL, and Cassandra

In total, 448 servers and VMs have been identified to date. There is a complex web of dependencies between servers and no-one has a clear view of the entire estate.

The board has approved a plan to migrate as much existing infrastructure as possible to Azure, to eliminate IT infrastructure overheads and 'clean house'. Your team has been tasked with planning and executing this migration.

## Lab summary

Before the lab, you will have pre-deployed an on-premises infrastructure hosted in Hyper-V.  This infrastructure is hosting a multi-tier application called 'SmartHotel', using Hyper-V VMs for each of the application tiers.

During the lab, you will migrate this entire application stack to Azure. This will include assessing the on-premises application using Azure Migrate; migrating the database tier to Azure SQL Database using SQL Server Data Migration Assistant (DMA) and the Azure Database Migration Service (DMS); and migrating the web and application tiers using Azure Site Recovery. This includes migration of both Windows and Linux VMs.

