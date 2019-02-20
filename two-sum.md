
## two-sum

``` java
class Solution {
    public int[] twoSum(int[] nums, int target) {
        for(int i = 0; i < nums.length; i++){
            for(int j = i + 1; j < nums.length; j++){
                if(nums[j] == target - nums[i]){
                    return new int[] {i, j};
                }
            }
        }
        return new int[0];
    }

}
```

### 分析

 * Time complexity  : O(n^2)
 * Space complexity : O(1).这个是怎么算的

​       第二种是用的是HashMap算的，有点奇怪，基本功里怎么还混入了数据结构，但时间复杂度能到1。所以怎么能在不适用数据结构情况下完成复杂度1呢