https://www.hackerrank.com/challenges/mini-max-sum/problem

```python
#!/bin/python3

import math
import os
import random
import re
import sys

# Complete the miniMaxSum function below.
def miniMaxSum(arr):
    sorted_arr = sorted(arr)
    print(f"{sum(sorted_arr[:4])} {sum(sorted_arr[1:])}")

if __name__ == '__main__':
    arr = list(map(int, input().rstrip().split()))

    miniMaxSum(arr)
```