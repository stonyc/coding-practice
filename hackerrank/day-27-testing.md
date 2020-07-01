https://www.hackerrank.com/challenges/30-testing

```python
class TestDataEmptyArray():

    @staticmethod
    def get_array():
        return []

class TestDataUniqueValues():

    @staticmethod
    def get_array():
        return [1, 2, 3, 4, -9, 5]

    @staticmethod
    def get_expected_result():
        return 4

class TestDataExactlyTwoDifferentMinimums():

    @staticmethod
    def get_array():
        return [1, 2, 3, 4, -9, 5, -9, 6]

    @staticmethod
    def get_expected_result():
        return 4
```
