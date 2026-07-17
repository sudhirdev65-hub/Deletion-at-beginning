class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
n1=Node("oorum blood")
n2=Node("thee ithuThalapathy")
n3=Node(" Unga vijay")
n4=Node("TVK flag anthem")
n5=Node(" melliname")
n6=Node(" Sakkarai nilave")
n1.next=n2
n2.next=n3
n3.next=n4
n4.next=n5
n5.next=n6
head=n1
def display(head):
     temp=head
     while temp is not None:
         print(temp.data,end="->")
         temp=temp.next
     print("None")
print("Original Linked List")
display(head)
print("Deletion at Beginning")
head=head.next
display(head)