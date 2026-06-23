#include

using namespace std;

class Student {

private:

string name;

int roll;

// static data member

static int count;

public:

Student(string n, int r) {

name = n;

roll = r;

count++;

}

void display() {

cout << "Name: " << name << ", Roll: " << roll << endl;

}

static void showCount() {

cout << "Total Students: " << count << endl;

}

};

int Student::count = 0;

int main() {

Student s1("Ram", 1);

Student s2("Sita", 2);

Student s3("Hari", 3);

s1.display();

s2.display();

s3.display();

// calling static function using class name

Student::showCount();

return 0;

}