https://www.hackerrank.com/challenges/30-sorting

```python
#!/bin/python3

import sys

n = int(input().strip())
a = list(map(int, input().strip().split(' ')))
# Write Your Code Here
nswaps = 0
for i in range(len(a)):
    for j in range(len(a)-1):
        if a[j] > a[j+1]:
            first = a[j+1]
            second = a[j]
            a[j] = first
            a[j+1] = second
            nswaps += 1
print(f"Array is sorted in {nswaps} swaps.")
print(f"First Element: {a[0]}")
print(f"Last Element: {a[-1]}")
```
