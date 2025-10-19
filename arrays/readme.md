
# largest number

```python
def solve1(nums):
    n=len(nums)
    ans=-1
    for i in range(n):
        flag=False
        for j in range(n):
            if(nums[i]>=nums[j]):
                continue
            else:
                flag=True
        if(flag==False):
            ans=nums[i]
            break
    return ans

def solve2(nums):
    n=len(nums)
    ans=-1
    for i in range(n):
        flag=False
        for j in range(n):
            if(nums[i]<nums[j]):
                flag=True
        if(flag==False):
            ans=nums[i]
            break
    return ans

class Solution:
    def largestElement(self, nums):
        n=len(nums)
        ans=float('-inf')
        for i in range(n):
            if(nums[i]>ans):
                ans=nums[i]
        return ans


nums=[2,3,4,6,2]
print(solve1(nums))
print(solve2(nums))
```
