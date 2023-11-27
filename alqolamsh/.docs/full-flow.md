graph TD
    A[Monitoring Dashboard]
    B[Block Sensitive Intent]
    C[Add Entity and Intent]
    D[View Most Used Intent/Entity]
    E[View Exist and Non-Exist Intent]
    F[Monitoring Dashboard]

A -->|Monitor| F
B -->|Block| F
C -->|Add| F
D -->|View| F
E -->|View| F
B -->|Block Sensitive Intent| G{User asks something inappropriate?}
G -->|Yes| I[Return 'Cannot Proceed' Response]
G -->|No| F
