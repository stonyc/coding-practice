```python
# Find the node:
def Solve(N, B):
    nodes = dict(zip(range(1,N+1), B))
    edges = []
    for node in nodes:
        count = 0
        start = node
        current = node
        for i in range(N):
            if current == start and i > 0:
                break
            else:
                count += 1
                current = nodes[current]
        edges.append(count)
    return edges.index(max(edges)) + 1

N = 7
for i in range(100):
    lst = list(range(1,N+1))
    random.shuffle(lst)
    Solve(N, lst)
```