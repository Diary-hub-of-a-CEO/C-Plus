#include

#include

#include

using namespace std;

int main() {

vector nums = {40, 10, 30, 20};

nums.push\_back(50);

sort(nums.begin(), nums.end());

cout << "Using Iterator: ";

for (vector::iterator it = nums.begin(); it != nums.end(); ++it) {

cout << \*it << " ";

}

cout << "\\n";

cout << "Using Range-based Loop: ";

for (int n : nums) {

cout << n << " ";

}

cout << "\\n";

return 0;

}