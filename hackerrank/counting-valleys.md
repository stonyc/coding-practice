https://www.hackerrank.com/challenges/counting-valleys/problem

```python
#!/bin/python3

import math
import os
import random
import re
import sys

# Complete the countingValleys function below.
def countingValleys(n, s):
    level = 0
    nval = 0
    for  move in s:
        if move == "U":
            level += 1
            if level == 0:
                nval += 1
        else:
            level -= 1
    return nval
    
if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    n = int(input())

    s = input()

    result = countingValleys(n, s)

    fptr.write(str(result) + '\n')

    fptr.close()
```