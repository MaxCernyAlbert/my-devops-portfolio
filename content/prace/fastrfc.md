---
title: "Automated ServiceNow Change Management"
date: 2025-01-05
description: "Integrated ServiceNow FastRFC workflow into GitHub Actions for automated, traceable deployments without manual intervention."
tags: ["ServiceNow API", "GitHub Actions", "ITSM Integration", "Automation"]
---

### The Challenge

Enterprise ITSM policies required formal Change Requests (RFCs) for every production deployment, but manual creation caused deployment delays and bottlenecks. Teams needed a way to maintain compliance while enabling rapid, automated deployments without human intervention.

### My Solution

Built a **reusable GitHub Actions workflow** that automatically creates FastRFC tickets in ServiceNow via API during deployment. The workflow captures deployment metadata (version, environment, approver), submits the RFC, waits for approval, and proceeds with deployment—all without manual steps. Full audit trail maintained in ServiceNow for compliance.

### The Impact

{{< impact-grid >}}
100%|RFC Compliance|green
85%|Faster Deployments|blue
Zero|Manual RFC Creation|purple
{{< /impact-grid >}}
