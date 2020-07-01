https://www.hackerrank.com/challenges/30-linked-list-deletion

```python
def removeDuplicates(self,head):
    h = head
    while head.next is not None:
        if head.next.data == head.data:
            head.next = head.next.next
        else:
            head = head.next
    return h
```
