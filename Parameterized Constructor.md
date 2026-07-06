#include

using namespace std;

class car{

public:

string brand;

string model;

int year;

car(string x, string y, int z ) {

brand = x;

model = y;

year= z;

}

};

int main(){

car car0obj1("Mercedez", "Sclass", 2001);

car car0obj2("Ferrari", "spyder", 2004);

cout<< car0obj1.brand<< " " << car0obj1.model<< " " << endl;

cout<< car0obj2.brand << " "<< car0obj2.model << " "<< endl;

return 0;

}