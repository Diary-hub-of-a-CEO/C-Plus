#include

using namespace std;

class Shape {

public:

int a, b;

void get\_data(int n, int m) {

a = n;

b = m;

}

virtual float area() = 0;

};

class Rectangle : public Shape {

public:

float area() override {

return a \* b;

}

};

class Triangle : public Shape {

public:

float area() override {

return 0.5 \* a \* b;

}

};

int main() {

Rectangle r;

Triangle t;

int length, breadth, base, height;

cout << "Enter the length and breadth of the rectangle: ";

cin >> length >> breadth;

r.get\_data(length, breadth);

cout << "Area of the rectangle is: " << r.area() << endl;

cout << "\\nEnter the base and height of the triangle: ";

cin >> base >> height;

t.get\_data(base, height);

cout << "Area of the triangle is: " << t.area() << endl;

return 0;

}