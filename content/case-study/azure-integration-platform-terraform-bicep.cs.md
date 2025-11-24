---
slug: "azure-integration-platform-terraform-bicep"
title: "Azure integrační platforma - Enterprise Terraform & Bicep architektura"
date: 2025-01-03
description: "Enterprise Azure architektura případová studie: Integrační platforma využívající Service Bus, Logic Apps, API Management nasazená přes Terraform + Bicep IaC. Kompletní GitOps workflow s Azure Landing Zone vzory."
tags: ["Azure Service Bus", "Logic Apps", "APIM", "Terraform", "Bicep", "Azure Landing Zone"]
keywords: ["azure integrační platforma", "terraform bicep azure", "azure service bus", "azure landing zone", "enterprise cloudová architektura", "azure architekt", "infrastructure as code"]
---

### Výzva

Klient potřeboval integrovat svůj proprietární software s jiným proprietárním systémem, vyměňovat data přes Azure Service Bus při zachování plné auditovatelnosti a compliance. Byla vyžadována integrace SharePoint pro správu dokumentů a vše muselo být plně automatizované a verzované.

### Mé řešení

Navrhl jsem kompletní **IaC integrační platformu** využívající Azure Service Bus pro messaging, Logic Apps pro orchestrační workflows, API Management pro bezpečné vystavení API a integraci SharePoint pro práci s dokumenty. Všechny komponenty—včetně Logic Apps workflows—byly definovány jako kód pomocí hybridní **Terraform + Bicep** deployment strategie. Kompletní GitOps workflow s automatizovaným testováním a deployment pipelines.

### Dopad

{{< impact-grid >}}
100%|Infrastructure as Code|green
Zero|Manuální konfigurace|blue
Kompletní|Audit Trail|purple
{{< /impact-grid >}}
