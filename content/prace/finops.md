

---
title: "Custom FinOps Intelligence Tool"
date: 2025-01-10
description: "Developing a proprietary cost-analysis tool that outperformed Azure Advisor and saved 25% of cloud spend."
tags: ["FinOps", "Azure", "Python", "Cost-Optimization"]
---

### The Challenge

A Logistics client faced a cloud bill growing 15% MoM. Azure Advisor was insufficient, missing context-specific waste like "zombie" dev environments running over weekends, and over-provisioned SQL resources.

### My Solution

I developed a **proprietary Python crawler** (Azure Function) that interacts directly with the Azure Resource Graph. It enforces tagging, identifies unattached disks/IPs, and auto-scales non-prod environments based on business hours.

### The Impact

{{< impact-grid >}}
25%|Bill Reduction|green
40h+|Admin Saved|blue
100%|Visibility|purple
{{< /impact-grid >}}

