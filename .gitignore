#include <iostream>
#include <Windows.h>

int main() {
    HANDLE hConsole = GetStdHandle(STD_OUTPUT_HANDLE);

    GUID hwid;
    if (CoCreateGuid(&hwid) == S_OK) {
        wchar_t gwidString[39];
        if (StringFromGUID2(hwid, gwidString, sizeof(gwidString) / sizeof(gwidString[0])) != 0) {
            SetConsoleTextAttribute(hConsole, 12);
            std::cout << " _________\n";
            std::cout << "/ ======= \\     COMPUTER HWID: ";
            SetConsoleTextAttribute(hConsole, 10);
            std::wcout << gwidString;
            SetConsoleTextAttribute(hConsole, 12);
            std::cout << "  )\n";
            std::cout << "/ __________\\\n";
            std::cout << "| ___________ |\n";
            std::cout << "| | -       | |\n";
            std::cout << "| |         | |\n";
            std::cout << "| |_________| |________________________\n";
            std::cout << "\\=____________/   GET HWID BY: https://www.miguelfiuza.com\n";
            std::cout << " / \"\"\"\"\"\"\"\"\"\"\" \\                       /\n";
            std::cout << "/ ::::::::::::: \\                  =D-'\n";
            std::cout << "(_________________)\n";

            SetConsoleTextAttribute(hConsole, 7);
        }
    }

    return 0;
}
