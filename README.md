# Experiment 5

# Aim: <br>
To study and implement C++ decision making statements. <br>

# Theory: <br>
Conditional statements allow you to make decisions within your programs. Specifically they can be used to execute specific blocks of code for particular situations only. <br>
There are four primary conditional statements in C language: _if statement_, _if-else statement_,_ if-else if-else statement_, and _switch statement_. <br> 
_if:_ The simplest form among conditionals where a certain condition is evaluated and if it evaluates true then certain flow control unit executes its commands. <br>
_if-else:_ This is an extension of the first form since we have the alternative block whose commands get executed provided that the original statement was false when selected. <br>
_if-elseif-else:_ This enables the evaluation of several conditions sequentially until it finds one which is true whereby if this happens its contained or associated block will be executed while ignoring all other blocks. <br>
_switch case:_ This facilitates picking one among many subprograms depending on a variable’s value. So rather than using multiple nested if-else statements we can use switch instead.<br>
<br>
# Code: <br>

```
#include <iostream>
using namespace std;
int main()
{
    int a,b,c;
    cout<<"if-else ladder"<<endl;
    cout<<"Enter the first number: ";
    cin>>a;
    cout<<"Enter the second number: ";
    cin>>b;
    cout<<"Enter the third number: ";
    cin>>c;
// if-elif-else ladder
    if ((a>b) && (a>c))
    {
        cout<<"First number is the largest."<<endl;
    }

    else if ((b>a) && (b>c))
    {
        cout<<"Second number is the largest."<<endl;
    }

    else
    {
        cout<<"Third number is the largest."<<endl;
    }
    cout<<endl;
    cout<<endl;

//nested if
    cout<<"nested if"<<endl;
     if ((a>b) && (a>c))
    {
        if (b>c)
        cout<<"Sum of first and second number: "<<a+b<<endl;
        else
        cout<<"Sum of first and third number: "<<a+c<<endl;
    }
    else if ((b>a) && (b>c))
    {
        if (a>c)
        cout<<"Subtraction of second and first number: "<<b-a<<endl;
        else
        cout<<"Subtraction of second and third number: "<<b-c<<endl;
    }
    else
    {
        if (a<b)
        cout<<"Product of third and first number: "<<c*a<<endl;
        else
        cout<<"Product of third and second number: "<<c*b<<endl;
    }

    cout<<endl;
    cout<<endl;
    //switch case
    cout<<"switch case"<<endl;
    int ch;
    float ans;
    cout<<"Enter the first number: ";
    cin>>a;
    cout<<"Enter the second number: ";
    cin>>b;
    cout<<"Press 1 for addition."<<endl;
    cout<<"Press 2 for subtraction. "<<endl;
    cout<<"Press 3 for multiplication. "<<endl;
    cout<<"Press 4 for division"<<endl;
    cout<<"Enter your choice: ";
    cin>>ch;

    switch (ch)
    {
    case 1:
    {
        ans = a + b;
        cout<<"Sum: "<<ans;
        break;
    }

    case 2:
    {
        ans = a - b;
        cout<<"Subtraction: "<<ans;
        break;
    }
    
    case 3:
    {
        ans = a * b;
        cout<<"Product: "<<ans;
        break;
    }

        case 4:
    {
        ans = a / b;
        cout<<"Division "<<ans;
        break;
    }

    default:
    {
        cout<<"INVALID INPUT";
    }
        break;
    }
}
```

# Output: 

![image](https://github.com/user-attachments/assets/6ef95412-a180-45d0-b168-768a2db0b72d)<br>
![image](https://github.com/user-attachments/assets/3e7ea3f8-4147-4824-846c-02748a58e277)



# Conclusion: <br>
&#8594; We learnt about conditional statements and their use case. <br>
&#8594; We learnt how to utilize these statements efficiently. <br>
<br>
