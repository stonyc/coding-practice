https://www.hackerrank.com/challenges/30-scope

```python
class Difference:
    def __init__(self, a):
        self.__elements = a

    # Add your code here
    def computeDifference(self):
        arr = sorted(self.__elements)
        self.maximumDifference = arr[-1] - arr[0]

# End of Difference class

_ = input()
a = [int(e) for e in input().split(' ')]

d = Difference(a)
d.computeDifference()

print(d.maximumDifference)
```
