# CAF Hackathon

**Advanced** - Azure Landing Zones Accelerator

---

## Challenge 1 - Enterprise Scale Deployment

In this challenge you will be deploying one of the Enterprise Scale Reference implementations located in this [repository](https://github.com/Azure/Enterprise-Scale).

Success criteria for this challenge:

- Define if it's a brownfield or greenfield deployment

- Create a high-level deployment workflow (diagram not a CICD pipeline!) including pre-requisites

- Deploy either the Trey Research or AdventureWorks reference implementation

- **Do not deploy** the integrated CICD pipeline

---

## Challenge 2 - IaC with GitHub Actions

In this challenge you will be manually creating a CICD pipeline which will allow you to operate the Azure platform using AzOps (IaC with GitHub Actions).

This PowerShell module is rooted in the principle that everything in Azure is a resource and to operate at-scale, it should be managed declaratively to determine target goal state of the overall platform. Guidance for this challenge is located [here](https://github.com/azure/azops/wiki/github-actions).

Success criteria for this challenge:

- Configure AzOps via Portal or command-line script
- Initiate the first Pull workflow
- Validate AzOps by creating a new [Policy Assignment](https://github.com/Azure/Enterprise-Scale/wiki/Deploying-Enterprise-Scale-Platform-DevOps#create-new-policy-assignment-for-validation)

## Challenge 2a - PaC with GitHub Actions

In this challenge you will be using Policy-As-Code to modify a policy definition which is blocking you from creating the Azure Bastion Subnet.

- In your hub network, try to create the Azure Bastion Subnet. Azure Policy should block the operation.
- Modify the policy which is enforcing the use of Network Security Groups.
- Create the Azure Bastion Subnet.

---

## Challenge 3 - Governance Reporting

In this challenge you will be implementing [AzGovViz](https://github.com/JulianHayward/Azure-MG-Sub-Governance-Reporting) which is a PowerShell based script that iterates your Azure Tenant´s Management Group hierarchy down to Subscription level. It captures most relevant Azure governance capabilities such as Azure Policy, RBAC and Blueprints and a lot more. From the collected data AzGovViz provides visibility on your HierarchyMap, creates a TenantSummary, creates DefinitionInsights and builds granular ScopeInsights on Management Groups and Subscriptions.

Success criteria for this challenge:

- Setup AzGovViz from the console or GitHub Codespaces
- Run AzGovViz

---

## Challenge 4 - Azure Design Review

In this challenge you will be doing an Azure design review to double-check that best practices are being followed. You will be using this [repo](https://github.com/Azure/review-checklists) which contains code and examples to operationalize spreadsheet-based checklists that can be used for Azure design reviews on multiple technologies.

Success criteria for this challenge:

- Use the Excel spreadsheet, import the latest checklist, and explore the contents of the file.
- If there is enough time left, use the Azure Resource Graph to verify your Azure environment.
