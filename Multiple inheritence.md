#include

using namespace std;

class printer {

public:

void print() {

cout << "Printing...." << endl;

}

};

class scanner {

public:

void scan() {

cout << "Scanning...." << endl;

}

};

class Allinone : public printer, public scanner {

public:

void doeverything() {

print();

scan();

}

};

int main() {

Allinone device;

device.doeverything();

return 0;

}