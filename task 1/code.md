**Problem Solving Statement:** Calculate current attendance % and min consecutive classes needed to reach threshold.

**Algorithm:**
1. Read total, attended, threshold
2. current=attended/total*100
3. If current>=threshold req=0 else formula

**Flowchart:**
```mermaid
flowchart TD
    A[Start]-->B[Read total attended threshold]
    B-->C[current=attended/total*100]
    C-->D{current>=threshold}
    D--Yes-->E[req=0]
    D--No-->F[req=formula]
    E-->G[Print]
    F-->G
    G-->H[End]
```

Sample Input 1:
100
65
75

Sample Output 1:
65.00
40

