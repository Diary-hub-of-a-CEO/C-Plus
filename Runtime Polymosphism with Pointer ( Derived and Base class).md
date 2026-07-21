#include

using namespace std;

class Base

{

public:

void display()

{

cout << "I am Class A" << endl;

}

};

class Derived : public Base

{

public:

void display()

{

cout << "I am Sashwat" << endl;

}

};

int main()

{

Base \*ptr;

Derived d;

ptr = &d;

ptr->display();

return 0;

}