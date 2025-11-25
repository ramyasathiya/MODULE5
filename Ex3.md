## Ex.No:3
## Ex.Name: Write a CPP Program to insert integer elements in to Queue ADT and display size of the queue,and first,Last element of the queue (use STL and set maximum size of the is 100)
## Date: 04/09/2025
## Aim:
To write a C++ program to insert integer elements into a Queue ADT using STL, display the size of the queue, and print the first and last elements. The maximum size of the queue is 100.

## Algorithm:
1.  Start the program.
2.  Declare a queue of integers with maximum size 100.
3.  Read the number of elements to insert.
4.  Check if the number of elements exceeds 100. If yes, restrict input.
5.  Insert each element into the queue using push().
6.  Display the size of the queue using size().
7.  Display the first element using front().
8.  Display the last element using back().
9.  Stop the program.
## Program:
```
#include <iostream>
#include <queue>
using namespace std;
int main()
{
    queue<int> q;
    int n;
    cin>>n;
    for(int i=0;i<n;i++)
    {
        int a;
        cin>>a;
        q.push(a);
    }
    cout<<"Size of the Queue is:"<<n<<endl;
    cout<<"The First Element of the Queue is:"<<q.front()<<endl;
    cout<<"The Last Element of the Queue is:"<<q.back()<<endl;
}
```
## Output:


<img width="793" height="321" alt="485473403-ef0b1e24-664c-45f3-b032-85b0b1a64f10" src="https://github.com/user-attachments/assets/aaec1259-3107-4f0c-80a5-a1a08b0296ab" />

## Result:
The program successfully inserts integer elements into the queue using STL, restricts the maximum size to 100, and displays the size of the queue along with the first and last elements.
