---
title: "Migrace Jenkins na GitHub Actions - Enterprise CI/CD transformace"
date: 2025-01-08
description: "Enterprise CI/CD transformace případová studie: Migrace bez výpadku z Jenkins a Azure DevOps na GitHub Actions. Terraform IaC, Policy as Code a integrace Azure Governance s 30% rychlejšími pipelines."
tags: ["Migrace", "GitHub Actions", "Jenkins", "Terraform", "Azure DevOps", "CI/CD Pipelines"]
keywords: ["migrace jenkins github actions", "migrace azure devops", "enterprise cicd", "terraform cicd", "devops transformace", "azure governance", "policy as code"]
---

{{< mermaid >}}
flowchart LR
    J["🔧 Jenkins"]
    A["⚡ Azure DevOps"]

    G["🚀 GITHUB"]

    G1["GitHub Actions"]
    G2["Governance"]
    G3["Policy as Code"]
    G4["IaC"]

    J --> G
    A --> G
    G1 --> G
    G2 --> G
    G3 --> G
    G4 --> G

    style J fill:#6b7280,stroke:#4b5563,color:#fff
    style A fill:#6b7280,stroke:#4b5563,color:#fff
    style G fill:#3b82f6,stroke:#2563eb,color:#fff,stroke-width:3px
    style G1 fill:#22c55e,stroke:#16a34a,color:#fff
    style G2 fill:#22c55e,stroke:#16a34a,color:#fff
    style G3 fill:#22c55e,stroke:#16a34a,color:#fff
    style G4 fill:#22c55e,stroke:#16a34a,color:#fff
{{< /mermaid >}}

### Výzva

Organizace provozovala fragmentovanou CI/CD infrastrukturu rozdělenou mezi Jenkins a Azure DevOps. Tato dvouplatformová konfigurace generovala významné licenční náklady a vytvářela denní tření pro vývojové týmy.

**Bolestivé body vývojářů:**
- Vývojáři si nemohli sestavit vlastní pipelines — neexistovaly žádné znovupoužitelné komponenty
- Týmy lepily dohromady vlastní řešení, která často selhávala v produkci
- Každá změna pipeline vyžadovala podporu a zásah DevOps týmu
- Nulová konzistence napříč projekty — každý tým implementoval CI/CD jinak
- Žádné standardy, žádná governance, žádné sdílené best practices

Nedostatek self-service možností znamenal, že DevOps tým se stal úzkým hrdlem, zpomalujícím dodávky napříč všemi projekty.

### Mé řešení

Provedl jsem kompletní migraci bez výpadku na GitHub Enterprise. Řešení se vyvinulo v komplexní platformu se znovupoužitelnými stavebními bloky:

- Převedl jsem komplexní Groovy/YAML pipelines na optimalizované **GitHub Actions** workflows
- Vytvořil jsem knihovnu **znovupoužitelných workflow komponent**, které si vývojáři mohou sami skládat
- Vytvořil jsem **komplexní dokumentaci** vysvětlující použití každého stavebního bloku
- Zavedl jsem **governance politiky** a **Policy as Code** standardy
- Standardizoval jsem veškerý provisioning infrastruktury přes **Terraform moduly**

Výsledek: vývojáři jsou nyní plně soběstační. Mohou sestavovat, upravovat a udržovat své vlastní pipelines bez zásahu DevOps. Workflows jsou čisté a čitelné — členové týmu z jiných oddělení je mohou snadno revidovat a pochopit. Doba běhu pipeline se snížila v průměru o 30%.

### Dopad

{{< impact-grid cols="2" >}}
$$$|Ušetřené licenční náklady|green
Sjednocená|Developer Experience|white
{{< /impact-grid >}}
