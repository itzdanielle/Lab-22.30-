# Lab-22.30-
#include <iostream>
using namespace std;

int main() {
  const int SIZE = 4;
  int grades[SIZE]; // there are 5 grades since the amount = 5
  double average;
  cout << "Enter " << SIZE << " grades:\n";

  for (int i = 0; i < SIZE; i++)
  {
    cin >> grades[i]; // user inputs 5 different grades
  }

  int sum = 0;
  cout << endl;
  for (int i = 0; i < SIZE; i++)
  {
    cout << "Element " << i+1 << " is " << grades[i] << endl;// This is for the element 1-5 displayed for each grade entered.
    sum = sum + grades[i]; // the total amount of all the grades entered
  }
    average = sum / SIZE;
    cout << "The average of all the elements is " << average << endl;
  cout << "The sum of the " << SIZE << " numbers is " << sum << endl;
}
