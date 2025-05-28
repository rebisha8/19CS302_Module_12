# EX 60 C function to find the peek element of the queue using linked list.
## AIM:
To write a C function to find the peek element of the queue using linked list.

## Algorithm
1. Start.
2. Define a variables.
3. Write a functions to find peek in Queue using linked list.
4. Read the value using scanf.
5. Ask the user to make an input.
6. Print out the answer.
7. End 

## Program:
```c
struct Node
{
char data;
struct Node *next;
}*front=NULL,*rear=NULL; 
void peek()
{
printf("peek:"); 
printf("%c\n",front->data);
}

```

## Output:
![Screenshot 2025-05-16 211941](https://github.com/user-attachments/assets/252d3c48-1fd7-471e-8c05-48b0e96013bd)




## Result:
Thus the program was executed and the output was verified successfully.
