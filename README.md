# CODSOFT-SIMPLE-CALCULATOR
Write a C++ program to develop a calculator program that performs basic arithmetic operations such as addition, subtraction, multiplication and division. Allow the user to input two numbers and choose an operation to perform.

#include <iostream>

using namespace std;

int main() {
  double num1, num2;
  char operation;

  cout << "Enter the first number: ";
  cin >> num1;

  cout << "Enter the second number: ";
  cin >> num2;

  cout << "Enter the operation (+, -, *, /): ";
  cin >> operation;

  switch (operation) {
    case '+':
      cout << "Result: " << num1 + num2 << endl;
      break;
    case '-':
      cout << "Result: " << num1 - num2 << endl;
      break;
    case '*':
      cout << "Result: " << num1 * num2 << endl;
      break;
    case '/':
      if (num2 != 0) {
        cout << "Result: " << num1 / num2 << endl;
      } else {
        cout << "Error: Division by zero!" << endl;
      }
      break;
    default:
      cout << "Error: Invalid operation!" << endl;
      break;
  }

  return 0;
}
