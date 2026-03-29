    class Solution {
    public:
        bool checkIfExist(vector<int>& arr) {
            unordered_set<int> st;
            for (int num : arr) {
                if (st.count(2 * num) || (num % 2 == 0 && st.count(num / 2))) {
                    return true;
                }
                st.insert(num);
            }
            return false;
        }
    };
    
  <img width="1350" height="611" alt="Screenshot 2026-03-29 162526" src="https://github.com/user-attachments/assets/5d9b3b53-5450-4a8c-8e6a-1539ba4fe8a1" />

