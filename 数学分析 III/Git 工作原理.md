---
date: 2024-07-14
---
```mermaid
graph LR
A["工作区"]
B["暂存区"]
C["本地仓库"]
D["远程仓库"]

A -->|"git add"| B 
B -->|"git commit"| C
C -->|"git push"| D
D --> |"git pull"| C
```
