1. Two Sum

Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

//Optimal solution using HashMap

 public int[] twoSum(int[] nums, int target) {
              
        HashMap<Integer,Integer> map  = new HashMap();
        
        //Fill HM
        for(int i=0;i<nums.length;i++){
            map.put(nums[i],i);
        }
            
            
        //Searching
         for(int i=0;i<nums.length;i++){ //2 7 11 15  target = 4
            int num = nums[i]; 
            int rem = target - num; 
            if(map.containsKey(rem)){
                int index = map.get(rem);
                if(index==i)continue;
                return new int[]{i,index}; 
            }  
        }
        
        return new int[]{};
        
    }
