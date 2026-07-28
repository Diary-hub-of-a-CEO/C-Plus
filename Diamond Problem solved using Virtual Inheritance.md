#include

using namespace std;

class Person {

protected:

string name;

int personID;

public:

Person() : name("Unknown"), personID(0) {

cout << "Person constructor called" << endl;

}

void setDetails(string n, int id) {

name = n;

personID = id;

}

void introduce() {

cout << "Name: " << name << endl;

cout << "Person ID: " << personID << endl;

}

};

class Teacher : virtual public Person {

protected:

string staffID;

string department;

public:

Teacher() : staffID("T000"), department("General") {

cout << "Teacher constructor called" << endl;

}

void setTeacher(string sid, string dept) {

staffID = sid;

department = dept;

}

void showTeacher() {

cout << "Staff ID: " << staffID << endl;

cout << "Department: " << department << endl;

}

};

class Student : virtual public Person {

protected:

int rollNo;

string faculty;

public:

Student() : rollNo(0), faculty("BIT") {

cout << "Student constructor called" << endl;

}

void setStudent(int r, string f) {

rollNo = r;

faculty = f;

}

void showStudent() {

cout << "Roll No: " << rollNo << endl;

cout << "Faculty: " << faculty << endl;

}

};

class TeachingAssistant : public Teacher, public Student {

public:

TeachingAssistant() {

cout << "Teaching Assistant constructor called" << endl;

}

void display() {

introduce();

showTeacher();

showStudent();

}

};

int main() {

TeachingAssistant ta;

ta.setDetails("Sashwat Khatiwada", 101);

ta.setTeacher("T101", "Computer Science");

ta.setStudent(25, "BIT");

cout << "\\n----- Details -----" << endl;

ta.display();

return 0;

}