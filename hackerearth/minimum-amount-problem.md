Minimum Amount Problem

```python
# Find the minimum:
def solve(S,cnt1,cnt2,cnt3,cost1,cost2,cost3):
    #your code goes here 
    def calculate_energy(n1, n2, n3):
        return (n1*2 + n2*3 + n3*5)
    def calculate_cost(n1, n2, n3):
        return sum([m * n for m, n in zip([n1,n2,n3], costs)])
    # Put inputs into lists:
    counts = [cnt1, cnt2, cnt3]
    costs = [cost1, cost2, cost3]
    pass_costs = []
    for i in range(counts[0]+1):
        for j in range(counts[1]+1):
            for k in range(counts[2]+1):
                E = calculate_energy(i, j, k)
                if E == S:
                    pass_costs.append(calculate_cost(i, j, k))
    try:
        lowest_cost_index = pass_costs.index(min(pass_costs))
        return pass_costs[lowest_cost_index]
    except IndexError:
        return -1

S=int(input())
cnt1,cnt2,cnt3=map(int,input().split(' '))
cost1,cost2,cost3=map(int,input().split(' '))
print(solve(S,cnt1,cnt2,cnt3,cost1,cost2,cost3))
```