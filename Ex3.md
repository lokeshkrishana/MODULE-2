# Ex.No:3
# Ex.Name:write a program to find the factorial of n Number using class methods(define a method with in class) .

## Aim:
To write a program to find the factorial of n Number using class methods(define a method with in class) .

## Algorithm:
Start

Define a class Factorial with a member function fact(int a).

In fact(int a):

Store the input number in a local variable al.

Initialize product = 1.

Repeat a loop i from 1 to al:

Multiply product by i.

After the loop ends, print the factorial value (product).

In the main() function:

Declare an integer variable v.

Read input number v from user.

Create an object f of class Factorial.

Call the function f.fact(v).

End




## Program:
#include <iostream>
using namespace std;
class Factorial{
  public:
  void fact(int a){
      int al = a;
      int product=1;
      for(int i=1;i<=al;i++)
      {
          product = product * i;
      }
      cout << "The Factorial of given number is:" << product;
  }
};

int main()
{
    int v;
    cin >> v;
    Factorial f;
    f.fact(v);
    return 0;
}


## Output:
<img width="1329" height="269" alt="image" src="https://github.com/user-attachments/assets/88aacce6-1aa3-489d-9743-08418cf26485" />



##Result:
Hence the program is executed successfully.
