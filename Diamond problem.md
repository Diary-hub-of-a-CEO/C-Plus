#include

using namespace std;

class base {

public:

int id;

void show() {

cout << "Base::show()" << endl;

}

};

class left : public base { };

class right : public base { };

class derived : public left, public right { };

int main() {

derived d;

// d.id = 10; // Error: Ambiguous

// d.show(); // Error: Ambiguous

// Access using scope resolution

d.left::id = 10;

d.right::id = 20;

cout << "Left ID: " << d.left::id << endl;

cout << "Right ID: " << d.right::id << endl;

d.left::show();

d.right::show();

return 0;

}