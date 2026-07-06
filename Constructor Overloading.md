#include

#include

using namespace std;

class Student {

private:

string name;

int age;

public:

// Default Constructor

Student() {

name = "Unknown";

age = 0;

}

// Constructor with name only

Student(string n) {

name = n;

age = 0;

}

// Constructor with name and age

Student(string n, int a) {

name = n;

age = a;

}

// Display Function

void displayInfo() {

cout << "Name: " << name << endl;

cout << "Age : " << age << endl;

cout << "-------------------" << endl;

}

};

int main() {

Student student1;

Student student2("Anya");

Student student3("Harsh", 20);

student1.displayInfo();

student2.displayInfo();

student3.displayInfo();

return 0;

}