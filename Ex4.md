# Ex.No:4
# Ex.Name:Write A CPP Program to create class  SquareBox and calculate the volume of the SquareBox, make use of static member variable in the class SquareBox. (Note: l=b=h)

## Aim:
To Write A CPP Program to create class  SquareBox and calculate the volume of the SquareBox, make use of static member variable in the class SquareBox. (Note: l=b=h)

## Algorithm:
Start

Define a class Square with:

Private data members: length, breadth, and depth.

Static data member: objCount initialized to 0 (to count total objects).

Constructor Square(int a, int b, int c):

Assign parameters a, b, c to length, breadth, and depth.

Print "Constructor called.".

Increment objCount by 1.

Member function Volume():

Compute length × breadth × depth.

Print the volume.

In the main() function:

Read three integers a1, a2, a3 from the user.

Create object s using Square(a1, a2, a3).

Call s.Volume() to display volume of first cuboid.

Read three integers b1, b2, b3 from the user.

Create another object j using Square(b1, b2, b3).

Call j.Volume() to display volume of second cuboid.

Print "Total objects: " followed by the value of Square::objCount.

End




## Program:
#include<iostream>
using namespace std;
class Square {
  private:
  int length;
  int breadth;
  int depth;
  public:
  static int objCount;
  Square(int a,int b,int c){
      length = a;
      breadth = b;
      depth = c;
      cout << "Constructor called." << endl;
      objCount++;
  }
  void Volume(){
      cout << "Volume :" << length*breadth*depth << endl;
  }
};
int Square::objCount = 0;
int main()
{
    int a1,a2,a3;
    cin >> a1 >> a2 >> a3;
    Square s(a1,a2,a3);
    s.Volume();
    int b1,b2,b3;
    cin >> b1 >> b2 >> b3;
    Square j(b1,b2,b3);
    j.Volume();
    cout << "Total objects: " << Square::objCount;
    return 0;
}


## Output:
<img width="1411" height="434" alt="image" src="https://github.com/user-attachments/assets/0fb4184d-2a3f-4f37-8dc7-d507372a0fdc" />



## Result:
Hence the program is executed successfully

