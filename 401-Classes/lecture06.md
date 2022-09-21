# Readings: Stack and Queues #

## What's the difference between Stack and Queue? ##
| Stack | Queue |
| ----------- | ----------- |
| The stack is based on LIFO(Last In First Out) principle | The queue is based on FIFO(First In First Out) principle. |
| Insertion Operation is called Push Operation | 	Insertion Operation is called Enqueue Operation |
| Deletion Operation is called Pop Operation | Deletion Operation is called Dequeue Operation |
| Push and Pop Operation takes place from one end of the stack | Enqueue and Dequeue Operation takes place from a different end of the queue |
| The most accessible element is called Top and the least accessible is called the Bottom of the stack | The insertion end is called Rear End and the deletion end is called the Front End.  |

You can find more differences from the [reference](https://favtutor.com/blogs/stack-vs-queue)


## What is Stacks and how to use it? ##
Stack is a data structure in which the element added last is removed first. It follows Last In First Out (LIFO) principle.

1. push(value) — This method will insert the value at one end of the Stack
2. pop() — This method will remove the value from the same end of the Stack at which it was inserted.

- The most important thing to remember in the stack data structure is that it stores the elements of the same data type only.

- Note: As unshift() and shift() method will insert and delete in the beginning of the Stack so they require entire array to be reindexed. Hence it’s not a good approach.

### Condition to Check if Stack is Empty ###
```
int Empty() 
{ 
if(top==-1) 
return 1; 
else return 0; 
}
```

### Condition to Check if Stack is Full ###
```
int Full()
{
    if(top==MAX-1)
        return 1;
    else
        return 0;
}
```


### Application of Stack Data Structure ###
There are many applications of stack data structure in real life. Some of them are as given below:

1. Stack is used for expression evaluation
2. Stack is used for parenthesis matching while working with expressions.
3. Stack is used in expression conversion. For example, infix to postfix or prefix to postfix
4. Stack is used in memory management
5. It is used in java virtual machine
6. It is used for the Backtracking problem-solving method
7. It is used in string parsing or string reversal. 
8. Stack is used to matching the HTML tags in web development
9. Stack is also used in function call for recursive functions. 



## What is Queue? ##
Queue is a data structure in which the element which is added first is removed first. It follows First In First Out (FIFO) principle. 

1. enqueue(value) — This method will insert the value at one end of the Queue.
2. dequeue() — This method will remove the value from the other end of the Queue.

### Condition to Check if Queue is Empty ###
```
int Empty()
{
    if(front==-1 || front==rear+1)
        return 1;
    else
        return 0;
}
```

### Condition to Check if Queue is Full ###
```
int Full()
{
    if(rear==MAX-1)
        return 1;
    else
        return 0;
}
```

### Application of Queue Data Structure ###
There are many applications of queue data structure in real life. Some of them are as given below:

1. The queue is used as a waiting list when the resource is to be shared with multiple systems. For example, CPU scheduling or disk scheduling
2. It is used in the operating system for FCFS scheduling, semaphores, buffer for devices and spooling the printers
3. Queues are used in routers and switches 
4. In networking, the queue is used when data is transferred asynchronously 
5. Used in maintaining the playlist in media players
6. Used to handle interrupts in the operating system
7. The queue is used in the round-robin scheduling algorithm


### *[Source01](https://medium.com/globant/implementing-stack-and-queue-in-js-600c81a92120)*  *[Source02](https://blog.sessionstack.com/how-javascript-works-stacks-and-queues-tips-for-efficient-implementation-8072a130380b)*
