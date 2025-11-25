## Ex.No:5
## Ex.Name: Write a C++ program to illustrate Student Based Multiple inheritance with protected access specifier, find the student total marks.
## Date: 04/09/2025
## Aim:
To write a C++ program to illustrate Student Based Multiple Inheritance with protected access specifier and find the total marks of a student.

## Algorithm:
Start the program.

Create a base class Subject with protected data members for two subject marks and a function to read them.

Create another base class Cocurricular with protected data member for cocurricular points and a function to read it.

Derive a class Student from both Subject and Cocurricular.

In the derived class, define a function to calculate the total marks (sum of subject marks and cocurricular points).

Display the total marks.

Stop the program.

## Program:
```
#include <iostream>
using namespace std;
class SubjectMarks {
protected:
    int mark1, mark2;
public:
    void getMarks(int m1, int m2) {
        mark1 = m1;
        mark2 = m2;
    }
};
class Cocurricular {
protected:
    int points;
public:
    void getPoints(int p) {
        points = p;
    }
};
class Student : public SubjectMarks, public Cocurricular {
public:
    void calculateTotal() {
        int total = mark1 + mark2 + points;
        cout << "The total marks of the students is " << total << endl;
    }
};

int main() {
    Student s;
    int m1, m2, p;

    cin >> m1 >> m2 >> p;

    s.getMarks(m1, m2);
    s.getPoints(p);
    s.calculateTotal();

    return 0;
}
```
## Output:

<img width="696" height="314" alt="485474437-d4bb7809-b683-4ee7-ae99-42b5210de6a3" src="https://github.com/user-attachments/assets/15a89137-242a-49ae-b94e-6741065d1b51" />

## Result:
The program successfully demonstrates multiple inheritance with protected access specifier by calculating and displaying the total marks of a student using subject marks and cocurricular points.
