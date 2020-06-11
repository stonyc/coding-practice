https://www.hackerearth.com/practice/basic-programming/operators/basics-of-operators/practice-problems/algorithm/going-to-office-e2ef3feb/

```python
'''
# Sample code to perform I/O:

name = input()                  # Reading input from STDIN
print('Hi, %s.' % name)         # Writing output to STDOUT

# Warning: Printing unwanted or ill-formatted data to output will cause the test cases to fail
'''

# Write your code here
def solve(D, Oc, Of, Od, Cs, Cb, Cm, Cd):
    Ot = Oc if D <= Of else Oc + (D-Of)*Od
    Ct = Cb + Cm*(D/Cs) + (D*Cd)
    print("Online Taxi" if Ot <= Ct else "Classic Taxi")

D = int(input())
Oc, Of, Od = map(int, input().split(" "))
Cs, Cb, Cm, Cd = map(int, input().split(" "))

solve(D, Oc, Of, Od, Cs, Cb, Cm, Cd)
```