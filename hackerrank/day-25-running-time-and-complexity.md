https://www.hackerrank.com/challenges/30-running-time-and-complexity

```python
import math

def check_prime(num):
    if num == 1:
        return "Not prime"
    sq = int(math.sqrt(num))
    for j in range(2, sq+1):
        if num % j == 0:
            return "Not prime"
    return "Prime"

# Enter your code here. Read input from STDIN. Print output to STDOUT
N = int(input())
for i in range(N):
    num = int(input())
    print(check_prime(num))
```
