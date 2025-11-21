---
title: "Enterprise Integration Platform"
date: 2025-01-03
description: "Architected IaC-based integration platform using Azure Service Bus, Logic Apps, APIM, and SharePoint with Terraform + Bicep deployment."
tags: ["Azure Service Bus", "Logic Apps", "APIM", "SharePoint", "Terraform", "Bicep"]
---

### The Challenge

Client needed to integrate their proprietary software with another proprietary system, exchanging data through Azure Service Bus while maintaining full auditability and compliance. SharePoint integration was required for document management, and everything needed to be fully automated and version-controlled.

### My Solution

Architected a complete **IaC-based integration platform** using Azure Service Bus for messaging, Logic Apps for orchestration workflows, API Management for secure API exposure, and SharePoint integration for document handling. All components—including Logic Apps workflows—were defined as code using a hybrid **Terraform + Bicep** deployment strategy. Full GitOps workflow with automated testing and deployment pipelines.

### The Impact

{{< impact-grid >}}
100%|Infrastructure as Code|green
Zero|Manual Configuration|blue
Full|Audit Trail|purple
{{< /impact-grid >}}
