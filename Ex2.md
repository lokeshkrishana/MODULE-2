# Ex.No:2
# Ex.Name:Write A CPP Program to create class RectangleBox and calculate the volume of the rectangleBoxe use of static member variable in the class RectangleBox.
## Date:
## Aim:
To create a class RectangleBox with static member variable to count the number of boxes created and calculate the volume of each rectangle box.

## Algorithm:

1.Start
2.Define class RectangleBox with private members for length, width, height.
3.Define a static member variable to count number of objects created.
4.Create a constructor to initialize dimensions and increment the static count variable.
5.Create a member function to calculate and return the volume.
6.Create a member function to display the count of RectangleBox objects created.
7.In the main function, create multiple RectangleBox objects with user inputs.
8.Display volume for each object and total count of objects created using static variable.
9.End

## Program:
#include <iostream>
using namespace std;

class RectangleBox {
private:
    double length, width, height;
    static int boxCount;  // Static member to count number of boxes

public:
    RectangleBox(double l, double w, double h) {
        length = l;
        width = w;
        height = h;
        boxCount++;
    }

    double volume() {
        return length * width * height;
    }
    static int getBoxCount() {
        return boxCount;
    }
};
int RectangleBox::boxCount = 0;
int main() {
    int n;
    cout << "Enter number of RectangleBoxes: ";
    cin >> n;

    RectangleBox* boxes = new RectangleBox[n];  
        for (int i = 0; i < n; i++) {
        double l, w, h;
        cout << "Enter length, width and height for box " << i+1 << ": ";
        cin >> l >> w >> h;
        boxes[i] = RectangleBox(l, w, h);
    }
    for (int i = 0; i < n; i++) {
        cout << "Volume of box " << i+1 << " = " << boxes[i].volume() << endl;
    }
    cout << "Total number of RectangleBox objects created: " << RectangleBox::getBoxCount() << endl;
    delete[] boxes;  // Clean up dynamically allocated array
    return 0;
}
## Output:

Enter number of RectangleBoxes: 3
Enter length, width and height for box 1: 2 3 4
Enter length, width and height for box 2: 5 5 5
Enter length, width and height for box 3: 1.5 2 3
Volume of box 1 = 24
Volume of box 2 = 125
Volume of box 3 = 9
Total number of RectangleBox objects created: 3

## Result:
The program successfully demonstrates the use of a static member variable to count the number of RectangleBox objects created and calculates the volume of each box based on user input.
