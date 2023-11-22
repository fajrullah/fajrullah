```mermaid
graph TD
  A[Sales] -->|Attend| B(Attendance)
  B -->|Add Photo & Location| C{Photos & Locations Added?}
  C -- Yes --> D(Continue Sales Activities)
  C -- No --> E[End - Incomplete Attendance]

  D -->|Generate Sales| F(Upload Invoices)
  F -->|Invoices Uploaded| G{Bonuses Granted?}
  G -- Yes --> H[End - Bonuses Granted]
  G -- No --> I[End - Bonuses Not Granted]

  style A fill:#98FB98,stroke:#000,stroke-width:2px;
  style B fill:#87CEEB,stroke:#000,stroke-width:2px;
  style C fill:#87CEEB,stroke:#000,stroke-width:2px;
  style D fill:#87CEEB,stroke:#000,stroke-width:2px;
  style E fill:#FF6347,stroke:#000,stroke-width:2px;
  style F fill:#87CEEB,stroke:#000,stroke-width:2px;
  style G fill:#87CEEB,stroke:#000,stroke-width:2px;
  style H fill:#98FB98,stroke:#000,stroke-width:2px;
  style I fill:#FF6347,stroke:#000,stroke-width:2px;

