class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
       unordered_map<int, int> mp;
       for(int i=0;i<nums.size();i++){
        int comp=target-nums[i];
         if(mp.count(comp)){
        return{mp[comp],i};
       }
        mp[nums[i]]=i;
       }
      
      
        return{};
    }
};
<img width="1358" height="626" alt="image" src="https://github.com/user-attachments/assets/d2602244-5b66-4825-a78b-89ed32218799" />
