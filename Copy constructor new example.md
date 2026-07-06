#include

using namespace std;

class Person {

private:

string name;

int age;

public:

// Parameterized Constructor

Person(string n, int a) {

name = n;

age = a;

}

// Copy Constructor

Person(const Person &source) {

name = source.name;

age = source.age;

}

// Display Function

void displayInfo() {

cout << "Name: " << name << endl;

cout << "Age: " << age << endl;

}

};

int main() {

// Original object

Person p1("Sashwat", 20);

// Copy object

Person p2 = p1;

cout << "Original Person:" << endl;

p1.displayInfo();

cout << "\\nCopied Person:" << endl;

p2.displayInfo();

return 0;

}