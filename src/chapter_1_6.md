# using namespace std;

```cpp
#include <iostream> 

int main() {
    std::cout << "Сайн уу, Дэлхий?"; 
    std::cout << "Сайн уу, Дэлхий?"; 
    std::cout << "Сайн уу, Дэлхий?"; 
    std::cout << "Сайн уу, Дэлхий?"; 
    std::cout << "Сайн уу, Дэлхий?"; 
    std::cout << "Сайн уу, Дэлхий?"; 
}
```

Бид `using namespace std;` гэж бичиж болно. Энэ нь `std::`-г бичих шаардлагагүй болгодог. Жишээ нь:

```cpp
#include <iostream> 
using namespace std;

int main() {
    cout << "Сайн уу, Дэлхий?"; 
    cout << "Сайн уу, Дэлхий?"; 
    cout << "Сайн уу, Дэлхий?"; 
    cout << "Сайн уу, Дэлхий?"; 
    cout << "Сайн уу, Дэлхий?"; 
    cout << "Сайн уу, Дэлхий?"; 
}
```