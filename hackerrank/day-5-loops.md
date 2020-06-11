https://www.hackerrank.com/challenges/30-loops/problem

```python
#!/bin/python3

import math
import os
import random
import re
import sys



if __name__ == '__main__':
    n = int(input())

    print("\n".join([f"{n} x {i} = {n * i}" for i in range(1, 11)]))
```