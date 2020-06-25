https://www.hackerrank.com/challenges/30-binary-numbers/problem

```python
#!/bin/python3

import math
import os
import random
import re
import sys

def max_ones(N):
    # Get binary representation using bin() then split on zeroes:
    ones = bin(N).split("b")[-1].split("0")
    return max([len(one) for one in ones])

if __name__ == '__main__':
    n = int(input())
    print(max_ones(n))

```
