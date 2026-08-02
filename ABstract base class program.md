#include

using namespace std;

class Account

{

public:

virtual void CalculateInterest() = 0;

};

class SavingAccount : public Account

{

public:

void CalculateInterest()

{

cout << "Saving Interest = 8%" << endl;

}

};

class CurrentAccount : public Account

{

public:

void CalculateInterest()

{

cout << "Current Account Interest = 0%" << endl;

}

};

int main()

{

SavingAccount s;

CurrentAccount c;

s.CalculateInterest();

c.CalculateInterest();

return 0;

}