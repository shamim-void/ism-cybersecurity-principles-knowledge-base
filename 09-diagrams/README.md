# 🎨 Visual Diagrams (Mermaid)

These diagrams help visualise the framework and processes.

---

## 1. Framework Overview

```mermaid
graph TD
    ISM[ISM Cybersecurity Principles] --> GOV[Govern]
    ISM --> IDE[Identify]
    ISM --> PRO[Protect]
    ISM --> DET[Detect]
    ISM --> RES[Respond]
    ISM --> REC[Recover]
    
    GOV --> GOV1[GOV-01: Executive Accountability]
    GOV --> GOV2[GOV-02: CISO Leadership]
    GOV --> GOV3[GOV-03: Risk Management]
    
    IDE --> IDE1[IDE-01: Asset Identification]
    IDE --> IDE2[IDE-02: Business Criticality]
    
    PRO --> PRO1[PRO-04: Attack Surface Reduction]
    PRO --> PRO2[PRO-08: Data Encryption]
    PRO --> PRO3[PRO-12: Least Privilege]
    
    DET --> DET1[DET-01: Centralised Logging]
    DET --> DET2[DET-02: Event Detection]
    
    RES --> RES1[RES-01: Incident Planning]
    RES --> RES2[RES-03: Incident Response]
    
    REC --> REC1[REC-01: Business Resumption]
```

---

## 2. Maturity Progression

```mermaid
graph LR
    A[Level 1: Initiated] --> B[Level 2: Initial]
    B --> C[Level 3: Developing]
    C --> D[Level 4: Managing]
    D --> E[Level 5: Optimising]
    A:::level1
    B:::level2
    C:::level3
    D:::level4
    E:::level5
    classDef level1 fill:#f9f,stroke:#333,color:#000
    classDef level2 fill:#ff9,stroke:#333,color:#000
    classDef level3 fill:#9f9,stroke:#333,color:#000
    classDef level4 fill:#9cf,stroke:#333,color:#000
    classDef level5 fill:#99f,stroke:#333,color:#000
```

---

## 3. Risk Management Process (GOV-03 / IDE-04)

```mermaid
flowchart TD
    A[Identify assets & risks] --> B[Analyse risks]
    B --> C[Evaluate risks]
    C --> D{Treat risks?}
    D -->|Yes| E[Implement controls]
    E --> F[Accept residual risk]
    D -->|No| F
    F --> G[Monitor & review]
    G --> A
```

---

## 4. Incident Management Lifecycle

```mermaid
flowchart LR
    A[Plan\nRES-01] --> B[Detect\nDET-03]
    B --> C[Report\nRES-02]
    C --> D[Contain, Eradicate, Recover\nRES-03]
    D --> E[Capture Lessons\nRES-04]
    E --> A
```