#include

#include

using namespace std;

int main() {

map marks;

marks\["Sashwat"\] = 99;

marks\["Anish"\] = 89;

marks\["Safal"\] = 80;

cout << "Student Marks:\\n";

for (auto &p : marks) {

cout << p.first << " : " << p.second << "\\n";

}

auto it = marks.find("Anish");

if (it != marks.end()) {

cout << "\\nAnish's Marks = " << it->second << endl;

} else {

cout << "\\nStudent not found." << endl;

}

return 0;

}