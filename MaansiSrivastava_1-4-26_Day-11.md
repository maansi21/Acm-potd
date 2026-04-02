     class Solution {
    public:
        ListNode* mergeTwoLists(ListNode* list1, ListNode* list2) {
            ListNode* dummy = new ListNode(0);
            ListNode* current = dummy;
        
        while (list1 && list2) {
            if (list1->val <= list2->val) {
                current->next = list1;
                list1 = list1->next;
            } else {
                current->next = list2;
                list2 = list2->next;
            }
            current = current->next;
        }
        
        current->next = list1 ? list1 : list2;
        return dummy->next;
    }
};
<img width="1353" height="612" alt="image" src="https://github.com/user-attachments/assets/b73493f2-989b-4e23-81b3-36e2252cb068" />
