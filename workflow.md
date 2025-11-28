
```mermaid
flowchart LR
    %% Nodes
    A[📥 Request Intake & Prioritization<br>(Product Owner)]:::po --> B[🕒 Assessment & Provisional ETA<br>(Stakeholders + Agency)]:::stake
    B --> C[📢 Communicate ETA to Requestor]:::po

    C --> D{🔀 Parallel Work}:::stake
    D --> E[📝 Brief Draft<br>(Agency)]:::agency
    D --> F[💰 Quotation<br>(Agency)]:::agency

    E --> G[✅ Combined Approval<br>(Stakeholders)]:::stake
    F --> G

    G --> H[⚙️ Execution & Continuous Testing<br>(Agency)]:::agency
    H --> I[🚀 Deployment<br>(Agency)]:::agency
    I --> J[📣 Communication to Team<br>(Product Owner)]:::po

    %% Styles
    classDef po fill:#f8d7da,stroke:#c82333,color:#000,font-weight:bold;
    classDef stake fill:#e2e3e5,stroke:#6c757d,color:#000,font-weight:bold;
    classDef agency fill:#d1ecf1,stroke:#0c5460,color:#000,font-weight:bold;
