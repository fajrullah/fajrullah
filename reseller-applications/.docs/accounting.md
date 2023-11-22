```mermaid
graph TD
  A[Sales] -->|Generate Invoice| B(Accounting Staff)
  B -->|Submit Invoice| C(System)
  C -->|Integrate with XML| D[Third-Party Accounting App]

  style A fill:#98FB98,stroke:#000,stroke-width:2px;
  style B fill:#87CEEB,stroke:#000,stroke-width:2px;
  style C fill:#87CEEB,stroke:#000,stroke-width:2px;
  style D fill:#87CEEB,stroke:#000,stroke-width:2px;