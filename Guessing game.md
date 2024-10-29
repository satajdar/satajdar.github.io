## Guessing game

'''mermaid
flowchart TD
A[Start] --> B[Initialize secret number]
    B --> C[Prompt player to guess]
    C --> D{Is the guess correct?}
    D -->|Yes| E[Player wins]
    D -->|No| F{Is the guess too high?}
    F -->|Yes| G[Hint: Too high]
    F -->|No| H[Hint: Too low]
    G --> I[Prompt for new guess]
    H --> I
    I --> D
    E --> J[End]
