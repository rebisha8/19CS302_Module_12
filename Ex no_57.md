# EX 57 C function to perfom push,pop and peek functions in Stack using Linked List.( store float data in stack)
## AIM:
To write a C function to perfom push,pop and peek functions in Stack using Linked List.

## Algorithm
1. Start.
2. Define a variables.
3. Write a functions to perform push, pop,peek,display, in Queue using linked 
list.
4. Read the value using scanf.
5. Ask the user to make an input.
6. Print out the answer.
7. End 

## Program:
```c
struct Node   
{  
int data;  
struct Node *next;  
}*head;
void push(int data)  
{ 
    struct Node*n=(struct Node*)malloc(sizeof(struct Node));
    if(head==NULL)
    {
    n->data=data;
    n->next=NULL;
    head=n;
    }
    else
    
    {
        n->data=data;
        n->next=head;
        head=n;
    }
    
}  
void pop()  
{ 
    struct Node*temp;
    if(head==NULL)
    {
        printf("stack is empty");
        return;
    }
    temp=head;
    head=head->next;
    free(temp);
}  
void display()  
{  
    struct Node*temp;
    if(head==NULL)
    {
        printf("stack is empty");
        return;
    }
    temp=head;
    printf("stack:");
    while(temp!=NULL)
    {
        printf("%d ",temp->data);
        temp=temp->next;
    }
    
}  
void peek()
{
printf("\nstack top:%d\n",head->data);
    
}


```

## Output:
![Screenshot 2025-05-16 211045](https://github.com/user-attachments/assets/05a39d0d-d227-4b16-adbd-349c006a683a)


## Result:
Thus the program was executed and the output was verified successfully.
