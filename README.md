# Code-1
# Code for linked list reversal
class node:

    def __init__(self,data):
        self.data=data
        self.next=None
# Defining a class called as linked_list 
class linked_list:

    def __init__(self):
        self.head=None


    def insert(self,new_data):

        new_node=node(NEW-DATA)
        temp=self.head

        while(temp!=None and temp.next!=None):
            temp=temp.next

        if(temp!=None):
            temp.next=new_node

        else:
            temp=new_node
            self.head=new_node

    def print_list(self):

        temp=self.head

        while(temp):

            print(temp.data)
            temp=temp.next

    def reverse(self):

        
        prev = None
        current = self.head
        while(current is not None):
            next = current.next
            current.next = prev
            prev = current
            current = next
        self.head = prev

        


if(__name__=='__main__'):

    llist=linked_list()
    llist.insert(1)
    llist.insert(2)
    llist.insert(3)
    llist.insert(4)
    llist.insert(5)
    print("The linked list is given as:")
    llist.print_list()
    llist.reverse()
    print("The reversed linked list is given as:")
    llist.print_list()

        
        
    
        
