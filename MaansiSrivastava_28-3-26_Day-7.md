    class Solution {
    public:
        void rotate(vector<int>& nums, int k) {
            int n=nums.size();
            k=k%n;
            reverse(nums.begin(),nums.end());
            reverse(nums.begin(),nums.begin()+k);
            reverse(nums.begin()+k,nums.end());
        }
    };
<img width="1348" height="615" alt="image" src="https://github.com/user-attachments/assets/74e1cd32-1fac-4539-b6e0-322b089562ad" />
