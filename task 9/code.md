
  **Problem:** Check subject min, aggregate cutoff, rank with tie-break maths.

**Algorithm:** 1.Read c min cutoff 2.Check each subject>=min 3.agg>=cutoff eligible 4.Sort desc agg, maths

**Flowchart:**
```mermaid
    A[Start] --> B[Input]
    B --> C[eligible empty]
    C --> D{Loop}
    D -->|Yes| E[Read student]
    E --> F{Check min}
    F -->|Fail| G[Skip]
    F -->|Pass| H[Check cutoff]
    H -->|Pass| I[Add to list]
    H -->|Fail| G
    I --> G
    G --> D
    D -->|No| J[Sort]
    J --> K[Print]
    K --> L[End]
```
Sample Input 1:
3
40
180
Aman
80
70
60
Riya
90
85
80
Karan
50
40
30

Sample Output 1:
Riya 255
Aman 210

