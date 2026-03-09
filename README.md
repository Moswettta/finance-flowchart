graph TD
    A([Start]) --> B[User Earns Income];
    B --> C[Record Income Manually<br>(e.g., in a notebook)];
    C --> D[Record Daily Expenses Manually];
    D --> E[Manually Calculate Totals<br>(Sum income, sum expenses)];
    E --> F[Review Financial Records];
    F --> G{Are Records Accurate?};
    
    subgraph Error Correction Loop
        G -- No --> H[Find & Correct Errors];
        H --> E;
    end

    G -- Yes --> B;

    style H fill:#f8d7da,stroke:#c87179,stroke-width:2px
    style A fill:#d4edda,stroke:#5c9e6e,stroke-width:2px
