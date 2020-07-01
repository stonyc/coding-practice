https://www.hackerrank.com/challenges/30-nested-logic

```python
rd, rm, ry = list(map(int, input().rstrip().split()))
dd, dm, dy = list(map(int, input().rstrip().split()))

if ry > dy:
    print(10000)
elif ry == dy and rm > dm:
    print(f"{(rm-dm)*500}")
elif ry == dy and rm == dm and rd > dd:
    print(f"{(rd-dd)*15}")
else:
    print(0)
```
