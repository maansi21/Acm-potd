    class Solution {
    public:
        int maxProfit(vector<int>& prices) {
            int min_price=INT_MAX;
            int maxProfit=0;
            for(int i=0;i<prices.size();i++){
                if(prices[i]<min_price){
                    min_price=prices[i];
                }
                else{
                    int profit=prices[i]-min_price;
                    if(profit>maxProfit){
                        maxProfit=profit;
                    }
                }
               
            }
             return maxProfit;
        }
    };
<img width="1360" height="621" alt="image" src="https://github.com/user-attachments/assets/e29fa8f0-7fef-4784-8dae-f5882a9903b6" />
