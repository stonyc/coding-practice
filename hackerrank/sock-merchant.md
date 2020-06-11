https://www.hackerrank.com/challenges/sock-merchant/problem

```python
#!/bin/python3

import math
import os
import random
import re
import sys

# Complete the sockMerchant function below.
def sockMerchant(n, ar):
    npairs = 0
    for color in set(ar):
        ncolor = sum([1 for sock in ar if sock == color])
        npairs += ncolor // 2
    return npairs

if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    n = int(input())

    ar = list(map(int, input().rstrip().split()))

    result = sockMerchant(n, ar)

    fptr.write(str(result) + '\n')

    fptr.close()
```