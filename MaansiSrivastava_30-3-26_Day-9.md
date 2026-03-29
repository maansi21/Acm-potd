    class Solution {
    public:
        bool hasCycle(ListNode *head) {
            if (!head) return false;
            ListNode *slow = head, *fast = head;
            while (fast && fast->next) {
                slow = slow->next;
                fast = fast->next->next;
                if (slow == fast) return true;
            }
            return false;
        }
    };
<img width="1365" height="621" alt="image" src="https://github.com/user-attachments/assets/b7532e8b-aa14-4624-8583-4f6b401fa464" />
