```mermaid
graph TD
  A[User] -->|Submits Form and Product Details| B(Platform)
  B -->|Checks Guarantee| C{Guarantee?}
  C ==>|Yes| D[Send Email with Payment Link]
  C ==>|No| E[Calculate Cost]
  D -->|No Cost| F[User Pays]
  E -->|Cost + Shipping| F[User Pays]
  F -->|User Pays| G[Proceed with Service]
  G -->|Service Completed| H[End]

  style A fill:#98FB98,stroke:#000,stroke-width:2px;
  style B fill:#FFD700,stroke:#000,stroke-width:2px;
  style C fill:#87CEEB,stroke:#000,stroke-width:2px;
  style D fill:#87CEFA,stroke:#000,stroke-width:2px;
  style E fill:#87CEEB,stroke:#000,stroke-width:2px;
  style F fill:#87CEEB,stroke:#000,stroke-width:2px;
  style G fill:#98FB98,stroke:#000,stroke-width:2px;
  style H fill:#98FB98,stroke:#000,stroke-width:2px;
