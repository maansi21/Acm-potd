    class Solution {
    public:
        ListNode* deleteDuplicates(ListNode* head) {
            if (!head) return nullptr;
            ListNode* current = head;
            while (current && current->next) {
                if (current->val == current->next->val) {
                    current->next = current->next->next;
                } else {
                    current = current->next;
                }
            }
            return head;
        }
    };
  <img width="1341" height="625" alt="image" src="https://github.com/user-attachments/assets/4479f2c7-13ef-43e6-8fd5-c55dbd39842a" />
