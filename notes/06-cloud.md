# 6. Cloud Computing and Virtualization

**Cloud computing** = renting computing (servers, storage, apps) over the internet, pay for what you use.
**Virtualization is the base of cloud.** Cloud providers use it to share big servers between many customers.

## Service models
- **IaaS** (Infrastructure as a Service): you rent virtual machines. Example: AWS **EC2**.
- **PaaS** (Platform as a Service): you only upload code. Example: Heroku, Google App Engine.
- **SaaS** (Software as a Service): ready software. Example: Gmail, Google Docs.

## Deployment models
- **Public cloud**: shared, run by a provider (AWS, Azure, Google Cloud).
- **Private cloud**: only for one company.
- **Hybrid cloud**: public + private together.

## Cloud features
On-demand use, scalability (grow or shrink), elasticity, pay-per-use, resource pooling.

## AWS EC2 quick idea
1. Choose OS image (AMI).
2. Choose size (CPU, RAM).
3. Launch the instance (a VM in the cloud).
4. Connect with SSH and run your app.
