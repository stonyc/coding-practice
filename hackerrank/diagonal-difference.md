https://www.hackerrank.com/challenges/diagonal-difference/problem

```python
#!/bin/python3

import math
import os
import random
import re
import sys

#
# Complete the 'diagonalDifference' function below.
#
# The function is expected to return an INTEGER.
# The function accepts 2D_INTEGER_ARRAY arr as parameter.
#

def diagonalDifference(arr):
    # Write your code here
    primary = []
    for i in range(len(arr)):
        for j in range(len(arr)):
            if i == j:
                primary.append(arr[i][j])
    secondary = []
    for i in range(len(arr)):
        for j in range(len(arr)):
            if i + j == len(arr) - 1:
                secondary.append(arr[i][j])
    print(primary, secondary)
    return abs(sum(primary) - sum(secondary))

if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    n = int(input().strip())

    arr = []

    for _ in range(n):
        arr.append(list(map(int, input().rstrip().split())))

    result = diagonalDifference(arr)

    fptr.write(str(result) + '\n')

    fptr.close()
```