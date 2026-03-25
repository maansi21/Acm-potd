class Solution {
public:
    int missingNumber(vector<int>& nums) {
        int n=nums.size();
        int xor1=0, xor2=0;

        for(int i=0;i<n;i++){
            xor1^=nums[i];
            xor2^=i;
        }
       xor2 ^= n;
        return xor1^xor2;
    }
};
<img width="1348" height="619" alt="image" src="https://github.com/user-attachments/assets/94da6a57-7acd-4917-bca9-5e7932bbb038" />
