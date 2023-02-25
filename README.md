class Solution {
    public ListNode reverseList(ListNode head) {
        ListNode prev=null;
        
        while(head!=null)
        {
            ListNode temp=head.next;
            head.next=prev;
            prev=head;
            head=temp;
        }
        return prev;//[5,4,3,2,1]

    }
}
