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
,,,        
