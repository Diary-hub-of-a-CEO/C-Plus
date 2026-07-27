#include

using namespace std;

// Base class

class Animal {

public:

void eat() {

cout << "Animal is eating." << endl;

}

};

class Dog : public Animal {

public:

void bark() {

cout << "Dog barks." << endl;

}

};

class Cat : public Animal {

public:

void meow() {

cout << "Cat meows." << endl;

}

};

class Cow : public Animal {

public:

void moo() {

cout << "Cow moos." << endl;

}

};

int main() {

Dog d;

Cat c;

Cow w;

d.eat();

d.bark();

c.eat();

c.meow();

w.eat();

w.moo();

return 0;

}