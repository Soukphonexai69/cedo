#include <iostream>

class Rectangle {
private:
    double width;
    double height;

public:
    // Constructor: khởi tạo width và height với giá trị đầu vào
    Rectangle(double w, double h) {
        width = w;
        height = h;
    }

    // Getter cho width
    double getWidth() const {
        return width;
    }

    // Getter cho height
    double getHeight() const {
        return height;
    }

    // Setter cho width
    void setWidth(double w) {
        width = w;
    }

    // Setter cho height
    void setHeight(double h) {
        height = h;
    }

    // Phương thức tính diện tích hình chữ nhật
    double calculateArea() const {
        return width * height;
    }

    // Phương thức hiển thị thông tin hình chữ nhật
    void display() const {
        std::cout << "Thông tin hình chữ nhật:\n";
        std::cout << "Chiều rộng: " << width << "\n";
        std::cout << "Chiều cao: " << height << "\n";
        std::cout << "Diện tích: " << calculateArea() << "\n";
    }
};

// Hàm main để kiểm tra lớp Rectangle
int main() {
    // Tạo một hình chữ nhật với chiều rộng 4 và chiều cao 6
    Rectangle rect(4, 6);

    // Hiển thị thông tin hình chữ nhật
    rect.display();

    return 0;
}
