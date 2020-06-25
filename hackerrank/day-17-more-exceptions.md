https://www.hackerrank.com/challenges/30-abstract-classes/problem

```python
#Write your code here
class Calculator:
    def __init__(self):
        pass

    def power(self, n, p):
        try:
            if any([n < 0, p < 0]):
                raise ValueError
            else:
                return n**p
        except ValueError:
            return "n and p should be non-negative"

myCalculator=Calculator()
T=int(input())
for i in range(T):
    n,p = map(int, input().split())
    try:
        ans=myCalculator.power(n,p)
        print(ans)
    except Exception as e:
        print(e)   
```
