Problem Solving Statement:
Input total classes and attended classes to find current percentage. Calculate minimum consecutive classes needed to reach threshold using formula.

Algorithm:
1.Read total, attended, threshold
2.current = attended/total_100
3.If current >= threshold required = 0
4.Else required = ceil((threshold_total - attended_100)/(100-threshold))
5.Print current and required

Flowchart:
``` mermaid

    A[Start] --> B[Read total, attended, threshold]
    B --> C[current = attended/total*100]
    C --> D{current >= threshold?}
    D -- Yes --> E[req=0]
    D -- No --> F[req=ceil((threshold*total/100 - attended)/(1-threshold/100))]
    E --> G[Print current, req]
    F --> G
    G --> H[End]
```
sample input:
100
65
75

sample output:
65.00
40
