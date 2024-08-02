## Конфликт при слиянии веток    
Когда сразу несколько членов команды вносят изменения в один и тот же фрагмент проекта в разных ветках, при слиянии могут происходить конфликты.

Допустим, вы решили отредактировать заголовок в тексте и исправить опечатки. В этот момент ваш коллега поменял тот же самый заголовок в соседней ветке и влил изменения в main.    
После завершения работы вы делаете финальный коммит в своей ветке, переходите в основную и пытаетесь выполнить слияние. Но в терминале ошибка. На схеме эта ситуация может выглядеть так.

```mermaid
flowchart TD
A1(You) 
A1 -->|git branch| B1(Your branch)
B1 --> |Внес правки в test.txt| C1(Your branch)
C1 -->|git merge| D2
    
A2(Main) --- C2(Coworker's merge) --- D2(Your merge – conflict)

A3(Coworker)
A3 -->|git branch| B3(Coworker's branch)
B3 -->|Внес правки в test.txt| C3(Coworker's branch)
C3 --> |git merge|C2

style C2 fill:#34b963
style D2 fill:#ff2400
```
### git scheme
```mermaid
    gitGraph
commit id: "create test.txt"
commit id: "add title and description"
branch "Coworker's branch"
branch "Your branch"
checkout "Coworker's branch"
commit id: "change title to test.txt"
checkout "Your branch"
commit id: "change title to test.txt too"
checkout main
merge "Coworker's branch" id: "coworker's merge"
merge "Your branch" id: "your merge – conflict" type: REVERSE
```