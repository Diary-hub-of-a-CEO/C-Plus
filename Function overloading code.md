#include

using namespace std;

//Overloaded functions to calculate the area

double area(double radius) { //For circle

return 3.14159 \* radius \*radius;

}

double area (double length , double width) {

// For rectangle

return length \*width;

}

int main(){

cout << "Area of circle (r=5): "<< area(5.0) << endl;

cout <<"Area of rectangle (4\*5) :"<< area(4.0, 5.0) << endl;

return 0;

}