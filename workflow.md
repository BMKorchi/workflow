
flowchart LR
    A[Request Intake & Prioritization<br/>(Product Owner)] --> B[Assessment & Provisional ETA<br/>(Stakeholders + Agency)]
    B --> C[Communicate ETA to Requestor]

    C --> D{Parallel Work}
    D --> E[Brief Draft<br/>(Agency)]
    D --> F[Quotation<br/>(Agency)]

    E --> G[Combined Approval<br/>(Stakeholders)]
    F --> G

    G --> H[Execution & Continuous Testing<br/>(Agency)]
    H --> I[Deployment<br/>(Agency)]
    I --> J[Communication to Team<br/>(Product Owner)]

    %% Assign classes with the older "class" syntax
    class A,C,J po;
    class B,D,G stake;
    class E,F,H,I agency;

    %% Define role styles
    classDef po fill:#f8d7da,stroke:#c82333,color:#000,font-weight:bold;
    classDef stake fill:#e2e3e5,stroke:#6c757d,color:#000,font-weight:bold;
    classDef agency fill:#d1ecf1,stroke:#0c5460,color:#000,font-weight:bold;
