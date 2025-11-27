# cpp-fundamentals-practice
In this I have cleared the basics of C++, moving from basics to advanced

Basic information:
1) #include <iostream> is the built in library in c++ that defines input/output (cout,cin) to machine and where data is stored.
2) using namespace std; is the standard that we use
3) ; is the terminator which defines the machine that the line end here and move to next line and execute the next line code
4) int main () is the function in which we write our main code to be executed in it and also it is very important when we use classes in oop
5) {These curly braces are the main body where we write our program to be executed } Main Block of our program
6) cout is used to get the output showed to us in terminal
7) we use cin to get the input from user


Code # 1: Find the area of the circle.
''' cpp
#include <iostream>
using namespace std;
int main () {
    float radius;
    
    cout<<"Enter Radius: ";
    cin>>radius;

    float area = 3.14159265 * radius * radius;  // frormula: Area = Pi x r2
    cout<<"Area of Circle: "<<area;

    return 0;
}
'''

Code # 2: Arithmatic operations
''' cpp
#include <iostream>
using namespace std;
int main() {
    // int x = 7, y = 2;

    // cout<<"x * y = "<<x*y<<endl;
    // cout<<"x / y = "<<x/y<<endl;
    // cout<<"x + y = "<<x+y<<endl;
    // cout<<"x - y = "<<x-y<<endl;

    float x = 7, y = 2;

    cout<<"x * y = "<<x*y<<endl;
    cout<<"x / y = "<<x/y<<endl;
    cout<<"x + y = "<<x+y<<endl;
    cout<<"x - y = "<<x-y<<endl;
}
'''

Code # 3: ASCII value to character using Typecasting
''' cpp
#include <iostream>
using namespace std;
int main () {
    while (true) {
    int num;
    cout<<"Enter any number: ";
    cin>>num;
    
    char value = (char)num;
    cout<<"The ASCII value of "<<num<<" is "<<value;
    cout<<endl;
    }
    cout<<endl;
    return 0;
}
'''

Code # 4: Finding ASCII value
''' cpp
#include <iostream>
using namespace std;
int main () {

    char ch;
    cout<<"Enter any character: ";
    cin>>ch;

    int value = (int)ch;
    cout<<"The ASCII value of "<<ch<<" is "<<value;
    return 0;
}
'''

Code # 5: Problem solving: Using float data-type but getting answer in integer
''' cpp
#include <iostream>
using namespace std;
int main () {

    float a = 7/22 * (3.14 + 2) * 3/5;
    cout<<a<<endl;
    cout<<endl;
    // Note that if value is int/float form the answer will be in float
    // Also if the value is in float/int form then answer will be in float

    cout<<5/2<<endl; // compiler will see it as int/int by default so output will be in int
    cout<<5.0/2<<endl; // compiler will see it as float/int by default so output will be in float
    cout<<5/2.0<<endl; // compiler will see it as int/float by default so output will be in float
    cout<<5.0/2.0<<endl; // compiler will see it as float/float by default so output will be in float
    return 0;
}
'''

Code # 6: Increment and Decrement
''' cpp
#include <iostream>
using namespace std;
int main() {
    int x = 7;
    // x = x + 1;
    // x+ = 1;
    // x+ = 5;
    
    
    // cout<<x<<endl;
    // x++; Increment it will add 1 to the value
    // cout<<x;

    cout<<x<<endl;
    --x; // Decrement it will subtract 1 from the value  
    cout<<x;
}
'''

Code # 7: Post and Pre-Increment + Decrement
''' cpp
#include <iostream>
using namespace std;
int main () {
    int x = 5;

    cout<<x<<endl;
    cout<<x++<<endl; //Post-Increment: In this the value of x is incremented, increased after getting the value x
    cout<<x<<endl;
    cout<<endl;

    cout<<x<<endl;
    cout<<x--<<endl; //Post-decrement: In this the value of x is decremented, decreased after getting the value x
    cout<<x<<endl;
    cout<<endl;


    cout<<x<<endl;
    cout<<++x<<endl; //Pre-Increment: In this the value of x is incremented, increased before getting the value x 
    cout<<endl;

    cout<<x<<endl;
    cout<<--x<<endl; //Pre-decrement: In this the value of x is decremented, decreased before getting the value x  
    cout<<endl;
}
'''

Code # 8: Take 3 input from user and output their product
''' cpp
#include <iostream>
using namespace std;
int main () {

    int num1,num2,num3;

    cout<<"Enter 1st number: ";
    cin>>num1;

    cout<<"Enter 2nd number: ";
    cin>>num2;

    cout<<"Enter 3rd number: ";
    cin>>num3;

    cout<< num1 * num2 * num3;
    return 0;
}
'''

Code # 9: Type-casting
''' cpp
#include <iostream>
using namespace std;
int main () {
    // Typecasting is used to convert int --> float, float --> int, int --> char, char --> int
    // generaly to change/convert the data-type according to need

    // Que) Take integer 'x' as input and print half of the numbers

    // Ans) so as we can see if user enter odd number then in integer we could'nt get the correct answer
    // And we are coomanded to do this in integer. So by using typecasting we can modify it to float to get correct answer.

    int x;

    cout<<"Enter a number: ";
    cin>>x;
    float y = (float)x;

    cout<<y/2;
}
'''
Code # 10: Variable upgradation
#include <iostream>
using namespace std;
int main () {
    int x;// declaration
    x = 5;// intialization

    cout<<x<<endl;

    x = 9;

    cout<<x<<endl;
    x = x+10;
    cout<<x<<endl;
     x = x-10;
    cout<<x<<endl;
     x = x-7;
    cout<<x<<endl;
     x = x*10;
    cout<<x<<endl;

     x+= 10;
    cout<<x<<endl;

     x-=10;
    cout<<x<<endl;
    return 0;
}

Code # 11: Make a program to find Volume of sphere
#include <iostream>
using namespace std;
int main () {

    float volume, radius;
    
    cout<<"Enter radius: ";
    cin>>radius;

    volume = (4.0/3.0) * 3.14159265 * radius * radius * radius;

    cout<<"Volume of a sphere is = "<<volume;

    return 0;
}
