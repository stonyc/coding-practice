https://www.hackerearth.com/practice/python/getting-started/input-and-output/practice-problems/golf/jadoo-and-dna-transcription/

```python
'''
# Sample code to perform I/O:

name = input()                  # Reading input from STDIN
print('Hi, %s.' % name)         # Writing output to STDOUT

# Warning: Printing unwanted or ill-formatted data to output will cause the test cases to fail
'''

# Write your code here
T = {"A":"U","C":"G","G":"C","T":"A"}
try:
    K = ""
    for L in input():
        K += T[L]
    print(K)
except:
    print("Invalid Input")
```