class Solution {
public:
    int removeDuplicates(vector<int>& nums) {
        if(nums.size()==0){
            return 0;
        }
        int i=0;
        for(int j=1;j<nums.size();j++){
            if(nums[j]!=nums[i]){
                i++;
                nums[i]=nums[j];

            }
        }
        return i+1;
    }
};
<img width="1360" height="621" alt="image" src="https://github.com/user-attachments/assets/391a391a-f1dd-4da2-8034-476a7b7ed68a" />
