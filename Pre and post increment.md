#include

using namespace std;

class Counter {

private:

int value;

public:

Counter(int v = 0) : value(v) {}

// Prefix ++

Counter operator++() {

++value;

return \*this;

}

// Postfix ++

Counter operator++(int) {

Counter temp = \*this;

++value;

return temp;

}

void display() const {

cout << "Value: " << value << endl;

}

};

int main() {

Counter c(5);

cout << "Original: ";

c.display();

Counter c1 = ++c;

cout << "After Prefix ++: ";

c.display();

cout << "Returned: ";

c1.display();

Counter c2 = c++;

cout << "After Postfix ++: ";

c.display();

cout << "Returned: ";

c2.display();

return 0;

}