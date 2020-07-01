https://www.hackerrank.com/challenges/30-binary-trees

```python
def levelOrder(self,root):
    queue = [root] if root else []
    
    while queue:
        node = queue.pop()
        print(node.data, end=" ")
        if node.left: queue.insert(0, node.left)
        if node.right: queue.insert(0, node.right)
```
