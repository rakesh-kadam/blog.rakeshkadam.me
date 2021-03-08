## Azure: Governance

## Governance 101
The governance in the cloud is critical as the processes and behavior is different in the cloud compared to on-premises. In the cloud by default, there are many types of public-facing services available (This could be bad). Governance is about the enforcement of rules and ensuring proper functioning to standards.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1615105444482/5FjTbi1Mg.png)

### Understanding your requirements
Takes some time to understand your requirement which should take into consideration the corporate standards and regulatory compliance. Azure is a shared responsibility model for many aspects of compliance. You can check Compliance Manager to help you track it. Often these are all around mitigating risk.

### Key Organizational Components
Management groups, Subscriptions, and Resource Groups are the components that are used to create an organizational structure in Azure.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1615104943943/vMh7P8IFJ.png)

### So what we can do?
Along with organizational components, we can make use of RBAC (Role-Based Access Control), Policy, Budgets, and Locking (subscription/RG/resources).

### A quick word on ARM (Azure Resource Manager)
Understanding the structure of resources helps with the Azure Policy. Everything is Azure is made up of resources that are defined in resource providers. A resource has properties and actions. 

### RBAC 
At all levels, access control can be leveraged on the management plane. Some services also support RBAC on the data plane. eg: some storage services. They can be inherited and roles consist of actions that are assigned to the security principle at a scope. Try to grant to groups and not users and leverage PIM for just-in-time access.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1615105229648/w5ehhonqW.png)

### Azure Policy
Azure policy sits at the top of ARM and any CRUD operation has to pass through it. It can be used for enforcement and audit. A policy is a set of conditions built around resource attributes and an effect. Policies can be grouped into initiatives for assignments and compliance.


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1615105295882/APYGm_NiT.png)
### Cost Management and Budgets
Cost Management provides insight and control of Azure spend. It consists of cost analysis, cost alerts, and budgets - Alert and Action Groups. Cost allocation with EA or Customer Agreement. You can use the Azure Price calculator to estimate the pricing.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1615105045386/LIVNoMUT2.png)

### Naming standards
Having a standard is very important and Azure has some great recommendations. Naming conventions apply to all resources and guest OS. Try to have consistent naming for cloud and on-premise.

### Tagging
A name: value pair which can be very powerful to provide identity attributes/metadata of a resource. Have standards for tags used and values. It can be enforced through policy. Its use includes search, filter, and billing.  

### Blueprints
Blueprints bring together different types of artifacts to "stamp" a configuration like resource groups, RABC, ARM JSON, Policy, and custom scripts. It can have different deploy modes.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1615105396794/WQXNyOTgq.png)

### Azure Resource Graph
Provides a way to query ARM very efficiently and across subscriptions using KQL. Portal or Powershell/CLI/REST can be used.

### Azure Advisor
Throughout your Azure life, there is constant re-evaluation and optimization. The azure advisor provides recommendations around key areas and should be checked weekly.

### Key Microsoft Resources

-  [Aka.ms/governancedocs](https://docs.microsoft.com/en-us/azure/governance/) 

-  [Cloud Adoption Framework](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/) 

-  [Well-Architected Framework](https://www.microsoft.com/azure/partners/well-architected) 

-  [Azure Architecture Center](https://docs.microsoft.com/en-us/azure/architecture/) 


