# Cloud Adoption Expert Learning Path

## Attendee Requirements

| Module        | Duration | Target Roles      | Required Certifications                                                                                                                                                          | Add. Recommended Certifications                                                                                                                                                                                                             | Pre-Learning                                                                                                                                                                                                                                         | Azure Subscription (see notes below)                                | Labs                                                                                                                                                                                                                                    |
| ------------- | -------- | ----------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| CAF 101       | 2-Days   | Sales & Technical | [AZ-900](https://docs.microsoft.com/en-us/learn/certifications/exams/az-900)                                                                                                     |                                                                                                                                                                                                                                             | [The business value of Microsoft Azure](https://docs.microsoft.com/en-us/learn/paths/learn-business-value-of-azure/)                                                                                                                                 | Not required                                                        |                                                                                                                                                                                                                                         |
| CAF Basic     | 1-Day    | Sales & Technical | CAF 101 plus [AZ-900](https://docs.microsoft.com/en-us/learn/certifications/exams/az-900)                                                                                        |                                                                                                                                                                                                                                             | CAF 101 or equivalent                                                                                                                                                                                                                                | Required per Team; each individual with Owner RBAC role             |                                                                                                                                                                                                                                         |
| CAF Migration | 2-Days   | Technical         | CAF Basic plus [AZ-104](https://docs.microsoft.com/en-us/learn/certifications/exams/az-104)                                                                                      | [AZ-500](https://docs.microsoft.com/en-us/learn/certifications/exams/az-500) and [AZ-305](https://docs.microsoft.com/en-us/learn/certifications/exams/az-305)                                                                               | [Applications and infrastructure migration and modernization](https://docs.microsoft.com/en-us/learn/modules/app-and-infra-migration-and-modernization/)                                                                                             | Required per Team; each individual with Owner RBAC role             | [Deploy this lab environment at least 1 day before HOL](https://github.com/jonathan-vella/MCW-Line-of-business-application-migration/blob/master/Hands-on%20lab/Before%20the%20HOL%20-%20Line-of-business%20application%20migration.md) |
| CAF Advanced  | 2-Days   | Technical         | CAF Migration plus [AZ-104](https://docs.microsoft.com/en-us/learn/certifications/exams/az-104) and [AZ-305](https://docs.microsoft.com/en-us/learn/certifications/exams/az-305) | [AZ-400](https://docs.microsoft.com/en-us/learn/certifications/exams/az-400), [AZ-500](https://docs.microsoft.com/en-us/learn/certifications/exams/az-500) and [AZ-700](https://docs.microsoft.com/en-us/learn/certifications/exams/az-700) | [Build a cloud governance strategy on Azure](https://docs.microsoft.com/en-us/learn/modules/build-cloud-governance-strategy-azure/) and [Enterprise Scale Architecture](https://docs.microsoft.com/en-us/learn/paths/enterprise-scale-architecture/) | Required per individual with Owner RBAC role and Tenant Root Access | Make sure that you have the necessary AAD permissions                                                                                                                                                                                   |

# Azure subscription requirements

- Azure subscriptions based on Free Account (aka Free Trial) are not compatible with the hands-on labs.

- Azure subscription for CAF Migration must be a paid (not Trial) subscription and can be shared across teams as long as there are sufficient resource quotas.

- Azure subscription for CAF Advanced must be a paid subscription associated to a non-production AAD tenant since [tenant root access](https://github.com/Azure/Enterprise-Scale/wiki/Deploying-Enterprise-Scale-Pre-requisites) is required during HOL.

 

# **Tooling Prerequisites**

To avoid any delays with downloading or installing tooling, have the following ready prior to attending:

- A modern laptop running the latest version of either Windows 10  or Window 11, Mac OS X 10.13 or higher, or Ubuntu 16.04.
- Install your choice of Integrated Development Environment (IDE) software, such
   as [Visual Studio](https://visualstudio.microsoft.com/vs/community/), [Visual Studio Code](https://code.visualstudio.com/download), [Eclipse](https://www.eclipse.org/), or [IntelliJ](https://www.jetbrains.com/idea/)
- Download of the latest version of PowerShell, Az. PowerShell Modules, [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest)