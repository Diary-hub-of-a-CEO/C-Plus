#include

using namespace std;

class Person{

private:

string name;

int age;

public:

Person(const std::string& name, int age) {

this->name= name;

this->age= age;

}

void displayInfo(){

std::cout<< "Name:"<< this->name << std::endl;

std::cout<< "Age:"<< this->name <

}

void updateAge(int newage){

this->age = newage;

}

};

int main(){

Person person("Kapil", 10);

person.displayInfo();

person.updateAge(20);

cout<< "After updating age:"<< endl;

person.displayInfo();

return 0;

}

}

}