#include <iostream.h>
#include<conio.h>
// Base class
class Animal {
public:
    void eat() {
        cout << "Eating..." << endl;
    }
};
// Single Inheritance
class Dog : public Animal {
public:
    void bark() {
        cout << "Barking..." << endl;
    }
};
// Multilevel Inheritance
class Bulldog : public Dog {
public:
    void play() {
        cout << "Playing..." << endl;
    }
};
// Hierarchical Inheritance
class Cat : public Animal {
public:
    void meow() {
        cout << "Meowing..." << endl;
    }
};
int main() {
    // Single Inheritance
    Dog dog;
    dog.eat();
    dog.bark();
    // Multilevel Inheritance
    Bulldog bulldog;
    bulldog.eat();
    bulldog.bark();
    bulldog.play();
    // Hierarchical Inheritance
    Cat cat;
    cat.eat();
    cat.meow();
getch ();
}
