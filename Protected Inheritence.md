#include

using namespace std;

class Animal {

public:

void speak() {

cout << "This is an animal." << endl;

}

};

class Dog : protected Animal {

public:

void display() {

speak();

}

};

int main() {

Dog d;

d.display();

return 0;

}