#include

#include

using namespace std;

template

class Box {

private:

T item;

public:

Box(T val) : item(val) {}

T get() const {

return item;

}

void set(T val) {

item = val;

}

};

int main() {

Box intBox(10);

Box strBox("Hello");

cout << intBox.get() << "\\n";

intBox.set(intBox.get() + 5);

cout << intBox.get() << "\\n";

cout << strBox.get() << "\\n";

return 0;

}