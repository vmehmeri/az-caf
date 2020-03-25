# Azure Cloud Adoption Framework
CAF is a set of methodologies. It's iterative, and not something "you do".

[Cloud Adoption Framework for Azure](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/ "Cloud Adoption Framework for Azure")

[CAF Assessmnent Benchmark](https://fusionassessment.azurewebsites.net/ "CAF Assessment Benchmark")

[Building a Digital Operating Model with Microsoft Cloud Adoption Framework (PDF)](https://azure.microsoft.com/en-us/resources/building-a-digital-operating-model-with-microsoft-cloud-adoption-framework/ "Building a Digital Operating Model with Microsoft Cloud Adoption Framework (PDF)")

[Microsoft CAF Strategy and Plan template](https://archcenter.blob.core.windows.net/cdn/fusion/readiness/Microsoft-Cloud-Adoption-Framework-Strategy-and-Plan-Template.docx "Microsoft Cloud Adoption Framework Strategy and Plan Template")

[Naming and Tagging tracker template](https://archcenter.blob.core.windows.net/cdn/fusion/readiness/CAF%20Readiness%20Naming%20and%20Tagging%20tracking%20template.xlsx "Naming and Tagging tracker template")

[Architectural Decision Guides](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/decision-guides/ "Architectural decision guides")

![CAF](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/_images/caf-overview.png "CAF Phases")

## Implement Disciplines of Cloud Governance
[Cost Management template](https://archcenter.blob.core.windows.net/cdn/fusion/governance/Cost%20Management%20Discipline%20Template.docx "Cost Management Template")

[Security Baseline template](https://archcenter.blob.core.windows.net/cdn/fusion/governance/Security%20Baseline%20Discipline%20Template.docx "Security Baseline Template")

[Identity Baseline template](https://archcenter.blob.core.windows.net/cdn/fusion/governance/Identity%20Baseline%20Discipline%20Template.docx "Identity Baseline Template")

[Resource consistency template](https://archcenter.blob.core.windows.net/cdn/fusion/governance/Resource%20Consistency%20Discipline%20Template.docx "Resource Consistency Template")

[Deployment Acceleration template](https://archcenter.blob.core.windows.net/cdn/fusion/governance/Deployment%20Acceleration%20Discipline%20Template.docx "Deployment Acceleration Template")

## Plan
Cloud Adoption Team (execution, agility) vs Cloud Governance Team (ensures processes and controls are implemented)
Rationalize Digital Estate
	* Incremental approach (Power of 10 * select first 19 applications to be migrated which are a mix of simple and complex workloads)
	* The output is a prioritized backlog

**Skills Readiness Plan**

**Cloud Adoption plan**
Converts the aspiratoinal goals of the cloud adoption strategy into an actionable plan. Use MSFT Template, sit down with client to fill it out.
* Identify owners of the applications
* Identify dependencies 

**Strategy, Plan & Ready Tooling**
Use Azure Devops Demo Generator (choose template: Microsoft Cloud Adoption Framework). 
* Scrum-based
* Includes epics, work items, etc.
* Can be customized with e.g. landing zone
* Can be integrated to Teams (don't ever need to use the browser/Devops)

Assessment - CAF benchmark: https://fusionassessment.azurewebsites.net/

**Common blockers:** 
* Team doesn't fully understand the cloud
* Stalled making hard decisions regarding networking, identity, connectivity, and centralized management principles
* Understanding governance, security & operations

**Involve CSO from the start. Aim for 100% alignment on the Azure environment**

## Ready
Go portal.azure.com
Type in the search bar: Quickstart Center
Select Azure Setup Guide


* Step 1: Define a management hierarchy
    * Create Management Groups, Subscriptions, and Resource Groups (optional)

* Step 2: Management Access (RBAC)
    * Add Role assignments in Subscriptions and Resource Groups

* Step 3: Manage Costs
    * Configure budget and alerts

* Step 4: Governance, security and compliance
    * Create and publish a blueprint
    * Assign Azure policies (may be part of the blueprint itself)
    * Explore Azure Security Center (ARM template for ASC may be part of the blueprint)

* Step 5: Monitoring and reporting
    * Explore Azure Monitor: visualize metrics, run log queries, set up alerts and actions
    * Explore Azure Service Health: Check global view of the health of Azure Services
    * Explore Azure Advisor: Check Azure recommendations for e.g:
        * High availability (e.g. add VM to scaleset)
        * Security (e.g. apply disk encryption or enable NSG)
        * Performance (e.g. create indexes for boosting SQL query performance)
        * Cost (e.g. resizing, shutting down underused VMs)
    * Operational excellence (e.g: set up and enforce policy rule, repair invalid log alerts, configure alerts)