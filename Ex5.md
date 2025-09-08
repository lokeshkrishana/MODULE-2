# Ex.No:5
# Ex.Name:Write a CPP Program to compute the total and percentage of a student by Function Overloading

## Aim:
To write a CPP Program to compute the total and percentage of a student by Function Overloading

## Algorithm:
Start

Define a function compute(int m1, int m2, int m3)

Add the three marks (m1 + m2 + m3).

Return the total.

Define a function percentage(float avg)

Divide the given value by 3 (avg / 3).

Return the result.

In the main() function:

Declare integer variables mk1, mk2, mk3.

Take input for the three marks.

Call compute(mk1, mk2, mk3) to calculate the total and store it in tot.

Print "Total=" followed by tot.

Call percentage(tot) to calculate the percentage and store it in perc.

Print "Percentage=" followed by perc.

End




## Program:
#include<iostream>
using namespace std;
int compute(int m1, int m2, int m3){ 
    int total = m1+m2+m3;  
    return total;
}
float percentage(float avg){ 
    avg = avg/3; 
    return avg;
}int main(){  
    int mk1, mk2,mk3; 
    cin>>mk1>>mk2>>mk3;  
    float tot = compute(mk1, mk2, mk3);  
    cout<<"Total="<<tot<<endl;     
    float perc= percentage(tot);  
    cout<<"Percentage="<<perc;
}


## Output:
<img width="1357" height="215" alt="image" src="https://github.com/user-attachments/assets/71362a75-8266-4310-a5ab-2a2c71319d46" />



## Result:
Hence the program executed successfully.

