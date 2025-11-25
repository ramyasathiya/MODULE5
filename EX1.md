## Ex.No:1
## Ex.Name: write a C++ program to implement FCFS algorithm(to read no of.process p1,p2 ,p3 and p4 and its burst time from the user) find out waiting time & Turn Around time of the the process?
## Date: 04/09/2025
## Aim:
To write a C++ program that implements the FCFS algorithm by reading the number of processes and their burst times, then calculating Waiting Time and Turnaround Time for each process.

## Algorithm:
1. Start program.
2. Read burst times of 4 processes into a queue.
3. Initialize wt = 0, ta = 0, counters for totals.
4. For each process in queue:

  •Add wt to total waiting. 
  •Update ta = ta + BT.
  •Add ta to total turnaround.
  •Print process number, BT, WT, TA.
  •Update wt = wt + BT.
  •Remove process from queue.

5. Stop program.
## Program:
```
#include <iostream>
#include <queue>
using namespace std;

int main(){
    cout << "Processes   BT time   WT time   TA time" << endl;
    queue<int> processes;
    int a;
    for(int i=0;i<4;i++){
        cin >> a;
        processes.push(a);
    }
    int wt=0,ta=0,i=1,cn=0,wn=0;
    while(!processes.empty()){
        wn += wt;
        ta+=processes.front();
        cn += ta;
        cout << "       " << i << "       " << processes.front() << "       " << wt << "       " << ta << endl;
        wt+=processes.front();
        processes.pop();
        i++;
    }
}
```
## Output:


<img width="671" height="408" alt="485470405-27e1fcb4-bb82-40d2-8ea5-7c1bc524fd9b" src="https://github.com/user-attachments/assets/238deec5-9515-463e-94f2-3b1d6f02123c" />

## Result:
Thus the program correctly implements FCFS Scheduling.
