#include <iostream>
using namespace std;

int main() {
    int arr[5], total = 0;
    float avg;

    cout << "Enter marks of 5 subjects:\n";

    for (int i = 0; i < 5; i++) {
        cin >> arr[i];
        total = total + arr[i];
    }

    cout << "The total marks are: " << total << endl;

    avg = total / 5.0;
    cout << "The average marks are: " << avg << endl;

    if (avg >= 70)
        cout << "Distinction";
    else if (avg >= 60)
        cout << "First Class";
    else if (avg >= 50)
        cout << "Second Class";
    else if (avg >= 40)
        cout << "Pass";
    else
        cout << "Fail";

    return 0;
}
