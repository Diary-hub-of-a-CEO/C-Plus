#include

using namespace std;

class A{

public:

void display() { cout << "I am Class A " << endl; }

};

class B : public A {

public:

void display() { cout << " I am class B" << endl; }

};

int main() {

B b1;

b1.display();

return 0;

}