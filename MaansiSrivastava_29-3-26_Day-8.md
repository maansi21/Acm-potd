    class Solution {
    public:
        ListNode* reverseList(ListNode* head) {
            ListNode* prev=nullptr, *curr=head;
            while(curr){
                ListNode* next=curr->next;
                curr->next=prev;
                prev=curr;
                curr=next;
            }
            return prev;
        }
    };
<img width="1352" height="608" alt="image" src="https://github.com/user-attachments/assets/9f34070c-90a5-48b9-b78a-2774a05dbb03" />
