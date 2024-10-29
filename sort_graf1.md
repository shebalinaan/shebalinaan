```mermaid
flowchart TD
A(["selection_sort(list)"])
    A --> B["len(list)"]
    B --> C{{"i in range(n-1)"}}
    C-->Q["min = i"]
    Q -->  E{{"j in range(i+1, n)"}}
    E --> F{"list[j] < list[min]"}
    F -->|true| G["min = j"]
    F--> |false| E
    E--> K{"min != i "}
    G-->E
    K-->|true|M["list[i], list[min] = list[min], list[i]"]
    M-->C
    K--> |false|C
    C--> N["print(list)"]
style Сортировка fill: yellow,stroke:orange;
style Шебалина_Анастасия_1367 fill: plum,stroke:red;
style A fill: pink,stroke:red,stroke-width:2px;
style N fill: pink,stroke:red,stroke-width:2px;
style C fill: aquamarine,stroke:blue,stroke-width:2px;
style E fill: aquamarine,stroke:blue,stroke-width:2px;
style F fill: coral,stroke:red,stroke-width:2px;
style K fill: coral,stroke:red,stroke-width:2px;
style B fill: khaki,stroke:brown,stroke-width:2px;
style G fill: khaki,stroke:brown,stroke-width:2px;
style Q fill: khaki,stroke:brown,stroke-width:2px;
style M fill: khaki,stroke:brown,stroke-width:2px;
