# upgraded-bassoon
​A GRC-focused case study auditing HIPAA compliance within global assistance operations. Analyzed ePHI lifecycle, from intake to regional transfer, testing Administrative and Technical safeguards. Includes a Risk Control Matrix (RCM) and ERP process walkthroughs to demonstrate audit readiness for Senior Associate roles in Risk &amp; Regulatory.


flowchart TD
    A[Request for Patient Information Received] --> B[Identify Requestor]

    B --> C{Is Request Authorized?}

    C -->|Yes| D[Verify Identity and Consent]
    C -->|No| E[Reject Request and Log Incident]

    D --> F[Access Patient Information]

    F --> G{Minimum Necessary Rule Applied?}
    G -->|Yes| H[Provide Required Information Only]
    G -->|No| I[Limit Data to Required Scope]

    H --> J[Document Disclosure]
    I --> J

    J --> K[Log Transaction for Audit Trail]

    K --> L[Close Request]

    E --> M[Report Potential Compliance Issue]
    M --> L

    %% Control Points
    B:::control
    C:::control
    D:::control
    G:::control
    J:::control
    K:::control

    %% Styling
    classDef control fill:#bbf,stroke:#333,stroke-width:2px;
