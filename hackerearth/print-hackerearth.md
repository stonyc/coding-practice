https://www.hackerearth.com/practice/basic-programming/implementation/basics-of-implementation/practice-problems/algorithm/print-hackerearth/

```python
'''
# Sample code to perform I/O:

name = input()                  # Reading input from STDIN
print('Hi, %s.' % name)         # Writing output to STDOUT

# Warning: Printing unwanted or ill-formatted data to output will cause the test cases to fail
'''

L = int(input())
chars = str(input())

def count_letters(word):
    unique = list(set(list(word)))
    counts = dict(zip(unique, [word.count(letter) for letter in unique]))
    return counts

if len(chars) >= len("hackerearth"):
    # Get the number of letters required to spell hackerearth:
    hacker = count_letters("hackerearth")
    # Get the number of letters in the input:
    test = count_letters(list(chars))
    iters = [test[k]//hacker[k] for k in list(hacker)]
    print(min(iters))
else:
    print(0)
```