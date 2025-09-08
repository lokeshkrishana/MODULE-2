# Ex.No:1
# Ex.Name:Write A CPP Program to allocate memory dynamically for a double array. (Note: p_array = new type [size]; )
## Aim:
To write A CPP Program to allocate memory dynamically for an character variable. (Note: p_var = new typename;)


## Algorithm:
Start

Define a class var_space with a public function allocateSpace().

Inside allocateSpace() function:

Dynamically allocate memory for a single character (ptr = new char).

Read a character from user input and store it in the allocated memory location (cin >> *ptr).

Display the character value stored (cout << "Character Value is : " << *ptr).

In the main() function:

Create an object s of class var_space.

Call the function s.allocateSpace().

End




## Program:
#include <iostream>
using namespace std; 
class var_space
{
  public:
  void allocateSpace()
  {
    char *ptr = new char;
    cin >> *ptr;
    cout << "Character Value is : " << *ptr;
  }
};
int main()
{
   var_space s;
   s.allocateSpace();
   return 0;
}


## Output:
<img width="1329" height="269" alt="image" src="https://github.com/user-attachments/assets/e65c2d88-9b0f-49ef-9d15-b48c31fef6da" />



## Result:
Hence the program is executed successfully.
