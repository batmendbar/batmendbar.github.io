# Хувьсагч

Програмын хувьд хувьсагч нь математикт ашиглагддаг хувьсагчаас өөр ойлголт юм. Математикт хувьсагч гэж үл мэдэгдэх утгыг илэрхийлдэг бол програмчлалын хувьд хувьсагч нь өгөгдөл хадгалах сав юм. 

Хувьсагчийг зарлахдаа эхлэээд агуулах утгын төрөл дараа нь нэрийг нь бичдэг. Шинээр зарлагдсан хувьсагч буюу сав нь эхэндээ дотроо утгагүй байдаг. Жишээ нь: 

```cpp
#include <iostream>

int main() {
    int minii_huvisagch; // Шинэ хувьсагч үүсгэв. Одоохондоо дотроо утгагүй
    return 0;
}
```

C++ хэлэнд утга олгох '=' үйлдлээр хувьсагч буюу саванд хадгалагдаж буй утгыг өөрчлөх боломжтой. Анхаарах зүйл нь '=' нь утга олгох үйлдэл бөгөөд математикт ашиглагддаг тэнцүү гэсэн ойлголт биш юм. Доорх жишээнд тулгуурлан уг ойлголтыг гүнзгийрүүлэн судлая: 

## Жишээ 1

```cpp
#include <iostream>

int main() {
    int x = 5; // Шинэ хувьсагч үүсгэн дотор нь 5 гэсэн утга хийх
    std::cout << x;
    return 0;
}
```

Дээрх код нь `x` гэсэн хувьсагч үүсгэж байгаа ба дотор нь 5 гэсэн утга оноож байна. Иймд c++ нь `std::cout << x;` мөрийг ажиллуулахын тулд `x` хувьсагчийг утгаар нь солино. Иймд дээрх код нь доорх код болгон солигдоно.

```cpp
#include <iostream>

int main() {
    int x = 5;
    std::cout << 5;
    return 0;
}
```

## Жишээ 2

```cpp

#include <iostream>

int main() {
    int x = 5; // x хувьсагчийг үүсгэн 5 утга оноож байна
    x = 10; // Хувьсагчийн өмнөх утгыг 10-аар сольж байна
    std::cout << x;
    return 0;
}
```

Дээрх код нь `x` гэсэн хувьсагч үүсгэж байгаа ба дотор нь 5 гэсэн утга оноож байна. Дараа нь `x` хувьсагчийн утгыг 10-аар сольж байна. Иймд c++ нь `std::cout << x;` мөрийг ажиллуулахын тулд `x` хувьсагчийг тухайн мөч дэх утга буюу 10-аар солино. Иймд дээрх код нь доорх код болгон солигдоно.

```cpp

#include <iostream>

int main() {
    int x = 5;
    x = 10;
    std::cout << 10;
    return 0;
}
```

