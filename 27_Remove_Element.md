# Remove Element Lc-27

### Given an integer array nums and an integer val, remove all occurrences of val in nums in-place. The order of the elements may be changed. Then return the number of elements in nums which are not equal to val.



***Code:***
```
    int removeElement(vector<int>& nums, int val) {
        int count=0;
        int j =0;
        for( int i=0; i<nums.size(); i++){
            if(nums[i]!=val){
                 swap(nums[i],nums[j]);
                 j++;
            }
        }
        return j;
    }
```     



>[!TIP]
>use ful information for Remainder

> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.