https://www.hackerrank.com/challenges/staircase/problem

```python
#!/bin/python3

import math
import os
import random
import re
import sys

# Complete the staircase function below.
def staircase(n):
    stairs = []
    for i, j in zip(list(range(n+1)), list(range(n+1))[::-1]):
        if j == 0:
            pass
        else:
            stairs.append(" "*i + "#"*j)
    # Define a variable for new line:
    newline = "\n"
    print(f"{newline.join([stair for stair in stairs[::-1]])}")

if __name__ == '__main__':
    n = int(input())

    staircase(n)
```