# Exp-13

## Aim - 
To study and implement constructor overloading.

## Theory - 
Constructors are special class functions automatically called when an object is created. 
Constructor overloading occurs when a class has multiple constructors with the same name but different parameter lists. 
Each must have a unique set of arguments, distinguished by the number and type of parameters.

Use cases for constructor overloading include:
Offering flexibility in how objects are created.
Providing various ways to initialize an object based on the input data.
Centralizing object initialization in the constructors, which improves code readability and maintenance.
Allowing multiple methods to instantiate objects based on specific needs.

## Code - 
```
# include<iostream>
using namespace std;

class room
{
    private:
    double l,b;

    public:
    room()
    {
        l = 1.2;
        b = 2.3;
    }
    room(double len, double bre)
    {
        l = len;
        b = bre;
    }
    room(double len)
    {
        l = len;
        b = 4.5;
    }
    double area()
    {
        return l*b;
    }

};
int main()
{
    room r1,r2(6.7,7.8),r3(9.1);
    cout<<"No parameter passed: "<<endl;
    cout<<"Area: "<<r1.area()<<endl;
    cout<<"Two parameters passed: "<<endl;
    cout<<"Area: "<<r2.area()<<endl;
    cout<<"One parameter passed: "<<endl;
    cout<<"Area: "<<r3.area()<<endl;
}
```

## Output - 
![image_2024-09-10_152342187](https://github.com/user-attachments/assets/25dad689-999a-4b15-ab13-c7b8e73c4585)

## Conclusion - 
→ We learnt about constructor overloading in C++.
→ We learnt the use case of constructor overloading in C++.

