PROBLEM STATEMENT:
Given total number of classes conducted, number of classes attended,
and required attendance threshold percentage, calculate:
- Current attendance percentage
- Minimum number of consecutive classes required to reach threshold
If current >= threshold, req = 0
Else req = ceil((threshold/100*total - attended) / (1 - threshold/100))

ALGORITHM:
1. START
2. Read total, attended, threshold
3. current = attended / total * 100
4. IF current >= threshold
5.    req = 0
6. ELSE
7.    numerator = (threshold/100*total) - attended
8.    denominator = 1 - (threshold/100)
9.    req = ceil(numerator / denominator)
10. ENDIF
11. Print current with 2 decimals
12. Print req
13. END

14. 
15. flowchart TD
16. ```mermaid
    A[Start] --> B[Read total, attended, threshold]
    B --> C[Calculate current percentage]
    C --> D{Is current >= threshold?}
    D -- Yes --> E[Set req to 0]
    D -- No --> F[Calculate req with ceil formula]
    E --> G[Print current and req]
    F --> G
    G --> H[End]
    ```
Sample Input 1:
100
65
75
Sample Output 1:
5.00
40
Sample Input 2:
80
70
75
Sample Output 2:
87.50
0
65
75
