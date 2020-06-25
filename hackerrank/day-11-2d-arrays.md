https://www.hackerrank.com/challenges/30-2d-arrays/problem

```python
#!/bin/python3

import math
import os
import random
import re
import sys

def hourglassSum(arr):
    sums = []
    for i, row in enumerate(arr[:-2]):
        for j, col in enumerate(row[:-2]):
            glass = sum([
                sum(arr[i][j:(j+3)]), 
                arr[i+1][j+1], 
                sum(arr[i+2][j:(j+3)])
                ])
            sums.append(glass)
    return max(sums)

if __name__ == '__main__':
    arr = []

    for _ in range(6):
        arr.append(list(map(int, input().rstrip().split())))

    print(hourglassSum(arr))
```
