#include

using namespace std;

class base {

public:

void display() {

cout << "I am base class" << endl;

}

};

class derived : public base {

public:

void display() {

cout << "I am derived class" << endl;

}

};

int main() {

base \*ptr;

derived d;

ptr = &d; // Base pointer points to derived object

ptr->display(); // Calls base class display()

return 0;

}