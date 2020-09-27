```
struct ListNode* deleteNode(struct ListNode* head, int val){
    if(head==NULL) return NULL;
    if(head->val==val) return head->next;
    struct ListNode*cur=head;
    while (cur->next!=NULL){
        if(cur->next->val!=val)
            cur=cur->next;
        else
        cur->next=cur->next->next;
    
    }
   
    return head;
}
```