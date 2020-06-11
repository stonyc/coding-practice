https://www.hackerrank.com/challenges/time-conversion/problem

```python
#!/bin/python3

import os
import sys

#
# Complete the timeConversion function below.
#
def timeConversion(s):
    #
    # Write your code here.
    #
    hours, mins, secs = s.split(":")
    secs, xm = secs[:2], secs[2:]
    if xm == "AM" and hours == "12":
        hours = "00"
    if xm == "PM" and hours != "12":
        hours = int(hours) + 12
    return f"{hours}:{mins}:{secs}"

if __name__ == '__main__':
    f = open(os.environ['OUTPUT_PATH'], 'w')

    s = input()

    result = timeConversion(s)

    f.write(result + '\n')

    f.close()
```