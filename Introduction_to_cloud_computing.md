# Cloud Computing 

[reference Link](https://learn.microsoft.com/en-us/training/modules/describe-cloud-compute/3-what-cloud-compute>)

Delivery of computing services over the internet. Computing services include common IT infrastructure such as virtual machines, storage, databases, and networking. Cloud services also expand the traditional IT offerings to include things like Internet of Things (IoT), machine learning (ML), and artificial intelligence (AI).



# Shared Responsibility Model

[reference Link](https://learn.microsoft.com/en-us/training/modules/describe-cloud-compute/4-describe-shared-responsibility-model) 

When using a cloud provider,__user__ always be responsible for:  
	• The information and data stored in the cloud  
	• Devices that are allowed to connect to your cloud (cell phones, computers, and so on)  
	• The accounts and identities of the people, services, and devices within your organization  
 
The **cloud provider** is always responsible for:  
	• The physical datacenter  
	• The physical network  
	• The physical hosts  
 
Your **service model** will determine responsibility for things like:  
	• Operating systems  
	• Network controls  
	• Applications  
	• Identity and infrastructure  

 ![Shared Responsibility Reference](https://learn.microsoft.com/en-us/training/wwl-azure/describe-cloud-compute/media/shared-responsibility-b3829bfe.svg)

# Cloud Models

[reference Link](https://learn.microsoft.com/en-us/training/modules/describe-cloud-compute/5-define-cloud-models)


1. A private cloud is, in some ways, the natural evolution from a corporate datacenter. It’s a cloud (delivering IT services over the internet) that’s used by a single entity.

2. A public cloud is built, controlled, and maintained by a third-party cloud provider. With a public cloud, anyone that wants to purchase cloud services can access and use resources. The general public availability is a key difference between public and private clouds.

3. A hybrid cloud is a computing environment that uses both public and private clouds in an inter-connected environment. A hybrid cloud environment can be used to allow a private cloud to surge for increased, temporary demand by deploying public cloud resources.
   
4. multi cloud you deal with two (or more) public cloud providers and manage resources and security in both environments.

5. Azure Arc is a set of technologies that helps manage your cloud environment
   
6. Azure VMware lets you run your VMware workloads in Azure with seamless integration and scalability.


# Comparision between Cloud Models
   
 | Public cloud |Private cloud | Hybrid cloud |
|---|---|---|
|No capital expenditures to scale up |Organizations have complete control over resources and security | Provides the most flexibility |
| Applications can be quickly provisioned and deprovisioned | Data is not collocated with other organizations’ data | Organizations determine where to run their applications |
| Organizations pay only for what they use | Hardware must be purchased for startup and maintenance | Organizations control security, compliance, or legal requirements|
Organizations don’t have complete control over resources and security | Organizations are responsible for hardware maintenance and updates | |


# Consumption-based Model

- Two types of expenses to consider.

  1. Capital expenditure (CapEx) is typically a one-time, up-front expenditure to purchase or secure tangible resources. A new building, repaving the parking lot,   building a datacenter, or buying a company vehicle are examples of CapEx.

  2. operational expenditure (OpEx) is spending money on services or products over time. Renting a convention center, leasing a company vehicle, or signing up for cloud services are all examples of OpEx.

- Cloud computing operates on a consumption-based model which is OpEx where we don’t pay for the physical infrastructure, the electricity, the security, or anything else associated with maintaining a datacenter. Instead, we pay for the IT resources we use. If we don’t use any IT resources this month, we don’t pay for any IT resources. 


- Consumption-based model has many benefits, including:

1. No upfront costs.
2. No need to purchase and manage costly infrastructure that users might not use to its fullest potential.
3. The ability to pay for more resources when they're needed.
4. The ability to stop paying for resources that are no longer needed.
