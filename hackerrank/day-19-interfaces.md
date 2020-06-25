https://www.hackerrank.com/challenges/30-interfaces

```python
class AdvancedArithmetic(object):
    def divisorSum(n):
        raise NotImplementedError

class Calculator(AdvancedArithmetic):
    def divisorSum(self, n):
        N = []
        for i in range(1, n+1):
            if n % i == 0:
                N.append(i)
        return sum(N)


n = int(input())
my_calculator = Calculator()
s = my_calculator.divisorSum(n)
print("I implemented: " + type(my_calculator).__bases__[0].__name__)
print(s)
```
