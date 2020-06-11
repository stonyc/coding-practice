https://www.hackerrank.com/challenges/30-review-loop/problem

```python
def parse(string):
    evens = ""
    odds = ""
    for i in list(range(len(string)))[::2]:
        evens += string[i]
    for j in list(range(len(string)))[1::2]:
        odds += string[j]
    print(f"{evens} {odds}")

# Enter your code here. Read input from STDIN. Print output to STDOUT
N = int(input())
for i in range(N):
    s = str(input())
    parse(s)
```