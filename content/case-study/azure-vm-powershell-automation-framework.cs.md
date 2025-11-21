---
title: "Azure VM automatizační framework - Enterprise správa konfigurace"
date: 2025-01-02
description: "Enterprise Azure automatizace případová studie: Modulární PowerShell framework pro zero-touch post-deployment VM. OS hardening, compliance scanning a integrace Azure Landing Zone s kompletním IaC přístupem."
tags: ["PowerShell", "Azure VMs", "Správa konfigurace", "Azure Landing Zone", "Azure DevOps", "IaC"]
keywords: ["azure vm automatizace", "azure landing zone", "enterprise správa konfigurace", "azure devops automatizace", "azure compliance", "azure architekt", "infrastructure as code"]
---

### Výzva

Po nasazení Azure VM přes IaC týmy bojovaly s post-deployment konfigurací—instalace softwaru, bezpečnostní hardening, nastavení monitoringu a připojení k doméně. Manuální konfigurace byla časově náročná, náchylná k chybám a nekonzistentní napříč prostředími. Neexistoval standardizovaný, opakovatelný proces.

### Mé řešení

Vyvinul jsem komplexní sadu **PowerShell modulů** pro automatizovanou post-deployment konfiguraci VM. Moduly řeší OS hardening, instalaci softwaru, doménovou integraci, deployment monitoring agentů a compliance scanning. Architektura je modulární a verzovaná, umožňující snadnou customizaci přes centralizované konfigurační soubory. Plně integrováno do deployment pipelines pro zero-touch provisioning.

### Dopad

{{< impact-grid >}}
90%|Snížení času konfigurace|green
100%|Konzistence|blue
Znovupoužitelné|Napříč prostředími|purple
{{< /impact-grid >}}
