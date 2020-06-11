https://www.hackerearth.com/practice/basic-programming/input-output/basics-of-input-output/practice-problems/algorithm/seating-arrangement-1/

```python
'''
# Sample code to perform I/O:

name = input()                  # Reading input from STDIN
print('Hi, %s.' % name)         # Writing output to STDOUT

# Warning: Printing unwanted or ill-formatted data to output will cause the test cases to fail
'''

# Write your code here
def get_seat_type(N):
    modulo = (N % 108) % 12
    if modulo in [0,1,6,7]:
        return "WS"
    elif modulo in [2,5,8,11]:
        return "MS"
    else:
        return "AS"

def get_facing_seat(N):
    modulo = N % 12
    if modulo > 0:
        pad = 12 - 2*modulo + 1
    else:
        pad = -11
    return N + pad

T = int(input())
for i in range(T):
    seat = int(input())
    facing_seat = get_facing_seat(seat)
    seat_type = get_seat_type(facing_seat)
    print(str(facing_seat), seat_type)
```