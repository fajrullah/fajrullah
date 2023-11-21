```mermaid
graph TD;
  subgraph NOC
    A[Alert Triggered]
  end

  subgraph Application
    B[Application Notifications]
    C[Call Phone]
    D[SMS]
    E[Mail]
  end

  subgraph Dashboard
    F[Return to Dashboard]
  end

  A -->|Alert Details| B
  B --> C
  B --> D
  B --> E
  C -->|Phone Call| F
  D -->|SMS| F
  E -->|Email| F
