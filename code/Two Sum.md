```python
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        dict = {}
        for i,n in enumerate(nums):
            m = target - n
            if m in dict:
                return [dict[m], i]
            else:
                dict[n] = i
```

遍历数组，然后用字典建立值和键的映射。

