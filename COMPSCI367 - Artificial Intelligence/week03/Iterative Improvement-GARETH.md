 - keep a single "current" [[state(s)]], try to improve it

## Main Idea
- finding a configuration & making it better - If we can make it better, we can update the current state

> n-queens
> ![[Pasted image 20231023175248.png]]
> - assign all variables randomly in the beginning (thus violating several constraints)
> - change 1 variable at a time, trying to reduce the number of violations at each step
> - [Greedy (Best-First) Search](https://www.notion.so/Greedy-Best-First-Search-b1f514fad4bc42baa51cd27494ba1a66?pvs=21) with h = number of constraints violate

> Traveling Salesman Problem
> ![[Pasted image 20231023175238.png]]
