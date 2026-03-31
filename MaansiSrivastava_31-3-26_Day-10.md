    class Solution {
    public:
        ListNode* middleNode(ListNode* head) {
            ListNode* slow = head, *fast = head;
            while (fast && fast->next) {
                slow = slow->next;
                fast = fast->next->next;
            }
            return slow;
        }
    };
<img width="1360" height="624" alt="image" src="https://github.com/user-attachments/assets/d7595c2a-d21b-44c5-9f6d-7f131310b0db" />
