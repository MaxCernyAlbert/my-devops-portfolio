---
title: "ServiceNow GitHub Actions ITSM automatizace - Enterprise Change Management"
date: 2025-01-05
description: "Enterprise ITSM automatizace případová studie: Automatizovaná integrace ServiceNow FastRFC s GitHub Actions pro Azure nasazení. 100% compliant change management bez manuálního zásahu."
tags: ["ServiceNow API", "GitHub Actions", "ITSM integrace", "Azure DevOps", "Change Management", "Enterprise"]
keywords: ["servicenow github actions", "azure devops itsm", "automatizace change managementu", "enterprise compliance", "devops governance", "azure deployment compliance"]
---

### Výzva

Enterprise ITSM politiky vyžadovaly formální Change Requesty (RFC) pro každé produkční nasazení, ale manuální vytváření způsobovalo zpoždění nasazení a úzká hrdla. Týmy potřebovaly způsob, jak udržet compliance při umožnění rychlých, automatizovaných nasazení bez lidského zásahu.

### Mé řešení

Vytvořil jsem **znovupoužitelný GitHub Actions workflow**, který automaticky vytváří FastRFC tickety v ServiceNow přes API během nasazení. Workflow zachycuje metadata nasazení (verze, prostředí, schvalovatel), odesílá RFC, čeká na schválení a pokračuje s nasazením—vše bez manuálních kroků. Kompletní audit trail je udržován v ServiceNow pro compliance.

### Dopad

{{< impact-grid >}}
100%|RFC compliance|green
85%|Rychlejší nasazení|blue
Zero|Manuální tvorba RFC|purple
{{< /impact-grid >}}
