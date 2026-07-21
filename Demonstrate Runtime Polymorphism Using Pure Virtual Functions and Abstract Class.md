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

#include

#include

using namespace std;

class Shape

{

public:

virtual double area() const = 0;

virtual double perimeter() const = 0;

virtual ~Shape() {}

};

class Circle : public Shape

{

private:

double radius;

public:

Circle(double r) : radius(r) {}

double area() const override

{

return 3.14 \* radius \* radius;

}

double perimeter() const override

{

return 2 \* 3.14 \* radius;

}

};

class Rectangle : public Shape

{

private:

double width;

double height;

public:

Rectangle(double w, double h) : width(w), height(h) {}

double area() const override

{

return width \* height;

}

double perimeter() const override

{

return 2 \* (width + height);

}

};

int main()

{

vector shapes;

shapes.push\_back(new Circle(5));

shapes.push\_back(new Rectangle(4, 6));

for (Shape\* s : shapes)

{

cout << "Area = " << s->area() << endl;

cout << "Perimeter = " << s->perimeter() << endl;

cout << endl;

}

for (Shape\* s : shapes)

{

delete s;

}

return 0;

}

return 0;

}