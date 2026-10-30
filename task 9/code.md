
  **Problem:** Check subject min, aggregate cutoff, rank with tie-break maths.

**Algorithm:** 1.Read c min cutoff 2.Check each subject>=min 3.agg>=cutoff eligible 4.Sort desc agg, maths

**Flowchart:**
```mermaid
flowchart TD
    A[Start]-->B[Read c min cutoff]
    B-->C[eligible=[] i=0]
    C-->D{i<c}
    D--Yes-->E[Read name m p ch]
    E-->F{m or p or ch < min}
    F--Yes-->G[i++]
    F--No-->H[agg=m+p+ch]
    H-->I{agg>=cutoff}
    I--Yes-->J[Add eligible]
    I--No-->G
    J-->G
    G-->D
    D--No-->K[Sort desc]
    K-->L[Print ranked]
    L-->M[End]
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

