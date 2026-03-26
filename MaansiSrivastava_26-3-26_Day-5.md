class Solution {
public:
    void moveZeroes(vector<int>& nums) {
        int j=0;
        for(int i=0;i<nums.size();i++){
            if(nums[i]!=0){
                swap(nums[i],nums[j]);
                j++;
            }
            
        }
}
};
<img width="1351" height="620" alt="image" src="https://github.com/user-attachments/assets/1c018f99-037e-44a1-b0dd-8bcf314939e3" />
