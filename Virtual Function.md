#include

using namespace std;

class Animal {

public:

virtual void speak() {

cout << "Animal makes a sound" << endl;

}

};

class Dog : public Animal {

public:

void speak() override {

cout << "Woof! Woof!" << endl;

}

};

int main() {

Animal\* ptr;

Dog myDog;

ptr = &myDog;

ptr->speak();

return 0;

}