---
title: "Mermaid Diagram Demo"
date: 2025-01-01
description: "Demo page for Mermaid diagrams"
draft: true
---

### Chaos to Order Transformation

{{< mermaid >}}
stateDiagram-v2
    [*] --> Chaos
    Chaos --> Transformation
    Transformation --> Excellence
    Excellence --> [*]

    Chaos --> Chaos: Firefighting
    Transformation --> Chaos: Failed attempt

    state Chaos {
        [*] --> Manual
        Manual --> NoStandards
        NoStandards --> Silos
    }

    state Excellence {
        [*] --> Automated
        Automated --> Predictable
        Predictable --> Scalable
    }
{{< /mermaid >}}

---

### CI/CD Migration

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
