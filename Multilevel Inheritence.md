#include

using namespace std;

class Vehicle {

public:

void move() {

cout << "Vehicle is moving." << endl;

}

};

class FlyingObject : public Vehicle {

public:

void fly() {

cout << "Flying object is flying." << endl;

}

};

class Aeroplane : public FlyingObject {

public:

void carryPassengers() {

cout << "Aeroplane is carrying passengers." << endl;

}

};

int main() {

Aeroplane a;

a.move();

a.fly();

a.carryPassengers();

return 0;

}