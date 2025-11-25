## Ex.No:4
## Ex.Name: Write a CPP Program to insert five character elements in to Stack ADT (use STL for Stack)
## Date: 04/09/2025
## Aim:
To write a C++ program to insert five character elements into Stack ADT using STL.

## Algorithm:
Start the program.
Declare a stack of type char.
Read five character elements from the user.
Insert each element into the stack using push().
Display the elements of the stack by popping them one by one until the stack becomes empty.
Stop the program.
## Program:
```
#include<iostream>
#include<stack>
using namespace std;
int main()
{
    stack<char> stack;
    int n;
    char str;
    cin>>n;
    cout<<"Size of the stack: "<<n<<endl;
    for(int i=0;i<n;i++){
        cin>>str;
        stack.push(str);
    }
    while(!stack.empty()){
        cout<<stack.top()<<" ";
        stack.pop();
    }
}
```
## Output:
<img width="484" height="272" alt="485473903-72c66d2b-bb8c-4c14-99d1-7ce8994fd52e" src="https://github.com/user-attachments/assets/6ae4ef15-a833-4ca1-abdb-59e65b733b54" />

## Result:
The program successfully inserts five character elements into the stack using STL and displays them in LIFO (Last In First Out) order.
