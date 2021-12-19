## Azure Fundamental

# Cloud Computing
Service delivery model over the internet (cloud). This includes but is not limited to

- **compute power** meaning servers such as Windows, Linux, hosting environments, etc.
storage like files and/or databases
- **networking** in azure but also outside when connecting to your company network
-** analytics** services for visualization and telemetry data

Key concepts

- **scalability** is the ability to scale, so allocate and deallocate resources at any time
- **elasticity** is the ability to scale dynamically
- **agility** is the ability to react fast (scale quickly)
- **fault tolerance** is the ability to maintain system uptime while physical and service component failures happen
- **disaster recovery** is the process and design principle which allows a system to recovers from natural or human-induced disasters
- **high availability** is the agreed level of operational uptime for the system. It is a simple calculation of system uptime versus the whole lifetime of the system.

> availability = uptime/(uptime + downtime)

# Economies of Scale

The principle of economies of scale states that as the companies grow they become more effective at managing shared operations. Be that HR and hiring, taxes, accounting, internal operations, marketing, big purchases via contracts meaning better discounts, etc.

Because of those, companies can save/earn more which in return allows for a reduction in the cost of their services to their customers. This is the so-called ‘price per unit.

It’s not possible to go to 0 because in the end, some underlying infrastructure needs to run to provide the services. But the larger the scale the more benefits can be passed to customers.

In fact, at the current scale, Microsoft can already offer multiple services for free due to how small a fraction of the cost it is for them.

# CapEx vs OpEx

Differences between Capital Expenditure and Operational Expenditure


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1639897062006/xM0m1FwRZ.png)

# What is a consumption-based model?

The consumption-based model is a pricing model used in the cloud so that customers are only charged based on their resource usage.

This model is characterized by
- No associated upfront cost
- No wasted resources as such no charges are incurred for unused resources*. Unused in this case is different per service. For instance, blob storage that stores any data is considered to be used, as it consumes the storage space. Virtual Machines that are running consume CPU, memory and other resources even if there isn’t any traffic. Hence they are considered to be used and will incur charges.
- Pay for what you need
- Stop paying when you don’t

**Consumption** is the virtual metric used to calculate how much each resource (service) in Azure was used. Each service has many smaller metrics that track its consumption to offer best possible pricing model. Those metrics are tracked on very granular level.

# Service Models responsibilities

As a service means which party will manage the particular layer and all the layers below.
- **Software** layer consists the application (application code and set) & the application data
- **Platform** layer means all the supporting software and the operating system required to host the application
- **Infrastructure** layer consists hardware the infrastructure and virtualization required to host the platform


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1639897856905/jh5-yWuyp.png)

# Responsibility Matrix
As such following table represents the responsibilities

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1639898207228/kwmR7sbYA.png)



# Cloud Deployment Model

Cloud Deployment Model is simple a separation that describes where are the company resources deployed. Whenever this is in a public cloud provider environment or private data center.

The below table presents high-level deployment model separation


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1639898023380/vWipVkocz.png)

# Public Cloud

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1639898064929/iLr4NLKgL.png)

# Private Cloud

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1639898101270/2katU6gAH.png)

# Hybrid Cloud

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1639898133860/fxUfZc2wp.png)

# Data Center

- **Physical facility**
- **Hosting** for a group of networked **servers**
- Own **power, cooling & networking** infrastructure

# Region
- Geographical area on the planet
- One but usually more datacenters connected with low-latency network (<2 milliseconds)
- Location for your services
- Some services are available only in certain regions
- Some services are global services, as such are not assigned/deployed in specific region
- Globally available with 50+ regions
- Special government regions (US DoD Central, US Gov Virginia, etc.)
- Special partnered regions (China East, China North)

# Availability Zone

- Regional feature
- Grouping of physically separate facilities
- Designed to protect from data center failures
- If zone goes down others continue working
- Two service categories
Zonal services (Virtual Machines, Disks, etc.)
Zone-redundant services (SQL, Storage, etc.)
- Not all regions are supported
-Supported region has three or more zones
- A zone is one or more data centers

# Region Pair
- Each region is paired with another region making it a region pair
- Region pairs are static and cannot be chosen
- Each pair resides within the same geography*
Exception is Brazil South
- Physical isolation with at least 300 miles distance (when possible)
- Some services have platform-provided replication
- Planned updates across the pairs
- Data residency maintained for disaster recovery

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1639899343148/ZEhEZWUlu.png)

# Geographies
- Discrete market
- Typically contains two or more regions
- Ensures data residency, sovereignty, resiliency, and compliance requirements are met
- Fault tolerant to protect from region-wide failures
- Broken up into areas
Americas,
Europe,
Asia Pacific,
Middle East and Africa
- Each region belongs only to one Geography

