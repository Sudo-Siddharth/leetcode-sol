/**
 *     ListNode *next;
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     ListNode(int x) : val(x), next(NULL) {}
 * };
 */
class Solution {
public:
    ListNode* addTwoNumbers(ListNode* l1, ListNode* l2) {
        int car=0,f=0;
        ListNode *l5,*l6;
        while(l1!=NULL && l2!=NULL)
        {
                car=(l1->val+l2->val+car);
            ListNode *l4=new ListNode(car%10);
            car=(car-(l4->val))/10;
                l1=l1->next;
                l2=l2->next;
            if(f==0)
            {
                l5=l4;
                l6=l4;
                f=1;
            }
            else
            {
            l5->next=l4;
            l5=l5->next;
            }
        }
        while(l1!=NULL)
        {
            car=(l1->val+car);
            ListNode *l4=new ListNode(car%10);
            car=(car-(l4->val))/10;
            l1=l1->next;
            l5->next=l4;
            l5=l5->next;
        }
        while(l2!=NULL)
        {
            car=(l2->val+car);
            ListNode *l4=new ListNode(car%10);
            car=(car-(l4->val))/10;
            l2=l2->next;
            l5->next=l4;
            l5=l5->next;
        }
        if(car!=0)
        {
            ListNode *l4=new ListNode(car%10);
            l5->next=l4;
            
        }
        return l6;
    }
};
