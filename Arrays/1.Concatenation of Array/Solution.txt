class Solution {
    public int[] getConcatenation(int[] nums) {
        
        
        int newSize=2*nums.length;
        int temp[]=new int[newSize];
        
        
        for(int i=0;i<newSize;i++)
        {
            if(i<nums.length)
            {
                temp[i]=nums[i];
            }
            else
            {
                temp[i]=nums[i-nums.length];
            }
            
        }
        
        return temp;
        
    }
}
