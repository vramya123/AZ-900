# Azure account

![image](https://github.com/vramya123/AZ-900/assets/23298075/b5f0c8b8-84ca-434b-8d72-a9769310ed89)

# Ways to interact with Azure
1. PowerShell command line interface (CLI) : pwsh . Note : we have to append each azure command with az word
2. BASH CLI : bash .  Note : we have to append each azure command with az word
3. Azure CLI interactive mode : az interactive . Note : we do not have to append each azure command with az word
4. Azure portal 

# Azure physical infrastructure

## Regions
A region is a geographical area on the planet that contains at least one, but potentially multiple datacenters that are nearby and networked together with a low-latency network.

## Availability Zones
- Availability zones are physically separate datacenters within an Azure region.
- Each availability zone is made up of one or more datacenters equipped with independent power, cooling, and networking.
- Availability zones are connected through high-speed, private fiber-optic networks.

  ![image](https://github.com/vramya123/AZ-900/assets/23298075/5b8770b5-d0f8-4789-9ebe-017a63ba2ba3)

**Note :-  To ensure resiliency, a minimum of three separate availability zones are present in all availability zone-enabled regions. However, not all Azure Regions currently support availability zones.** 

## Region pairs
Most Azure regions are paired with another region within the same geography (such as US, Europe, or Asia) at least 300 miles away. This approach allows for the replication of resources across a geography that helps reduce the likelihood of interruptions because of events such as natural disasters, civil unrest, power outages, or physical network outages that affect an entire region. For example, if a region in a pair was affected by a natural disaster, services would automatically fail over to the other region in its region pair.

![image](https://github.com/vramya123/AZ-900/assets/23298075/ded37d92-6fcb-42a1-959f-d1378c0082c8)

Advantages of region pairs:
1. If an extensive Azure outage occurs, one region out of every pair is prioritized to make sure at least one is restored as quickly as possible for applications hosted in that region pair.
2. Planned Azure updates are rolled out to paired regions one region at a time to minimize downtime and risk of application outage.
3. Data continues to reside within the same geography as its pair (except for Brazil South) for tax- and law-enforcement jurisdiction purposes.

**Note :- Most regions are paired in two directions, meaning they are the backup for the region that provides a backup for them (West US and East US back each other up). However, some regions, such as West India and Brazil South, are paired in only one direction.**

## Sovereign Regions
Sovereign regions are instances of Azure that are isolated from the main instance of Azure. You may need to use a sovereign region for compliance or legal purposes.

Azure sovereign regions include:

US DoD Central, US Gov Virginia, US Gov Iowa and more: These regions are physical and logical network-isolated instances of Azure for U.S. government agencies and partners. These datacenters are operated by screened U.S. personnel and include additional compliance certifications.
China East, China North, and more: These regions are available through a unique partnership between Microsoft and 21Vianet, whereby Microsoft doesn't directly maintain the datacenters.

# Azure management infrastructure

## Azure resources and resource groups

A resource is the basic building block of Azure. Anything you create, provision, deploy, etc. is a resource. Virtual Machines (VMs), virtual networks, databases, cognitive services, etc. are all considered resources within Azure.
Resource groups  are a way to logically organize resources and are simply groupings of resources. When you create a resource, you’re required to place it into a resource group. 

**Note:-
1. A single resource can only be in one resource group at a time.
2. Resource groups can't be nested, meaning you can’t put resource group B inside of resource group A.**

![image](https://github.com/vramya123/AZ-900/assets/23298075/7e854432-a6f0-4834-8c86-62d06f7f7814)

 ## Azure subscriptions                                                                                                    
- Subscriptions allow you to logically organize your resource groups and facilitate billing.
- It also provides you with authenticated and authorized access to Azure products and services.

-  There are two types of subscription boundaries that you can use:

Billing boundary: This subscription type determines how an Azure account is billed for using Azure. You can create multiple subscriptions for different types of billing requirements. Azure generates separate billing reports and invoices for each subscription so that you can organize and manage costs.

Access control boundary: Azure applies access-management policies at the subscription level, and you can create separate subscriptions to reflect different organizational structures. An example is that within a business, you have different departments to which you apply distinct Azure subscription policies. This billing model allows you to manage and control access to the resources that users provision with specific subscriptions.

## Azure management groups
- Azure management groups provide a level of scope above subscriptions. You organize subscriptions into containers called management groups and apply governance conditions to the management groups. All subscriptions within a management group automatically inherit the conditions applied to the management group, the same way that resource groups inherit settings from subscriptions and resources inherit from resource groups.
- Management groups can be nested.

  ![image](https://github.com/vramya123/AZ-900/assets/23298075/85fd4330-a6bd-4890-bd77-939669106a59)

  * 10,000 management groups can be supported in a single directory.
  *  A management group tree can support up to six levels of depth. This limit doesn't include the root level or the subscription level.
  *  Each management group and subscription can support only one parent.
