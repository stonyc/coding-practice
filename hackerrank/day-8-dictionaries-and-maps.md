https://www.hackerrank.com/challenges/30-dictionaries-and-maps/problem

```python
import sys

# Enter your code here. Read input from STDIN. Print output to STDOUT
N = int(input())
book = dict()
for i in range(N):
    name, number = input().split()
    book.update(dict(zip([name], [number])))
for line in sys.stdin:
    lookup = line.strip()
    if lookup in book:
        print(f"{lookup}={book[lookup]}")
    else:
        print("Not found")
```
