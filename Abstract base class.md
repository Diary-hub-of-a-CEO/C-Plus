#include

using namespace std;

// Abstract Base Class

class Shape {

public:

virtual void area() = 0; // Pure virtual function

};

// Derived Class for Circle

class Circle : public Shape {

private:

float radius;

public:

Circle(float r) {

radius = r;

}

void area() override {

cout << "Area of Circle = " << 3.1416 \* radius \* radius << endl;

}

};

// Derived Class for Rectangle

class Rectangle : public Shape {

private:

float length, breadth;

public:

Rectangle(float l, float b) {

length = l;

breadth = b;

}

void area() override {

cout << "Area of Rectangle = " << length \* breadth << endl;

}

};

int main() {

Circle c(5);

Rectangle r(10, 6);

c.area();

r.area();

return 0;

}