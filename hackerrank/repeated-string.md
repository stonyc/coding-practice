https://www.hackerrank.com/challenges/repeated-string/problem

```python
#!/bin/python3

import math
import os
import random
import re
import sys

# Complete the repeatedString function below.
def repeatedString(s, n):
    N=0
    N=s.count('a')
    N*=n//len(s)
    N+=s[0:n%len(s)].count('a')
    return N
    
if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    s = input()

    n = int(input())

    result = repeatedString(s, n)

    fptr.write(str(result) + '\n')

    fptr.close()
```