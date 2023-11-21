```mermaid
graph TD;
  subgraph Platform
    A[Platform]
    B[Show Products based on Reseller Level]
    C[Apply Reseller-specific Discount]
    D[Reseller Selects Products]
    E[Add Products to Cart]
    F[View Shopping Cart]
    G[Modify Cart]
    H[Reseller Places Order]
    I[Backend Validates Cart]
    J[Generate Payment Link]
    K[Hold Stock of Selected Products]
    L[Reseller Makes Payment]
    M[Integrate with Courier]
    N[Order Shipped]
  end

  subgraph Reseller
    O[Reseller]
    P[Cancel Order]
  end

  subgraph Backend
    Q[Backend]
    R[Validate Cart]
    S[Generate Payment Link]
    T[Release Stock on Cancellation]
  end

  A -->|Reseller Interaction| B
  B --> C
  C -->|Show Discounted Products| D
  D -->|Reseller Chooses Products| E
  E -->|Add to Cart| F
  F -->|View Cart| G
  G -->|Modify Cart| H
  H -->|Places Order| I
  I -->|Validation Result| S
  S --> J
  J --> K
  K -->|Payment Confirmation| L
  L -->|Payment Confirmation| M
  M --> N
  O -->|Decides to Cancel| P
  P --> T
  T -->|Stock Released| B
