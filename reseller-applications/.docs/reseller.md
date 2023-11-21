```mermaid
graph TD;
  subgraph Reseller
    A[Reseller]
  end

  subgraph Platform
    B[Platform]
    C[Check Reseller Level]
    D[Apply Discount]
    E[Complete Purchase]
    F[Cashback based on Level]
  end

  A -->|Initiates Purchase| B
  B -->|Requests Reseller Level| C
  C -->|Level 1| D
  C -->|Level 2| D
  C -->|Level 3| D
  D -->|Applies Discount| E
  E -->|Completes Purchase| F
  F -->|Determines Cashback| B
  
