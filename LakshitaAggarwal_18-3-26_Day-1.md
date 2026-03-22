class Solution {
public:
    int removeDuplicates(vector<int>& nums) {
        int i=0,j=1;

        while(j<nums.size()){
            if(nums[i]!=nums[j]){
                i++;
                swap(nums[j],nums[i]);
            }
            j++;
        }

        return i+1;
    }
        

};
