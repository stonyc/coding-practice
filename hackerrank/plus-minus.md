https://www.hackerrank.com/challenges/plus-minus/problem

```python
#!/bin/python3

import math
import os
import random
import re
import sys

# Complete the plusMinus function below.
def plusMinus(arr):
    print(f"{len([n for n in arr if n > 0]) / len(arr):.5f}")
    print(f"{len([n for n in arr if n < 0]) / len(arr):.5f}")
    print(f"{len([n for n in arr if n == 0]) / len(arr):.5f}")

if __name__ == '__main__':
    n = int(input())

    arr = list(map(int, input().rstrip().split()))

    plusMinus(arr)
```