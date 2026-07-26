#include

using namespace std;

// Base class

class Vehicle {

public:

void start() {

cout << "Vehicle is starting." << endl;

}

};

class Car : public Vehicle {

public:

void drive() {

cout << "Car is driving." << endl;

}

};

int main() {

Car c;

c.start();

c.drive();

return 0;

}