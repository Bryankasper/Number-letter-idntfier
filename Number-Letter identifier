#include <iostream>
#include <sstream>
#include <vector>

using namespace std;

int main() {
    vector<int> nums;
    string line;
    int sum = 0;

    cout << "Enter a list of integers separated by spaces: ";
    getline(cin, line);

    istringstream iss(line);
    while (iss) {
        int num;
        iss >> num;

        if (iss.fail()) {
            iss.clear();
            string word;
            iss >> word;

            cerr << "Error: " << word << " is not an integer" << endl;
        } else {
            nums.push_back(num);
            sum += num;
        }
    }

    cout << "The sum of the numbers is " << sum << endl;
    cout << "The numbers are: ";
    for (int i = 0; i < nums.size(); i++) {
        if (i > 0) {
            cout << ", ";
        }
        cout << nums[i];
    }
    cout << endl;

    return 0;
}
