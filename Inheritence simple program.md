#include

using namespace std;

class Animal {

public:

void speak() {

cout << "Animal makes a sound" << endl;

}

};

class Dog : public Animal {

public:

void speak() {

cout << "Dog barks" << endl;

}

};

int main() {

Animal a;

Dog d;

a.speak();

d.speak();

return 0;

}