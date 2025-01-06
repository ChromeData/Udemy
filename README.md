# Microsoft Azure

## Building a Mini Azure Environment for Learning (AZ-900)

---

## Introduction

In this project, we create a foundational environment in Microsoft Azure to explore and learn the core concepts of the AZ-900 certification. This setup includes key Azure services such as Virtual Machines, Resource Groups, Storage Accounts, and Network Security Groups. The goal is to understand how these components interact and to practice basic configuration and monitoring. 

Metrics and insights from this setup include:
- **Azure Resource Logs**: Tracking resource changes and access.
- **Activity Logs**: Monitoring administrative activities.
- **Network Watcher Metrics**: Visualizing inbound and outbound traffic flows.
- **Cost Analysis**: Reviewing the cost breakdown of resources used.

---

## Architecture Before Optimization

### Description of the Environment:

- **Azure Resource Groups**: Logical containers for managing Azure resources.
- **Virtual Machines (VMs)**:
  - 1 Windows Server
  - 1 Linux (Ubuntu) Server
- **Storage Account**: Used for diagnostics and logging.
- **Network Security Groups (NSG)**: Applied to allow unrestricted access for testing.
- **Virtual Network**: Default configuration connecting resources.
- **Azure Monitor**: Basic setup for tracking metrics and logs.

### Key Observations:
- No cost optimization measures applied.
- Security rules are lenient to enable broad accessibility.
- No autoscaling or high availability configurations.

---

## Architecture After Optimization / Security Enhancements

### Security Improvements:
- **Resource Groups**: Reorganized to separate production and development resources.
- **Virtual Machines (VMs)**:
  - Hardened configurations with restricted admin access via Azure Bastion.
  - Applied patch management for operating systems.
- **Network Security Groups (NSG)**: Restricted inbound traffic to specific IPs.
- **Storage Account**: Enforced encryption for data at rest.
- **Azure Cost Management**: Enabled budgeting and alerting for cost control.
- **Azure Monitor**: Enhanced monitoring with alerts for resource health and activity.

These improvements significantly reduced the environment's vulnerability and ensured better cost management and performance monitoring.

---

## Hands-On Practice and Observations

### Before Optimization:
1. **Activity Logs**: Unfiltered logs capturing all admin actions.
2. **Network Watcher Logs**: High levels of incoming unauthorized traffic.

### After Optimization:
1. **Azure Security Center**: Reduced recommendations from critical to minor.
2. **Cost Analysis**: Improved resource utilization and cost efficiency.
3. **Network Watcher Logs**: Only permitted IPs access the environment.

---

## Learnings and Outcomes

This exercise demonstrates:
- The importance of organizing Azure resources effectively.
- How to secure Azure environments using NSGs and other built-in tools.
- The role of Azure Monitor in tracking performance and detecting anomalies.
- The impact of cost management tools for staying within budget.

---

## Additional Resources

- [Microsoft Learn: AZ-900 Learning Path](https://learn.microsoft.com/en-us/certifications/exams/az-900/)
- [Udemy Course: AZ-900 Fundamentals](https://www.udemy.com/course/az900-azure/)
- [Azure Architecture Center](https://learn.microsoft.com/en-us/azure/architecture/)

---

## Conclusion

This project serves as a practical guide to understanding the fundamental concepts of Microsoft Azure as outlined in the AZ-900 certification. By building and optimizing a mini Azure environment, learners can gain hands-on experience to confidently approach the exam.

---
