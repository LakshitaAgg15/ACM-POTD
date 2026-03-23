
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

<img width="1920" height="1020" alt="Screenshot 2026-03-22 123631" src="https://github.com/user-attachments/assets/ccc83569-2d89-40cf-a672-8846d9a73407" />
