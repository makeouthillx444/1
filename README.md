# animal

#include <iostream>
#include <string>

using namespace std;

// Базовый класс
class Animal {
protected:
    string name;
    int age;

public:
    Animal(string name, int age) {
        this->name = name;
        this->age = age;
    }

    void Eat() {
        // Заглушка
    }

    void Sleep() {
        // Заглушка
    }
};

// Класс Птица
class Bird : public Animal {
public:
    Bird(string name, int age) : Animal(name, age) {}

    void Fly() {
        // Заглушка
    }
};

// Класс Рыба
class Fish : public Animal {
public:
    Fish(string name, int age) : Animal(name, age) {}

    void Swim() {
        // Заглушка
    }
};

// Класс Млекопитающее
class Mammal : public Animal {
public:
    Mammal(string name, int age) : Animal(name, age) {}

    void Walk() {
        // Заглушка
    }
};

int main() {
    return 0;
}
