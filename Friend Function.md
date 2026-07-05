#include

using namespace std;

class Rectangle {

private:

int width;

int height;

public:

Rectangle(int w, int h) : width(w), height(h) {}

friend void displayArea(Rectangle r);

int area= r.width \* r.height;

cout<< "Area: " << area << endl;

}

int main() {

Rectangle rect(5,10);

displayArea(rect);

return 0;

}