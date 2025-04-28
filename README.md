EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

Aim: To write a C program to display stack elements using an array. 

Algorithm:
```
1.Include Necessary Header Files
2.Declare Global Variables
3.Define the Display Function
4.Main Function (or Other Relevant Code)
5.Initialize the stack and top as needed.
6.Perform stack operations (push, pop, etc.).
7.Use the display function to visualize the stack's contents
```
Program:
```
char stack[100];
int top,i;
void display()
{
    for(i=top;i>=0;i--)
    {
        printf("%c ",stack[i]);
    }
    if(top ==-1)
    {
        printf("stack is empty\n");
    }
}
```
Output:

![mod11](https://github.com/user-attachments/assets/b98f92bf-f681-4405-a9b6-584aa9f5de4b)



Result: Thus, the program to display stack elements using an array is verified successfully.

EXP NO:12 PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY. 

Aim: To create a C program to push the given element in to a stack using array.
Algorithm:
```
Declare global variables for the stack size, top index, and the stack itself.
Define the push function to add a floating-point number to the stack.
Initialize the stack size, top index, and the stack itself.
Call the push function as needed.
```
Program:
```
int size=3,top=-1,stack[100];
void push (int data)
{
    stack[++top]=data;
}
```

Output:
![mod12](https://github.com/user-attachments/assets/249a9544-1248-4f6c-8cf9-90f98b1e3130)



Result: Thus, the program to push the given element in to a stack using array is verified successfully

EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.

Aim: To write a C program to display queue elements using array

Algorithm:
```
Declare global variables for the queue, rear, front, and iteration.
Define the display function to print the elements of the queue.
Initialize the queue, rear, and front as needed.
Call the display function and perform other queue operations as needed.
```
Program:
```
float queue[50];
int front,rear;
void display()
{
    if(front==-1 && rear==-1)
    {
        printf("No elements to display\n");
    }
    else
    {
        for(int i=front;i<=rear;i++)
        {
            printf("%.1f\n",queue[i]);
        }
    }
    
}

```
Output:

![mod13](https://github.com/user-attachments/assets/ae1a16be-2e24-45c5-841d-f467ff96a6ea)


Result: Thus, the program to display queue elements using array is verified successfully.

EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.

Aim: To write a C program to insert elements in queue using array.

Algorithm:
```
Declare global variables for the size, rear, front, and the queue itself.
Define the enqueue function to add a float to the queue.
Initialize the rear, front, and size of the queue as needed.
Call the enqueue function as needed.
```

Program:
```
int front;
int rear;
char queue[50];
void enqueue(char data)
{
    if(front==-1)
    {
        front=0;
    }
    rear++;
    queue[rear]=data;
}
```

Output:

![mod14](https://github.com/user-attachments/assets/23dfa85f-ffc1-47d8-9f3c-c29da3739d82)


Result: Thus, the program to insert elements in queue using array is verified successfully.

EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY

Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:
```
Check if the Queue is Empty o If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
Delete the Front Element o If the queue is not empty, the element at the front index is deleted. o Increment the front pointer by 1 to remove the element and point to the next element in the queue.
Check if the Queue Becomes Empty After Deletion: o After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
End the Function.
```
Program:
```
float queue[50];
int front, rear;
void dequeue()
{
    if(front==-1 && rear==-1){
        printf("Queue Underflow.\n");
    }
    else if(front<rear)
    {
        front++;
    }
    else
    {
        front=-1;
        rear=-1;
        printf("No elements to display");
    }
}
```
Output:
![mod15](https://github.com/user-attachments/assets/24784b5d-6e9a-4cfa-a966-3ae547d29120)


Result: Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
