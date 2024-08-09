#Exp_5

AIM:
To study and implement C++ decision making statements.

if Statement:
The if statement evaluates a condition. If the condition is true, the code block inside the if statement is executed.

if-else Statement:
This extends the if statement by adding an else block. If the condition is false, the code inside the else block is executed.

switch Statement:
Used for handling multiple possible values of a single variable. It selects a block of code to execute based on the variable’s value.

Calculator Statement:
It is used for doing mathematical calculations among some given values.

CODE:
1.

```
using namespace std;
int main() 
{
    double n1, n2, n3;
    cout << "Enter three numbers: ";
    cin >> n1 >> n2 >> n3;
    if(n1 >= n2 && n1 >= n3)
        cout << "Largest number: " << n1;
    else if(n2 >= n1 && n2 >= n3)
        cout << "Largest number: " << n2;
    else 
        cout << "Largest number: " << n3;
        return 0;
}
```
2.
```
#include <iostream>
using namespace std;
int main() 
{
    double n1, n2, n3;
    cout << "Enter three numbers: ";
    cin >> n1 >> n2 >> n3;
    if (n1 >= n2) 
    {
        if (n1 >= n3)
            cout << "Largest number: " << n1;
        else
            cout << "Largest number: " << n3;
    }
    else {
        if (n2 >= n3)
            cout << "Largest number: " << n2;
        else
            cout << "Largest number: " << n3;
    }
    return 0;
}
```
3.
```
#include<iostream>
using namespace std;

int main() {
    char oper;
    float num1, num2;

    cout << "Enter an operator (+, -, *, /): ";
    cin >> oper;
    cout << "Enter two numbers: " << endl;
    cin >> num1 >> num2;

    switch (oper) {
        case '+':
            cout << num1 << " + " << num2 << " = " << num1 + num2 << endl;
            break;
        case '-':
            cout << num1 << " - " << num2 << " = " << num1 - num2 << endl;
            break;
        case '*':
            cout << num1 << " * " << num2 << " = " << num1 * num2 << endl;
            break;
        case '/':
            if (num2 != 0)
                cout << num1 << " / " << num2 << " = " << num1 / num2 << endl;
            else
                cout << "Error! Division by zero." << endl;
            break;
        default:
            cout << "Error! The operator is not correct" << endl;
            break;
    }

    return 0;
}
```
4.
```
#include<iostream>
using namespace std;

int main()
{
    int choice;
    cout << "1. Monday" << endl
         << "2. Tuesday" << endl
         << "3. Wednesday" << endl
         << "4. Thursday" << endl
         << "5. Friday" << endl
         << "6. Saturday" << endl
         << "7. Sunday" << endl;
    cout << "Enter your choice: ";
    cin >> choice;
    
    switch(choice) {
        case 1:
            cout << "Monday" << endl;
            break;
        case 2:
            cout << "Tuesday" << endl;
            break;
        case 3:
            cout << "Wednesday" << endl;
            break;
        case 4:
            cout << "Thursday" << endl;
            break;
        case 5:
            cout << "Friday" << endl;
            break;
        case 6:
            cout << "Saturday" << endl;
            break;
        case 7:
            cout << "Sunday" << endl;
            break;
        default:
            cout << "Wrong Input" << endl;
            break;
    }
    
    return 0;
}
```
OUTPUT:
1.

<img width="281" alt="Screenshot 2024-08-09 at 17 49 57" src="https://github.com/user-attachments/assets/c69b09ca-8a7b-4660-aac3-e32993a04c4f">

2.

<img width="286" alt="Screenshot 2024-08-09 at 17 50 21" src="https://github.com/user-attachments/assets/1334bec7-570d-4a76-8d25-a2ec536b29fd">

3.

<img width="307" alt="Screenshot 2024-08-09 at 17 50 48" src="https://github.com/user-attachments/assets/7fef6157-7bf5-4388-a2d0-75e4c5998d0d">

4.

<img width="482" alt="Screenshot 2024-08-09 at 17 51 13" src="https://github.com/user-attachments/assets/b83cfe58-056e-4af9-a5c1-5b0b2e09590d">

Conclusion:
Decision-making statements in programming control the flow of execution based on conditions. The if-else statement executes different code blocks depending on whether a condition is true or false, while the nested if else statement allows for multiple conditions to be checked in sequence. The switch statement provides a way to select one of many code blocks to execute based on the value of an expression, ideal for handling discrete values. calculator helps in doing mathematical operations.
